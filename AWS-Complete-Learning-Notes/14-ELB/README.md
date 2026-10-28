# 14. Elastic Load Balancing: ALB, NLB and GWLB

[⬅ Back to AWS Learning Home](../README.md)

## 1. Introduction

Distribute traffic and add health checks.

**Why this matters for Linux/DevOps:** Understanding this topic helps you build, secure, automate, monitor, or troubleshoot production infrastructure.

## 2. Concepts to Understand

- **ALB Layer 7** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **NLB Layer 4** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **target groups** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **listeners** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **health checks** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **TLS** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **cross-zone** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **sticky sessions** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **availability** — research the definition, purpose, configuration choices, limitations, and operational impact.

## 3. Hands-on Lab (Step by Step)

**Prerequisites:** AWS account with appropriate permissions, a selected Region, an approved budget, and a disposable test environment.

1. Read the concepts above and identify the AWS service in the console.
2. Check service pricing and whether your account plan permits this lab.
3. Design two EC2 web servers behind an ALB in two AZs; check target health and test round-robin-style distribution; clean up ALB, target groups and EC2. This lab can incur charges.
4. Record the AWS resource IDs, Region, screenshots (without secrets), and what you observed.
5. Validate the expected result and record any errors and fixes.
6. **Cleanup:** Delete or stop all resources created for the lab, including dependent volumes, snapshots, IPs, log groups and other billable resources where applicable. Confirm deletion and inspect Billing.

## 4. Commands / CLI Practice

Replace placeholder values with your own test resources. Do not paste credentials into Git.

```bash
aws elbv2 describe-load-balancers --output table
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

**Q1. ALB vs NLB?**

**Answer:** ALB handles HTTP(S) Layer 7 routing

**Q2. Why are health checks needed?**

**Answer:** To route traffic only to healthy targets.

## 7. Scenario Question

**Q. You are asked to implement elastic load balancing: alb, nlb and gwlb for a production team. What is your approach?**

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
