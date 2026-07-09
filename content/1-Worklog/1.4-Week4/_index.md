---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives:

* Set up VPC Peering connections.
* Configure AWS Transit Gateway.

### Tasks Completed This Week:

| Day | Tasks | Start Date | Completion Date | Reference |
| --- | ----- | ---------- | --------------- | --------- |
| Fri | - Launch a CloudFormation stack.<br>- Create a Security Group.<br>- Launch EC2 instances. | 08/05/2026 | 08/05/2026 | <https://000019.awsstudygroup.com/2-prerequiste/> |
| Sat | - Update Network ACLs.<br>- Configure VPC Peering.<br>- Configure DNS resolution between peered VPCs. | 09/05/2026 | 09/05/2026 | <https://000019.awsstudygroup.com/3-updatenetworkacl/> |
| Mon | - Set up AWS Transit Gateway.<br>- Create a Transit Gateway. | 11/05/2026 | 11/05/2026 | <https://000020.awsstudygroup.com/1-introduce/> |
| Tue | - Create Transit Gateway Attachments.<br>- Create a Transit Gateway Route Table. | 12/05/2026 | 12/05/2026 | <https://000020.awsstudygroup.com/4-transigatewayattachments/> |
| Wed | - Add Transit Gateway routes to the VPC Route Tables. | 13/05/2026 | 13/05/2026 | <https://000020.awsstudygroup.com/6-result/> |

### Week 4 Achievements:

* Learned how to configure **VPC Peering** and **AWS Transit Gateway**.
* Successfully:
  * Updated Route Tables, Network ACLs, and DNS settings to enable communication between VPCs.
  * Created and configured an AWS Transit Gateway.
  * Created Transit Gateway Attachments and a Transit Gateway Route Table.
  * Added Transit Gateway routes to VPC Route Tables.
  * Verified connectivity between Amazon EC2 instances located in different VPCs.
* Gained a clear understanding of the differences between **VPC Peering** and **AWS Transit Gateway**, including their use cases and network architecture.

### Screenshots:

{{< figure src="/images/1-Worklog/1.4-Week4/createVPC.png" title="Create a VPC" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createHGVPC.png" title="Create a Security Group for HG VPC" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createEC2.png" title="Launch an EC2 Instance" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/updateACL.png" title="Update Network ACLs" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/connectVPC.png" title="Configure VPC Peering" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createKeypair.png" title="Create an EC2 Key Pair" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createTransitGateway.png" title="Create an AWS Transit Gateway" >}}
{{< figure src="/images/1-Worklog/1.4-Week4/createGatewayRoute.png" title="Create a Transit Gateway Route Table" >}}