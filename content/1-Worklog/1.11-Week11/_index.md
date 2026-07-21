---
title: "Week 11 Worklog"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Week 11 Objectives:

* Learn how to build and secure APIs in a serverless architecture on AWS.

* Practice user authentication with Amazon Cognito and control access to APIs.

* Become familiar with AWS WAF, AWS Lambda, and S3 Presigned URLs for secure file uploads.


### Tasks to Be Completed This Week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Learn about the secure file upload process for Amazon S3.<br>- Study how API Gateway, AWS Lambda, and Amazon S3 work together in a serverless architecture.<br>- Become familiar with using tokens to verify user requests. | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/><br><https://000078.awsstudygroup.com/vi/> |
| 3 | - Practice creating an Amazon Cognito User Pool and App Client.<br>- Configure sign-in methods, password policies, and account verification.<br>- Learn how Cognito issues tokens after a user successfully signs in. | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/cognito/><br><https://000081.awsstudygroup.com/vi/2-create-user-pool/> |
| 4 | - Create routes and HTTP methods in Amazon API Gateway.<br>- Integrate API Gateway with AWS Lambda to process requests.<br>- Configure a Cognito Authorizer to restrict API access to authenticated users. | 01/07/2026 | 01/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/apigateway/><br><https://000079.awsstudygroup.com/vi/1-introduction/><br><https://000117.awsstudygroup.com/6-identity/6.8-authorizer/> |
| 5 | - Learn how AWS WAF protects websites and APIs from invalid or malicious requests.<br>- Become familiar with Web ACLs, AWS Managed Rules, and request rate limiting.<br>- Practice associating a Web ACL with the resource that needs protection. | 02/07/2026 | 02/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/waf/><br><https://000026.awsstudygroup.com/vi/3-useawswaf/> |
| 6 | - Build a Lambda function that generates an S3 Presigned URL with a limited validity period.<br>- Review the IAM permissions required for Lambda to access Amazon S3.<br>- Test the process of calling the API and uploading files to S3 without granting public write access to the Bucket. | 03/07/2026 | 03/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/lambda-handler/><br><https://000078.awsstudygroup.com/vi/><br><https://000033.awsstudygroup.com/vi/6-demo/> |


### Week 11 Achievements:

* Completed the configuration of an Amazon Cognito User Pool and App Client.

* Created API Gateway routes integrated with AWS Lambda.

* Applied a Cognito Authorizer to control access to the API.

* Configured AWS WAF to improve API protection against unusual requests.

* Generated an S3 Presigned URL for secure file uploads within a limited period.

* Successfully tested the authentication, API request, and Amazon S3 upload workflow.