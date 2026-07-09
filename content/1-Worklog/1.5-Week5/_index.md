---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---


### Week 5 Objectives:

* Deploy AWS Backup for the system.
* Learn how to restore data from backups and automate the backup and recovery process.
* Configure notifications to monitor backup and restore operations.

### Tasks Completed This Week:

| Day | Tasks | Start Date | Completion Date | Reference |
| --- | ----- | ---------- | --------------- | --------- |
| Fri | - Create an Amazon S3 bucket.<br>- Deploy the required infrastructure. | 15/05/2026 | 15/05/2026 | <https://000013.awsstudygroup.com/2-prerequiste/2.1-creates3bucket/> |
| Sat | - Create an AWS Backup Plan. | 16/05/2026 | 16/05/2026 | <https://000013.awsstudygroup.com/3-createbackupplan/> |
| Mon | - Configure backup notifications. | 18/05/2026 | 18/05/2026 | <https://000013.awsstudygroup.com/4-enablenoti/> |
| Tue | - Test the restore process. | 19/05/2026 | 19/05/2026 | <https://000013.awsstudygroup.com/5-testrestore/> |
| Wed | - Use AWS File Gateway. | 20/05/2026 | 20/05/2026 | <https://000024.awsstudygroup.com/2-prerequiste/> |
| Thu | - Use AWS Storage Gateway. | 21/05/2026 | 21/05/2026 | <https://000024.awsstudygroup.com/2-useawsstoragegw/> |

### Week 5 Achievements:

* Successfully created an **Amazon S3 bucket** to store system backup data.
* Deployed the **AWS Backup** infrastructure and configured a **Backup Vault**.
* Configured **Amazon SNS** notifications to monitor backup and restore operations.
* Gained hands-on experience with **AWS Storage Gateway** and **File Gateway** for integrating on-premises storage with AWS.
* Understood the automated workflow for backup, restore, and system monitoring on AWS.

### Screenshots:

{{< figure src="/images/1-Worklog/1.5-Week5/createS3Bucket.png" title="Create an Amazon S3 Bucket" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createFolder.png" title="Create a Folder" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/uploadFile.png" title="Upload a File" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/permissions.png" title="Block Public Access" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/editPolicy.png" title="Edit the Bucket Policy" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createBackUp.png" title="Create a Backup Plan" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/testRestore.png" title="Test Data Restoration" >}}
{{< figure src="/images/1-Worklog/1.5-Week5/createStorageGateway.png" title="Create an AWS Storage Gateway" >}}