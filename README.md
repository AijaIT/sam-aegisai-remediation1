# SAM AegisAI – S3 Bucket Remediation System

SAM AegisAI is a lightweight automation tool designed to simulate and remediate public S3 bucket access violations using AWS Lambda, CloudWatch Events, and Python. This proof-of-concept is ideal for small businesses or startups looking to implement DevSecOps-style cloud compliance on a budget.

## Features

- Detects public access to Amazon S3 buckets  
- Simulates a security threat when a bucket is made public  
- Automatically revokes public access using a Lambda function  
- Logs actions for auditing and security review  

## Built With

- AWS Lambda  
- Amazon S3  
- CloudWatch Events  
- AWS Config   
- GuardDuty  
- Python (boto3)  
- GitHub + GitHub Desktop  

## Developed By

Aija Murry – Cloud & Cybersecurity Professional  
AWS Solutions Architect | Security+ Certified  
Atlanta, GA  

## Future Plans

- Add SNS notifications  
- Integrate with GuardDuty and AWS Config  
- Dockerize for container-based deployments  

