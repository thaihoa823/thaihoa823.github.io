---
title: "Week 12 Worklog"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---




### Week 12 Objectives:

* Complete an asynchronous image-processing workflow based on an event-driven architecture on AWS.

* Integrate Amazon S3, AWS Lambda, DynamoDB Streams, and Amazon Rekognition to automatically process, analyze, and store image information.

* Test the entire workflow, monitor execution logs, and clean up the practice resources.


### Tasks to Be Completed This Week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Create two separate Amazon S3 Buckets for storing original and processed images.<br>- Configure an Object Created event to automatically invoke AWS Lambda when a new image is uploaded.<br>- Configure the IAM Role and required permissions for the Lambda function. | 06/07/2026 | 06/07/2026 | <https://000078.awsstudygroup.com/vi/><br><https://000078.awsstudygroup.com/vi/2-resize-image-function/> |
| 3 | - Develop a Lambda function to read images from Amazon S3, resize them, and optimize their file sizes.<br>- Store the processed images in the destination Bucket.<br>- Monitor the execution process and troubleshoot errors through Amazon CloudWatch Logs. | 07/07/2026 | 07/07/2026 | <https://000078.awsstudygroup.com/vi/2-resize-image-function/><br><https://000008.awsstudygroup.com/vi/> |
| 4 | - Create an Amazon DynamoDB table to store image metadata.<br>- Define the Partition Key and the required attributes for each record.<br>- Enable DynamoDB Streams and connect the Stream to a Lambda function to process data changes. | 08/07/2026 | 08/07/2026 | <https://000078.awsstudygroup.com/vi/><br><https://000039.awsstudygroup.com/3-ladv/3.9/> |
| 5 | - Develop a Lambda function that receives events from DynamoDB Streams.<br>- Integrate Amazon Rekognition to detect objects, assign labels, and moderate image content.<br>- Update the analysis results in the DynamoDB table. | 09/07/2026 | 09/07/2026 | <https://000056.awsstudygroup.com/vi/2-adding-object-recognition-using-aws-rekognition/><br><https://000039.awsstudygroup.com/3-ladv/3.9/> |
| 6 | - Test the complete workflow, from image upload and processing to Rekognition analysis and metadata updates.<br>- Verify the images in the S3 Buckets, the records in DynamoDB, and the execution logs in CloudWatch.<br>- Organize the source code, complete the documentation, and remove unused resources. | 10/07/2026 | 10/07/2026 | <https://000078.awsstudygroup.com/vi/4-cleanup/><br><https://000008.awsstudygroup.com/vi/><br><https://000056.awsstudygroup.com/vi/> |


### Week 12 Achievements:

* Completed an asynchronous image-processing workflow based on an event-driven architecture.

* Successfully connected Amazon S3 with AWS Lambda to automatically resize and optimize images.

* Used DynamoDB Streams to trigger the data-analysis process whenever image metadata changed.

* Integrated Amazon Rekognition to detect objects, assign labels, and moderate image content.

* Successfully verified the entire processing workflow through Amazon CloudWatch Logs.

* Packaged the project and successfully pushed the complete source-code repository, including a detailed installation guide in the `README.md` file, to a personal GitHub repository.