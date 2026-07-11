---
title: "Proposal"
date: 2026-07-01
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Smart Image Platform  
## A Comprehensive AWS Serverless & Event-Driven Solution for Smart Image Storage and Processing  

### 1. Executive Summary  
The **Smart Image Platform** is an advanced cloud solution engineered to automate image uploads, secure storage, dynamic compression, and AI-powered content analysis. By fully leveraging an **AWS Serverless** and **Event-Driven** architecture, the platform guarantees high availability, seamless auto-scaling, and optimal cost efficiency. The entire frontend interface and backend API layer are strictly protected at the edge, utilizing Amazon Cognito to enforce access control restricted to internal organizational accounts.

### 2. Problem Statement  
* **Current Problem:** Traditional file management and image processing systems heavily struggle with resource elasticity when handling sudden spikes in user uploads. Executing image resizing, metadata extraction, and AI classification tags synchronously on legacy servers causes major bandwidth bottlenecks, exhausts compute hardware, and significantly inflates response latency for end-users.  
* **Proposed Solution:** Build a fully asynchronous, decoupled cloud architecture orchestrated by native AWS event triggers. Users interact through a Web interface (React App) authenticated securely via Amazon Cognito. All incoming traffic is filtered at the perimeter by an AWS WAF firewall layered in front of Amazon API Gateway. Raw assets are stored in Amazon S3, instantly triggering downstream AWS Lambda pipelines: one computing branch handles image optimization and compression before pushing outputs to a separate destination bucket, while a parallel branch invokes Amazon Rekognition AI to analyze objects and write catalog indexes into Amazon DynamoDB asynchronously.  
* **Benefits and Return on Investment (ROI):** Eliminates 100% of predictable monthly overhead tied to maintaining 24/7 dedicated compute hardware by embracing a strict Pay-as-you-go pricing model. The initial development and testing phases yield an approximate 80% reduction in infrastructure costs by operating comfortably within the boundaries of the AWS Free Tier. Automating the image tagging process with AI eliminates manual asset indexing labor entirely while significantly improving data metadata catalog accuracy.

### 3. Solution Architecture  
The platform orchestrates Serverless cloud services to streamline chronological data flows, as illustrated in the system execution layout below:

![Smart Image Platform Architecture](/images/2-Proposal/platform_architecture.jpeg)

* **Detailed Execution Flow:**
  1. The user accesses and interacts with the web interface via a **Browser (React App)**.
  2. The client application dispatches authentication credentials to **Amazon Cognito**. Upon successful authentication, the browser receives a valid identity token (ID Token).
  3. The frontend application attaches the token to outbound API requests, passing traffic through the **AWS WAF** perimeter shield.
  4. AWS WAF evaluates the request against core safety rule sets (AWSManagedRulesCommonRuleSet) and rate limiting (RateLimitRule) to block malicious traffic and API spam before routing valid payloads to **Amazon API Gateway**. The API Gateway uses a Cognito Authorizer to cross-check operational permissions.
  5. API Gateway triggers the **AWS Lambda (API Handler Lambda)** to execute backend route routing, validate user quotas against the **DynamoDB UserQuotas** table, manage user profile updates synchronizing back to Cognito User Pool attributes, and safely generate an S3 Presigned PUT URL.
  6. The client browser uses the time-bound Presigned URL to PUT the raw binary image stream directly into the **S3 Bucket (Raw Store)** under the `users/<userId>/` prefix, completely offloading network bandwidth from the core API layer.
  7. The object creation event under the `users/` prefix inside the raw **S3 Bucket** instantly emits a notification that triggers the asynchronous **AWS Lambda (Image Processor Lambda)**.
  8. The Image Processor Lambda handles two processing jobs concurrently:
     * **8.a:** Compresses, optimizes, and resizes the image asset using the `Sharp` library before writing the finalized output securely into the designated **processed S3 Bucket**.
     * **8.b:** Extracts fundamental image file attributes (dimensions, format, byte size, creation timestamp, EXIF metadata) and populates an initial record index with status `PROCESSED` inside **Amazon DynamoDB**.
  9. The generation or modification of item attributes (switching status to `PROCESSED`) within the database automatically emits an event that streams down to trigger the **AWS Lambda (AI Analyzer Lambda)** via DynamoDB Streams.
  10. This Lambda function interacts directly with **Amazon Rekognition** to execute object detection, automatic tag classification, and content moderation checks. It then writes the computed AI labels and moderation status back into the **DynamoDB** table records, updating the final image status to `COMPLETED` (or `FLAGGED` for moderation review).
  11. **Secure Distribution:** When users request to view or download images, the frontend requests time-bound **S3 Presigned GET URLs** via the API Gateway, letting the API Handler securely authorize and distribute short-term URLs for both original files and thumbnails directly from the private buckets.
  12. **Admin Moderation Queue:** Admins check flagged assets using the admin endpoints which query the DynamoDB table via a dedicated moderation index (`GSI2-ModerationIndex`) and can approve/reject items.

### 4. Technical Implementation  
* **Deployment Phases:**
  1. *Research & Architecture Design:* Map out complete application workflows, research programmatic implementation models for S3 Presigned URLs, and layout decoupled event-driven service blueprints (1 Month).
  2. *Cost Projection & Security Perimeter Analysis:* Utilize the AWS Pricing Calculator to map budget thresholds and formulate precise AWS Budget Alerts to mitigate financial risks stemming from programming defects like infinite computing loops (Month 1).
  3. *Core Services Development & Configuration:* Provision default virtual networks, build NoSQL DynamoDB table structures with global secondary indexes, write Lambda runtime code handling target image processing libraries (bundling `Sharp` for `linux-arm64` runtime), and integrate Amazon Rekognition SDK modules (Month 2).
  4. *Frontend Integration, Stress Testing, & Deployment:* Connect the finalized React App user interface, run heavy end-to-end load tests validating concurrent upload streams, purge loose testing assets, and migrate configurations to a production-ready state (Month 3).

* **Technical Requirements:**
  * *Frontend:* Single Page Application (SPA) compiled utilizing **React.js + Vite**, integrating the Amazon Cognito Auth SDK to safely validate sessions and cryptographically parse identity tokens. Network request layers utilize Axios clients to directly push binary multi-part file streams over S3 Presigned targets.
  * *Backend & Cloud Infrastructure:* AWS Lambda runtimes built on Node.js 20.x utilizing TypeScript. Database storage utilizes DynamoDB set to On-Demand capacity allocation with separate tables for metadata (`Images`), upload tracking (`UserQuotas`), and profile details (`UserProfiles`). S3 raw bucket features standard transition to Infrequent Access (90 days), Glacier transition (365 days), and old version deletion (30 days) to optimize costs.

### 5. Roadmap & Implementation Milestones  
* **Month 1:** Complete foundational cloud architecture research tracks; register official AWS developer environments and implement base security configurations (IAM permissions boundaries, Budget alerts).
* **Month 2:** Finalize system technical dependency designs; establish target Amazon API Gateway routing rules, set up DynamoDB tables, and complete production runtime code handling back-end Lambda processing tasks.
* **Month 3:** Build out the React.js client frontend dashboards; initiate thorough end-to-end system testing, populate code repositories with clean engineering documentation on GitHub, and complete the final project handover.

### 6. Budget Estimation  
Financial budgets are estimated against typical MVP pilot testing workloads managing fewer than 5,000 processed images per month, fitting almost entirely within the AWS Free Tier parameters (Permanent and 12-Month introductory terms):

* **AWS Lambda:** 0.00 USD/month (Safely below the 1 million free monthly requests tier).
* **Amazon S3:** ~0.05 USD/month (Allocated for multi-tier raw and optimized image storage, under the 5 GB threshold).
* **Amazon DynamoDB:** 0.00 USD/month (Configured in On-Demand allocation mode, utilizing under 25 GB of free static data allocation).
* **Amazon API Gateway:** 0.00 USD/month (Under the 1 million free introductory REST API call bracket).
* **Amazon Rekognition:** 0.00 USD/month (Operating within the 5,000 free monthly images tier provided by AWS Free Tier).
* **AWS WAF:** ~5.00 USD/month (Flat-rate base charge per Web ACL and basic inspection rules. *Note: Can be safely turned off during local sandbox testing phases to achieve zero-cost overhead*).

*Total Projected Costs:* ~0.00 USD/month (Operating purely inside Free Tier allocations with AWS WAF disabled during sandbox tests) OR ~5.05 USD/month (Operating with edge application firewall shields enabled).

### 7. Risk Management  
* **Risk of Infinite Computing Loops:** A processing Lambda writes optimized assets back into the monitored raw ingestion directory, triggering itself endlessly and depleting available cloud budget credits rapidly.
  * *Mitigation Strategy:* Enforce hard separation lines between media storage zones by provisioning two distinct buckets: a raw input store (`raw-images-bucket`) that holds the exclusive trigger connection to compute functions, and an output store (`processed-images-bucket`) completely detached from automated backend execution triggers. Additionally, S3 notifications are restricted to the `users/` prefix.
* **Denial of Service (DDoS) or API Ingestion Spam:** Malicious external scripts flooding ingress gateways with concurrent fake file requests to artificially drive up Lambda resource executions.
  * *Mitigation Strategy:* Enforce strict edge rate limiting rules via AWS WAF (configured with a flat `RateLimitRule` of 2,000 requests per 5 minutes per IP) at the perimeter and deploy throttling caps (Request per second limits) on specialized target API keys handled by the Amazon API Gateway.
* **Unprotected Public S3 Bucket Data Leakage:** User images exposed publicly due to loose access rules.
  * *Mitigation Strategy:* Enable global Block Public Access attributes on all S3 Buckets. Raw and processed S3 objects are only accessed via temporary S3 Presigned GET URLs generated by the authorized Lambda backend, preventing any direct public access paths.

### 8. Expected Outcomes  
* **Technical Performance:** The client interface achieves ultra-low response latency indicators because computationally taxing media resizing steps and multi-label AI analysis tasks are handled asynchronously downstream.
* **Long-Term Enterprise Value:** Establishes a modular cloud platform blueprint built on Clean Code practices. The system can scale seamlessly from a handful of internal users up to thousands of concurrent transactions without requiring any manual server hardware tuning or management intervention.