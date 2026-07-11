---
title: "Week 10 Worklog"
date: 2026-06-15
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

{{% notice warning %}}
Note: The following information is for reference purposes only. Please do not copy verbatim for your own report.
{{% /notice %}}


### Week 10 Objectives:

* Learn the basic concepts of hybrid DNS.
* Understand Route 53 Resolver inbound endpoints, outbound endpoints, and resolver rules.
* Practice reviewing a simple DNS connection between AWS and a simulated on-premises environment.


### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Learn the purpose of Amazon Route 53 and Route 53 Resolver <br> - Understand the basic idea of hybrid DNS <br> - Review inbound endpoints, outbound endpoints, and resolver rules | 06/15/2026 | 06/15/2026 | <https://000010.awsstudygroup.com/> |
| 3 | - Review the workshop architecture <br> - Create or review the required key pair and Security Group <br> - Deploy the sample VPC resources using a CloudFormation template | 06/16/2026 | 06/16/2026 | <https://000010.awsstudygroup.com/2-preparation/> |
| 4 | - Review the AWS Managed Microsoft AD environment used to simulate an on-premises DNS system <br> - Check the VPC, subnet, and DNS settings <br> - Verify that the required resources are available | 06/17/2026 | 06/17/2026 | <https://000010.awsstudygroup.com/4-microsoft-ad-deployment/> |
| 5 | - Create or review a Route 53 Resolver outbound endpoint <br> - Create a simple resolver forwarding rule <br> - Associate the rule with the selected VPC | 06/18/2026 | 06/18/2026 | <https://000010.awsstudygroup.com/5-setuphyriddns/5.1-createoe/> <br> <https://000010.awsstudygroup.com/5-setuphyriddns/5.2-createroute53/> |
| 6 | - Create or review a Route 53 Resolver inbound endpoint <br> - Test DNS name resolution between the AWS environment and the simulated on-premises environment <br> - Record the test result <br> - Delete temporary workshop resources after practice | 06/19/2026 | 06/19/2026 | <https://000010.awsstudygroup.com/5-setuphyriddns/5.3-createie/> <br> <https://000010.awsstudygroup.com/5-setuphyriddns/5.4-test-results/> <br> <https://000010.awsstudygroup.com/6-clean-up-resources/> |


### Week 10 Achievements:

* Understood the basic purpose of hybrid DNS.

* Learned the basic meaning of:
  * Route 53 Resolver
  * Inbound endpoint
  * Outbound endpoint
  * Resolver rule
  * DNS forwarding

* Reviewed the architecture used to connect AWS DNS with a simulated on-premises DNS environment.

* Used a CloudFormation template to create or review the required network resources.

* Reviewed the VPC, subnet, Security Group, and DNS settings.

* Learned how an outbound endpoint forwards DNS queries to another DNS system.

* Created or reviewed a simple resolver forwarding rule.

* Associated the resolver rule with a VPC.

* Learned how an inbound endpoint receives DNS queries from an external DNS system.

* Tested basic DNS name resolution between two environments.

* Recorded the DNS test result.

* Deleted temporary workshop resources after completing the practice.