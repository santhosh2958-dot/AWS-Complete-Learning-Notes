# 12. VPC, Subnets, Routing and Security Groups

[⬅ Back to AWS Learning Home](../README.md)

## 1. Introduction

Build a network for AWS applications.

**Why this matters for Linux/DevOps:** Understanding this topic helps you build, secure, automate, monitor, or troubleshoot production infrastructure.

## 2. Concepts to Understand

- **VPC CIDR** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **public/private subnets** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **route tables** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **internet gateway** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **NAT gateway** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **NACL vs SG** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **DNS** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **VPC endpoints** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **peering** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **transit gateway** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **VPN** — research the definition, purpose, configuration choices, limitations, and operational impact.

## 3. Hands-on Lab (Step by Step)

**Prerequisites:** AWS account with appropriate permissions, a selected Region, an approved budget, and a disposable test environment.

1. Read the concepts above and identify the AWS service in the console.
2. Check service pricing and whether your account plan permits this lab.
3. Draw a /16 VPC with two /24 public subnets and two /24 private subnets across AZs; identify internet gateway and NAT route; create a minimal VPC only if budget permits; avoid NAT gateway for cost-sensitive practice.
4. Record the AWS resource IDs, Region, screenshots (without secrets), and what you observed.
5. Validate the expected result and record any errors and fixes.
6. **Cleanup:** Delete or stop all resources created for the lab, including dependent volumes, snapshots, IPs, log groups and other billable resources where applicable. Confirm deletion and inspect Billing.

## 4. Commands / CLI Practice

Replace placeholder values with your own test resources. Do not paste credentials into Git.

```bash
aws ec2 describe-vpcs --output table
aws ec2 describe-subnets --output table
aws ec2 describe-route-tables --output table
```

**Verify:** Observe command output, confirm correct Region/account, and cross-check the AWS console. Some commands require permissions, installed software, or existing resources.

## 5. Common Troubleshooting

| Symptom | What to check |
|---|---|
| AccessDenied | Caller identity, identity/resource policies, role, explicit denies, organization restrictions |
| Resource not found | Region, account, resource ID, service availability |
| Operation blocked | Account plan, service quota, prerequisites, resource state |
| Unexpected charges | Running resources, data transfer, storage, public IPs, logs, retained backups |

## 6. Interview Questions and Answers

**Q1. SG vs NACL?**

**Answer:** Security groups are stateful instance/ENI-level controls

**Q2. What makes a subnet public?**

**Answer:** Its associated route table has a route to an internet gateway

## 7. Scenario Question

**Q. You are asked to implement vpc, subnets, routing and security groups for a production team. What is your approach?**

**Answer:** Clarify requirements and cost constraints; choose the correct Region and architecture; apply least-privilege IAM and encryption; test in a non-production environment; monitor outcomes; document rollback and cleanup.

## 8. Revision Checklist

- [ ] I can explain this service in simple words.
- [ ] I understand the major concepts and trade-offs.
- [ ] I have completed a safe lab or architecture exercise.
- [ ] I can explain the commands and expected output.
- [ ] I know common troubleshooting steps.
- [ ] I can answer the interview questions without notes.

## 9. Official Documentation

- [AWS Documentation](https://docs.aws.amazon.com/)
- [AWS Pricing](https://aws.amazon.com/pricing/)
- [AWS Well-Architected](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
