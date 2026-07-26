---
title: "Event 3"
date: 2026-07-26
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Event Reflection Report: Agentic AI and the AWS Hackathon Journey

&emsp;**Participation Date:** July 26, 2026  

&emsp;**Role:** Attendee  

&emsp;**Main Content:** Sharing practical Hackathon experiences, building Agentic AI products, designing AWS architectures, optimizing costs, and demonstrating real-world solutions.  

### Event Objectives

* Share practical experiences from participating in Agentic AI Build Week and AWS-related Hackathons.

* Introduce how teams identified problems, developed minimum viable products, and completed their solutions within a limited timeframe.

* Present practical applications of Computer Vision, Generative AI, and Agentic AI in crowd monitoring, business analysis, architecture design, and conversational ordering.

* Help participants better understand how AWS services can be combined to build scalable, secure, observable, and cost-efficient systems.

* Share challenges, lessons learned, teamwork experience, and preparation methods for Hackathon competitions.

* Encourage students and beginners to actively participate in technology events, build products, and learn through practical experience.


### Presentation Teams and Members

#### Team 3KA – The Hackathon Journey

* **Huynh An Khuong**
* **Nguyen Quoc Huy**
* **Ngo Quang Khoi**
* **Hoang Le Thanh Duc**
* **Dang Nguyen Phuoc Loc**
* **Dang Truong Hung**

#### Team SignalScout

* **Le Tan Luc**
* **Do Hoang Hieu**
* **Trieu Quoc Hao**
* **Nguyen Van Duy Khiem**
* **Nguyen Cong Minh**
* **Nguyen Tran Minh Quan**

#### Team Plan V – Solution Architect Professional AI Native App

* **Pham Tien Thuan Phat**
* **Huynh Hoang Long**
* **Le Minh Nghia**
* **Tran Dai Vi**
* **Nguyen An**

#### One Team – Colonel AI

* **Anh Duy**
* **Tran Dong**
* **Doan Trung**
* **Minh Viet**
* **Anshul Roy**


### Key Highlights

## 1. The Hackathon Journey – 24 Hours of Building, Failing, and Learning

Team 3KA shared their complete experience of participating in a 24-hour Hackathon. Instead of focusing only on the final result, the team emphasized the lessons they gained while building the product, encountering errors, changing ideas, and collaborating with other members.

Their journey was divided into four stages:

* Registering and selecting a suitable track.

* Building a product under time pressure.

* Presenting and demonstrating the product to the judges.

* Reviewing the experience and identifying lessons after the competition.

The team joined the Hackathon to challenge themselves beyond the classroom, gain practical experience with AI and AWS, learn how to build an end-to-end product within a short timeframe, and improve their teamwork skills.

### The S.H.E.P.H.E.R.D Project

The team developed a prototype named **S.H.E.P.H.E.R.D**, which stands for:

**Smart Human-flow Evaluation, Prediction, Hazard Detection, Response, and Dispatch**

The system was designed to support crowd-density monitoring in busy locations such as entrances, queues, exhibition booths, and event areas.

In practice, operators may need to monitor multiple cameras and locations simultaneously. Manual monitoring has several limitations:

* Slow response when incidents occur.

* Difficulty scaling as the number of cameras and monitored areas increases.

* Possibility of missing unusual activities.

* Inability to respond quickly when crowd conditions change.

S.H.E.P.H.E.R.D was developed to analyze live camera footage and convert visual data into clear operational information.

Its core capabilities include:

* Detecting and tracking people in video footage.

* Measuring crowd density.

* Evaluating queue conditions.

* Identifying early signs of congestion.

* Predicting overcrowding pressure.

* Generating proactive alerts.

* Recommending staff-dispatch actions.

### Technologies Used

* **YOLO** for detecting objects in images and videos.

* **ByteTrack** for tracking objects across multiple frames.

* **Amazon SageMaker** for supporting cloud-based inference.

* **Amazon Bedrock AgentCore** and **Strands Agent** for building the Agentic AI layer.

* **React Monitoring Dashboard** for displaying monitoring metrics and alerts.

### Agentic AI Layer

The solution included two important Agentic AI components:

#### Autonomous Monitor

* Continuously monitors live crowd metrics.

* Detects signs of congestion.

* Predicts possible overcrowding.

* Automatically generates proactive alerts.

#### Operator Copilot

* Allows operators to ask questions in natural language.

* Provides answers based on live monitoring data.

* Combines prediction tools with operational actions.

* Delivers concise, understandable, and evidence-based responses.

### Challenges Faced by the Team

* Limited prior knowledge of AI.

* First-time experience with several AWS services.

* Very limited development time.

* Difficulty maintaining a reliable live-video stream.

* High inference latency.

* Difficulty preserving object tracking across frames.

* Camera placement affected the quality of the analysis.

* Multiple source-code errors occurred during development.

* The team had to balance the number of features with the available time.

* The AI Agent needed to be proactive, explainable, and capable of recommending suitable actions.

### Lessons from the Hackathon Journey

The team recommended preparing the following items before participating in a Hackathon:

* A clear goal and an early definition of what completion means.

* Required tools, accounts, and starter code.

* Clearly assigned roles for development, design, presentation, and testing.

* A short demo script that has been rehearsed in advance.

* A limited product scope that can be completed and demonstrated reliably.

An important lesson was that a small but complete product is more valuable than a large idea that does not work.


## 2. SignalScout – Corporate Strategic Signal Analysis

SignalScout is an AI platform designed to detect strategic changes and corporate-restructuring signals at an early stage.

In practice, information about a company is often scattered across multiple sources. Collecting, validating, and connecting this information into a reliable conclusion can require a significant amount of time.

SignalScout aims to:

* Collect and validate corporate evidence.

* Detect strategic changes early.

* Identify restructuring signals.

* Analyze financial and operational metrics.

* Develop possible business scenarios.

* Connect scattered signals into a clear narrative.

* Provide supporting evidence for every conclusion.

* Support Maintain, Adapt, or Accelerate decisions.

### Target Users

* Corporate strategy teams.

* Enterprise risk-management teams.

* Competitive-intelligence teams.

* B2B enterprise account-management teams.

### Value of the Solution

* Provides a self-service dashboard.

* Displays analysis reports, timelines, and risk alerts.

* Generates transparent and verifiable results.

* Supports decision-making while keeping humans in control of the final decision.

* Provides supporting evidence rather than presenting unsupported conclusions.

### Technologies and Supporting Platforms

The solution combines the AWS ecosystem with several supporting platforms:

* Amazon Bedrock.

* Amazon Bedrock AgentCore.

* AWS WAF.

* AWS Amplify Hosting.

* Amazon CloudWatch.

* AWS Secrets Manager.

* Amazon DynamoDB.

* AWS Lambda.

* Amazon Route 53.

* AWS CloudTrail.

* Amazon S3 Intelligent-Tiering.

* Amazon API Gateway.

* Amazon Cognito.

* Langfuse.

* TinyFish.

* Apify.

### Cost Analysis and Optimization

The team not only developed the system functions but also estimated operating costs for different usage levels.

According to the presentation, the estimated total AWS service costs were:

* Low-usage scenario: approximately **USD 17 per month**.

* Medium-usage scenario: approximately **USD 35 per month**.

* High-usage scenario: approximately **USD 130 per month**.

When external platforms such as Apify, TinyFish, and Langfuse were included, the estimated total monthly cost ranged from approximately **USD 81 to USD 359**.

The team also proposed a more cost-efficient architecture, demonstrating that system design must balance processing capability, reliability, and operating budget.


## 3. Solution Architect Professional AI Native App

The Plan V presentation focused on using Agentic AI to support the work of a Solution Architect.

During the solution-consulting process, Solution Architects often need to complete many manual tasks:

* Read BRD or PRD documents line by line.

* Extract and categorize requirements.

* Identify missing requirements.

* Draft an initial architecture from a blank page.

* Create architecture diagrams.

* Produce high-level cloud-cost estimates.

* Write Infrastructure as Code.

* Adjust the architecture based on customer feedback.

These activities require significant experience and can take considerable time, especially when the customer requests the solution urgently.

### Proposed Solution

The team developed the **Solution Architect Professional AI Native App**, an AI application capable of:

* Analyzing requirements written in natural language.

* Analyzing structured project-requirement documents.

* Creating a requirements catalogue within a short period.

* Proposing multiple high-level architecture options.

* Supporting both AWS and hybrid-cloud architectures.

* Aligning proposals with company standards.

* Generating editable Draw.io diagrams.

* Using official AWS Architecture Icons.

* Providing directional AWS cost estimates for the `ap-southeast-1` Region.

* Highlighting recommendations, assumptions, and requirement gaps.

* Allowing users to refine the architecture through a chat interface.

* Supporting project-specific custom instructions.

* Supporting the automatic generation of Infrastructure as Code.

### Impact of the Solution

Before using the application:

* Solution Architects had to read BRD or PRD documents manually.

* Each architecture was often started from a blank page.

* Infrastructure as Code had to be written manually.

* Cost estimates depended heavily on individual experience.

After using the application:

* Users could upload documents and communicate using natural language.

* The system could generate a Requirements Catalogue within minutes.

* Solution Architects received a grounded first draft for review and refinement.

* Infrastructure as Code could be generated automatically.

* A directional cost estimate was produced together with the architecture.

An important point was that AI does not completely replace the Solution Architect. AI supports repetitive tasks and generates an initial draft, while the professional remains responsible for reviewing, refining, and approving the final solution.


## 4. Colonel AI – AI-Powered Conversational Ordering

The One Team presentation introduced the development journey of the **KFC Bot Agent**, an AI Agent designed to support conversational ordering across multiple communication channels.

Instead of requiring customers to leave their current conversation, download an application, create an account, and complete several ordering steps, the solution allows customers to place an order directly within their existing messaging channel.

The supported or planned channels include:

* Zalo Official Account.

* Messenger.

* WhatsApp.

* Additional communication channels that may be added in the future.

### Challenges of Conversational Ordering

Conversational ordering is not simply a question-and-answer task. The AI must accurately understand:

* Product names.

* Quantities.

* Product sizes and variants.

* Voucher rules.

* Current cart status.

* Error conditions.

* Business rules.

* Order-confirmation requirements.

A traditional chatbot may only generate a response, while an AI Agent must perform actions based on real business data.

The presented workflow included:

1. Identifying the user's goal.

2. Planning the required steps.

3. Selecting appropriate tools.

4. Performing the actions.

5. Verifying the result before confirmation.

The Agent must understand the ordering intent, search trusted business data, update the shopping cart, apply promotions, and verify the real order before confirmation.

### Transition from Monolithic Architecture to Microservices

The presentation also compared two architecture models:

#### Monolithic Architecture

* All functions are contained in one large codebase.

* Components are tightly coupled.

* Release cycles are slow.

* Individual functions are difficult to scale independently.

* Development teams are highly dependent on one another.

#### Microservices Architecture

* The system is divided into small, independent services.

* Each service manages its own logic and data.

* Services can be deployed independently.

* Faster development and innovation are supported.

* Scalability is improved.

### Multi-Channel Architecture

The solution was designed according to the principle:

**Design Once – Deploy Everywhere**

When a new communication channel is required, the team only needs to add an adapter. When a new business system needs to be connected, a connector can be added. When a new capability is required, an additional tool can be provided to the Agent.

This design enables the system to change and expand without rebuilding the entire application.

### Presented Results

According to the team's estimates:

* The average cost was approximately **USD 0.006 per order**.

* The total infrastructure cost was approximately **USD 88 per month** for 500 orders per day.

* The end-to-end latency from sending a message to receiving a response was approximately **3–5 seconds**.

* Amazon Bedrock represented the largest portion of the operating cost.

* Using AgentCore reduced the infrastructure code by approximately **60%**.

The solution demonstrated that Agentic AI can be applied to a real business process, but it must be combined with trusted data, clear business rules, and a verification step before completing a transaction.


### Knowledge Gained

#### Product-Building Mindset

* A project should begin with a real problem instead of selecting the technology first.

* The product scope must match the available time and team resources.

* A small but stable product is more valuable than an unfinished product with too many features.

* The team should define the completion criteria at the beginning.

* The demo should be treated as part of the product rather than something prepared at the last minute.

#### Agentic AI Knowledge

* An AI Agent differs from a chatbot because it can plan, use tools, perform actions, and verify results.

* An Agent should only perform actions based on trusted data.

* The system needs human-control mechanisms for important decisions.

* A good AI Agent should be proactive, explainable, and capable of recommending suitable actions.

* Agentic AI can be used in monitoring, business analysis, architecture design, and e-commerce.

#### AWS Architecture Knowledge

* Microservices support functional separation and independent deployment.

* The architecture should support the addition of new channels, systems, and tools.

* Amazon Bedrock and AgentCore can support the development of Agentic AI applications.

* CloudWatch and CloudTrail support monitoring, tracing, and auditing.

* AWS WAF, Amazon Cognito, and Secrets Manager play important roles in application security.

* AWS Lambda, DynamoDB, API Gateway, and Amazon S3 are suitable for serverless workloads.

* Region selection affects latency, integration options, and cost.

#### Cost-Management Knowledge

* Cost estimation should be performed during the architecture-design stage.

* AI-model and token costs may represent a large portion of the operating budget.

* The design should include both AWS costs and external-service costs.

* Multiple cost scenarios should be prepared for low, medium, and high usage.

* Architecture optimization should reduce cost without sacrificing performance and reliability.

#### Teamwork Skills

* Team members should have clearly assigned responsibilities.

* The team should agree on source-control and commit-management practices.

* Sensitive files such as `.env` must never be uploaded to a public source-code repository.

* Members should communicate frequently to avoid duplicated or missing tasks.

* A team with diverse skills is often more effective than a team whose members perform the same role.

* Time should be allocated for rehearsing the presentation and demo.


### Application to Study and Work

* Apply problem identification and scope limitation before starting an AWS project.

* Develop products using an MVP approach and complete the primary workflow before adding advanced functions.

* Divide systems into independent components to simplify development, testing, and scaling.

* Use AWS Architecture Icons and Draw.io to present architectures clearly.

* Create assumption tables and cost estimates during architecture design.

* Use Amazon CloudWatch to monitor logs, metrics, and system errors.

* Apply AWS WAF, Amazon Cognito, and Secrets Manager to strengthen security.

* Study Amazon Bedrock and AgentCore to develop Agentic AI capabilities.

* Design AI Agents according to the process of understanding goals, planning, using tools, acting, and verifying.

* Keep humans in control of important actions and final decisions.

* Prepare accounts, tools, starter code, and a demo script before joining a Hackathon.

* Manage source code carefully and never commit access keys, secret keys, or `.env` files.

* Assign members to development, architecture, interface design, testing, and presentation responsibilities.


### Experience During the Event

Participating in the event on July 26, 2026, was a valuable experience that introduced me to different approaches to building products with AI and AWS.

#### Learning from Practical Projects

The four presentations did not only introduce ideas. They also explained the problems, solutions, architectures, costs, challenges, and demonstration results. Through these presentations, I better understood how an initial idea can be developed into a working product.

The S.H.E.P.H.E.R.D project demonstrated how Computer Vision, object tracking, and Agentic AI can be combined to solve crowd-monitoring problems.

SignalScout showed how AI can support businesses in collecting evidence, connecting data, and detecting strategic changes.

The Solution Architect Professional AI Native App demonstrated how AI can assist with requirement analysis, architecture generation, diagram creation, Infrastructure as Code, and cost estimation.

Colonel AI demonstrated how an AI Agent can perform a practical business workflow across multiple communication channels.

#### Understanding Product-Development Challenges

The teams openly shared challenges such as limited AI experience, first-time use of AWS, restricted development time, source-code errors, latency, cost, and the pressure of preparing a working demo.

These experiences helped me understand that errors and changes in direction are normal parts of product development. The important point is to identify the correct priorities and complete a functional primary workflow.

#### Changing My Perspective on Hackathons

Previously, I mainly considered a Hackathon to be a programming competition. After attending the event, I understood that a Hackathon is also an opportunity to:

* Test problem-solving abilities.

* Work under limited time conditions.

* Learn new technologies quickly.

* Communicate and divide tasks within a team.

* Present ideas to other people.

* Connect with people who share similar technology interests.

* Discover one's own practical capabilities.

#### Personal Lessons

The most important lesson I gained was that I do not need to wait until I have complete knowledge before starting. Actively participating, experimenting, and completing a small product can provide more practical experience than studying theory alone.

I also learned that architecture, cost, security, and demonstration requirements should be considered from the beginning. A good technical solution should not only function correctly but should also be explainable, scalable, and suitable for real-world requirements.


### Event Images

![The Hackathon Journey presentation by Team 3KA](/images/event-participated/event3.1.png)

![SignalScout presentation](/images/event-participated/event3.2.png)

![Solution Architect Professional AI Native App presentation](/images/event-participated/event3.3.png)


> Overall, the event helped me better understand the process of building Agentic AI products on AWS, from problem identification, architecture design, MVP development, and testing to cost estimation, product presentation, and post-Hackathon reflection.