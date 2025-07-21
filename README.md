# SAM AegisAI – S3 Bucket Remediation System

## Overview

**SAM AegisAI** is a lightweight automation tool designed to detect and remediate public S3 bucket access violations using AWS Lambda, CloudWatch Events, AWS Config, and SNS. This proof-of-concept helps small businesses or startups implement DevSecOps-style compliance without breaking the bank.

---

## Features

- Detects public access to Amazon S3 buckets  
- Simulates a security threat when a bucket is made public  
- Automatically revokes public access using a Lambda function  
- Sends real-time email alerts via Amazon SNS  
- Logs actions for auditing and security review  

---

## Architecture

![SAM AegisAI Architecture](assets/sam-architecture.png)

This diagram illustrates the event-driven flow:
1. **AWS Config** or **CloudWatch Events** detect misconfigurations  
2. Triggers a **Lambda** function  
3. Lambda remediates the issue by blocking public access  
4. Sends an **SNS alert** for real-time visibility  

---

## Built With

- AWS Lambda  
- Amazon S3  
- AWS Config  
- AWS CloudTrail  
- Amazon SNS  
- Amazon CloudWatch Events  
- Amazon GuardDuty  
- Python (boto3)  
- GitHub + GitHub Desktop  

---

## Developed By

**Aija Murry** – Cloud & Cybersecurity Professional  
AWS Solutions Architect | Security+ Certified  
Atlanta, GA  

---

## Future Plans

- Add Slack and SMS alerting via SNS  
- Expand remediation to EC2 Security Groups  
- Integrate with AWS Security Hub  
- Build a React/Tailwind web dashboard  
- Dockerize for flexible deployments  

---

## Deployment (Quick Start)

1. **Clone the repo**  
   ```bash
   git clone https://github.com/yourusername/sam-aegisai-remediation1.git
   cd sam-aegisai-remediation1

## Set up IAM role and policy 

aws iam create-role --role-name sam-remediation-role \
  --assume-role-policy-document file://iam/sam-remediation-trust-policy.json

aws iam put-role-policy --role-name sam-remediation-role \
  --policy-name sam-remediation-policy \
  --policy-document file://iam/sam-remediation-policy.json


## Deploy the stack using AWS SAM

sam build
sam deploy --guided


## Feedback or Questions? 

Feel free to connect with me on LinkedIn! 




