---
title: "Week 6 Worklog"
date: 2026-05-18
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

{{% notice warning %}}
Note: The following information is for reference purposes only. Please do not copy verbatim for your own report.
{{% /notice %}}


### Week 6 Objectives:

* Learn the basic concepts of Elastic Load Balancing and EC2 Auto Scaling.
* Understand Launch Templates, Target Groups, and Application Load Balancers.
* Practice creating a simple scalable web server environment.


### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Learn the purpose of Elastic Load Balancing and EC2 Auto Scaling <br> - Understand the basic roles of a Load Balancer, Target Group, Launch Template, and Auto Scaling Group | 05/18/2026 | 05/18/2026 | <https://000006.awsstudygroup.com/> |
| 3 | - Create a Launch Template for a small Amazon Linux EC2 instance <br> - Add a simple user data script to install a web server <br> - Select the required Security Group and key pair | 05/19/2026 | 05/19/2026 | <https://000006.awsstudygroup.com/2-create-launch-template/> |
| 4 | - Create a Target Group for EC2 instances <br> - Configure a basic health check <br> - Create an Application Load Balancer in public subnets <br> - Connect the Load Balancer listener to the Target Group | 05/20/2026 | 05/20/2026 | <https://000006.awsstudygroup.com/3-create-target-group/> <br> <https://000006.awsstudygroup.com/4-create-load-balancer/> |
| 5 | - Create an Auto Scaling Group using the Launch Template <br> - Set minimum, desired, and maximum instance capacity <br> - Attach the Auto Scaling Group to the Target Group <br> - Check the health status of the EC2 instances | 05/21/2026 | 05/21/2026 | <https://000006.awsstudygroup.com/5-create-auto-scaling-group/> |
| 6 | - Open the Load Balancer DNS name and test the web page <br> - Review basic CloudWatch metrics for the Auto Scaling Group <br> - Change the desired capacity and observe the number of instances <br> - Delete the Auto Scaling Group, Load Balancer, Target Group, and Launch Template after practice | 05/22/2026 | 05/22/2026 | <https://000006.awsstudygroup.com/6-test-auto-scaling/> <br> <https://000006.awsstudygroup.com/7-clean-up/> |


### Week 6 Achievements:

* Understood the basic purpose of Elastic Load Balancing and EC2 Auto Scaling.

* Learned the basic meaning of:
  * Launch Template
  * Target Group
  * Health Check
  * Application Load Balancer
  * Auto Scaling Group

* Created a Launch Template for an Amazon Linux EC2 instance.

* Used a simple user data script to install a web server.

* Created a Target Group and configured a basic health check.

* Created an Application Load Balancer and connected it to the Target Group.

* Created an Auto Scaling Group with minimum, desired, and maximum capacity settings.

* Checked the health status of EC2 instances in the Target Group.

* Accessed the test web page through the Load Balancer DNS name.

* Changed the desired capacity and observed the number of EC2 instances.

* Deleted temporary scaling and load-balancing resources after completing the practice.