# SAM AegisAI – S3 Bucket Remediation System

## 🛡️ SAM AegisAI - Auto Remediation Architecture

This project uses AWS Config Rules, EventBridge, and Lambda to detect and automatically remediate public S3 bucket access. Alerts are sent via Amazon SNS.

![SAM AegisAI Architecture](https://i.imgur.com/VFkPgMz.png)


**SAM AegisAI** is a lightweight automation tool designed to simulate and remediate public S3 bucket access violations using AWS Lambda, CloudWatch Events, AWS Config, and SNS. This proof-of-concept is ideal for small businesses or startups looking to implement DevSecOps-style cloud compliance on a budget.

---

## Features

- Detects public access to Amazon S3 buckets
- Simulates a security threat when a bucket is made public
- Automatically revokes public access using a Lambda function
- Sends real-time email alerts via Amazon SNS
- Logs actions for auditing and security review

---

## Built With

- AWS Lambda  
- Amazon S3  
- AWS Config  
- CloudTrail  
- Amazon SNS  
- CloudWatch Events  
- GuardDuty  
- Python (boto3)  
- GitHub + GitHub Desktop  

---

##  Developed By

**Aija Murry** – Cloud & Cybersecurity Professional  
AWS Solutions Architect | Security+ Certified  
Atlanta, GA

---

## Future Plans

- Add support for Slack or SMS alerting via SNS  
- Expand Lambda functions to cover EC2 security group misconfigurations  
- Build a lightweight web dashboard for monitoring actions  
- Dockerize for container-based deployments



