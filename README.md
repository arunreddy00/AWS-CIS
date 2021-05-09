# AWS-CIS

Edit accordingly
AWS-CIS

AWS Security Enabling

### Governance-control:
-----------------------
The Cloudformation template implements this by creating AWS Config rules, Amazon CloudWatch alarms, and CloudWatch Events rules in your AWS account, as well as the supporting logging services: AWS CloudTrail, AWS Config, AWS CloudWatch Logs and an SNS topic for email notifications.
Pre-Requisites

•	Create S3 bucket for logs, note bucket name

•	Edit Governance-control.yaml with valid email address for notification line 165

•	Edit KMS key for encryption line  78

•	Edit S3 bucket in line 7,9

•	Deploy Governance-control.yaml from Cloud formation


### AWS Security-Hub:
---------------------------------
A Cloudformation template to enable AWS Security Hub, Configure findings notifications using a Cloudwatch Event rule to match on Security Hub findings and send notifications to an SNS topic

•	Edit Security-hub.yaml with valid email address for notification line 11

•	Deploy Security-hub.yaml from Cloud formation

### AWS Guard-Duty:
----------------------------------
A Cloudformation template to enable AWS Guard Duty, Continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads. Email Notifications enable notifications for GuardDuty and Security Hub using CloudWatch Event Rules and SNS.

•	Edit Guard-Duty.yaml with valid email address for notifications in line 13

•	Deploy Guard-Duty.yaml from Cloud formation

