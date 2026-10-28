# ☁️ AWS Complete Learning Journey — Beginner to DevOps Engineer

Welcome to my independent **AWS learning and interview preparation repository**. This is a hands-on, Linux-focused guide from cloud fundamentals to production DevOps architecture.

> **Goal:** Learn → Practice → Troubleshoot → Document → Revise → Build.

## 🎯 Learning Outcomes

- Understand cloud computing, AWS, Azure, Google Cloud and hybrid environments.
- Create and secure an AWS account, control costs and understand the console.
- Deploy Linux EC2 web servers and manage AMIs, EBS, snapshots, networks and permissions.
- Build highly available architectures using load balancers, Auto Scaling, DNS and CDN.
- Monitor, audit and administer AWS with CloudWatch, CloudTrail and Systems Manager.
- Automate infrastructure and delivery with CLI, Terraform, CloudFormation, containers and CI/CD.
- Explore serverless, AI/Bedrock and advanced AWS design.
- Prepare for interviews with hands-on examples and scenario answers.

## 📚 Complete Learning Index

| No. | Topic | What I Will Learn |
|---|---|---|
| 01 | [Cloud Computing Introduction](01-Cloud-Foundations/README.md) | Cloud computing delivers on-demand compute, storage, databases, and networking over the internet. |
| 02 | [AWS vs Azure vs Google Cloud and Hybrid Cloud](02-Cloud-Providers/README.md) | Understand public, private, hybrid and multicloud patterns and major cloud platforms. |
| 03 | [AWS Account Creation, Free Tier and Billing](03-AWS-Account-and-Billing/README.md) | Create and protect a learning account and understand billing before deploying anything. |
| 04 | [AWS Console Dashboard and AWS CLI](04-AWS-Console-and-CLI/README.md) | Learn navigation, Region selection, service search, account menu, CloudShell and CLI profiles. |
| 05 | [AWS Regions, Availability Zones and Edge Locations](05-Regions-and-AZs/README.md) | Understand AWS infrastructure geography and resilient placement. |
| 06 | [IAM, Roles, Policies and Security Fundamentals](06-IAM-and-Security/README.md) | Control who can access AWS resources and what they may do. |
| 07 | [EC2 Fundamentals and Instance Launch](07-EC2-Basics/README.md) | Learn virtual servers, instance lifecycle, AMIs, networking and key pairs. |
| 08 | [Create an Ubuntu Web Server on EC2](08-EC2-Web-Server/README.md) | Install and publish a basic Nginx website on an EC2 Linux instance. |
| 09 | [EC2 Instance Types, Stop, Start, Resize and Termination Protection](09-EC2-Operations/README.md) | Safely manage lifecycle and instance sizing. |
| 10 | [AMIs, Golden Images and Recovery](10-AMI-and-Backups/README.md) | Create reusable server images and understand backup consistency. |
| 11 | [EBS Volumes, Snapshots and Storage](11-EBS-and-Snapshots/README.md) | Understand EC2 block storage and data protection. |
| 12 | [VPC, Subnets, Routing and Security Groups](12-VPC-and-Networking/README.md) | Build a network for AWS applications. |
| 13 | [Amazon S3 Object Storage](13-S3/README.md) | Store and protect files and static website assets. |
| 14 | [Elastic Load Balancing: ALB, NLB and GWLB](14-ELB/README.md) | Distribute traffic and add health checks. |
| 15 | [EC2 Auto Scaling](15-Auto-Scaling/README.md) | Maintain desired capacity automatically. |
| 16 | [Route 53 and DNS](16-Route53/README.md) | Understand domain resolution and AWS DNS routing. |
| 17 | [Amazon CloudFront CDN](17-CloudFront/README.md) | Deliver content through edge caching. |
| 18 | [RDS, Aurora and DynamoDB](18-RDS-and-Databases/README.md) | Choose managed SQL or NoSQL data services. |
| 19 | [CloudWatch Metrics, Logs and Alarms](19-CloudWatch/README.md) | Observe application and infrastructure health. |
| 20 | [AWS CloudTrail Auditing](20-CloudTrail/README.md) | Audit API calls and account activity. |
| 21 | [AWS Systems Manager and Session Manager](21-Systems-Manager/README.md) | Manage EC2 without opening inbound SSH ports. |
| 22 | [AWS Lambda, API Gateway and EventBridge](22-Lambda-and-Serverless/README.md) | Run event-driven code without provisioning a server. |
| 23 | [KMS, Secrets Manager and Parameter Store](23-KMS-and-Secrets/README.md) | Protect keys, passwords and configuration. |
| 24 | [AWS CloudFormation](24-CloudFormation/README.md) | Describe AWS infrastructure declaratively. |
| 25 | [Terraform for AWS](25-Terraform-on-AWS/README.md) | Provision infrastructure repeatably using Terraform. |
| 26 | [ECR, ECS, Fargate and EKS](26-Containers-ECR-ECS-EKS/README.md) | Run and deploy containers on AWS. |
| 27 | [CI/CD with CodeBuild, CodeDeploy and CodePipeline](27-CICD/README.md) | Automate build, test and deployment workflows. |
| 28 | [AWS Backup, High Availability and Disaster Recovery](28-Backup-DR/README.md) | Plan recovery and resilient operations. |
| 29 | [Cost Optimization and AWS Well-Architected](29-Cost-and-Well-Architected/README.md) | Design reliable, secure, efficient, cost-aware systems. |
| 30 | [Amazon Bedrock and Generative AI Basics](30-Bedrock-and-AI/README.md) | Understand managed foundation model access and AI security. |
| 31 | [Advanced Networking: VPN, Direct Connect and Endpoints](31-Network-Advanced/README.md) | Connect cloud networks securely and diagnose connectivity. |
| 32 | [AWS Troubleshooting Playbook](32-Troubleshooting/README.md) | Diagnose EC2, IAM, S3, VPC, DNS, SSM and deployment failures. |
| 33 | [AWS Interview Questions and Scenario Practice](33-Interview-Preparation/README.md) | Revise AWS core concepts with real troubleshooting scenarios. |

## 🗺️ Suggested Learning Order

**Phase 1 — Foundation:** Chapters 01–06 (cloud, account, console, Regions, IAM).

**Phase 2 — Linux on AWS:** Chapters 07–13 (EC2, Nginx web server, operations, AMI, EBS, VPC, S3).

**Phase 3 — Production AWS:** Chapters 14–20 (load balancing, scaling, DNS, CDN, databases, monitoring and auditing).

**Phase 4 — Operations and DevOps:** Chapters 21–29 (Session Manager, Lambda, security, IaC, containers, CI/CD, backups and cost).

**Phase 5 — Advanced + interviews:** Chapters 30–33 and the projects folder.

## 🔐 Account Setup and Cost Safety (Read First)

1. Go to [AWS Free Tier](https://aws.amazon.com/free/) and follow the current sign-up process. AWS account plan and service access differ; do not assume every service is free.
2. Verify contact/payment details and secure the root user with MFA.
3. Create a separate day-to-day administrative identity (prefer IAM Identity Center when appropriate).
4. Set a low [AWS Budget](https://console.aws.amazon.com/billing/home#/budgets) and email notifications. Budgets are alerts, **not an automatic hard spending cap**.
5. Choose a Region deliberately; check resource availability, data residency and prices.
6. Use tags like `Project=aws-learning`, `Owner=student`, `Environment=lab`.
7. **Always clean up:** EC2, EBS volumes/snapshots, load balancers, NAT gateways, public IPv4, RDS, EKS, CloudWatch logs and other resources can cost money.
8. Never commit passwords, private keys, tokens, state files containing secrets or access keys.

Current AWS plan details: [AWS Free Tier documentation](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/free-tier.html).

## 🧪 Daily Practice Method

1. Read one topic's definition and concepts.
2. Explain its use case in your own words.
3. Follow the console lab, then reproduce relevant steps using AWS CLI.
4. Capture commands, expected results and screenshots without secrets.
5. Troubleshoot one deliberately introduced safe error.
6. Answer the interview questions aloud.
7. Remove resources and verify costs.
8. Commit revised notes to GitHub.

## 📝 Standard Notes Template

Every chapter includes: Introduction → Concepts → Hands-on lab → Commands → Troubleshooting → Interview Q&A → Scenario → Revision checklist → Official resources.

## 🛠️ Hands-on Projects

See [Projects](34-Hands-on-Projects/README.md) for step-by-step guided mini projects and architecture exercises.

## 📅 12-Week Study Plan

| Week | Focus | Deliverable |
|---|---|---|
| 1 | Cloud concepts, account, dashboard, Regions, IAM | Secure account + billing budget |
| 2 | EC2, SSH/Session Manager, Ubuntu web server | Working Nginx website |
| 3 | EC2 operations, AMI, EBS and snapshots | Image and restore lab |
| 4 | VPC, subnets, routing, SG, S3 | Architecture diagram + private bucket |
| 5 | ALB, Auto Scaling, Route 53, CloudFront | Resilient web architecture design |
| 6 | RDS, DynamoDB, CloudWatch, CloudTrail | Monitoring and auditing notes |
| 7 | Systems Manager, KMS, Secrets Manager | Secure operations lab |
| 8 | Lambda, API Gateway, EventBridge | Serverless hello world |
| 9 | CloudFormation and Terraform | Repeatable infrastructure plan |
| 10 | ECR, ECS, EKS, CI/CD | Container pipeline design |
| 11 | Backup, DR, cost, troubleshooting | Incident response runbook |
| 12 | Bedrock, architecture, interview practice | Capstone design and mock interview |

## 📖 Interview Preparation Routine

For every chapter: **What is it? Why use it? How configure it? How secure it? How monitor it? What can fail? What does it cost?** Practice explaining real-world examples.

## 🔗 Official References

- [AWS Documentation](https://docs.aws.amazon.com/)
- [AWS Skill Builder](https://skillbuilder.aws/)
- [AWS Architecture Center](https://aws.amazon.com/architecture/)
- [AWS Pricing Calculator](https://calculator.aws/)
- [AWS Well-Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)

⭐ **Learning every day. Practicing every service. Building AWS and DevOps skills step by step.**
