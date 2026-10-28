# Deploy Ubuntu Nginx website

[⬅ Projects Index](README.md)

## Goal
Build and explain a real-world AWS workflow using **EC2 + SG + Ubuntu + Nginx**.

## Prerequisites
AWS account with appropriate access, cost estimate, budget alert, selected Region, and disposable resources.

## Steps
1. Draw the architecture and data flow.
2. Identify IAM permissions and security boundaries.
3. Estimate recurring and one-time costs.
4. Launch EC2, allow port 80, install Nginx, publish index.html, browse IP, inspect journalctl and terminate.
5. Verify functionality, health and logs.
6. Capture command outputs and screenshots without credentials.
7. Simulate one safe failure and document recovery.
8. Clean up **all** created resources and verify Billing.

## Interview Questions and Answers

**Q1. How do you secure this project?**

**A:** Least-privilege IAM, encrypted storage and transit, restrictive network rules, logging, patching and secure secrets.

**Q2. How do you troubleshoot a failure?**

**A:** Check the request path from DNS/network through service health and app logs; inspect IAM and CloudWatch/CloudTrail as appropriate.

**Q3. How do you manage cost?**

**A:** Estimate before launch, tag resources, monitor budgets, select minimal capacity and remove unused resources.

## My Notes

- Date:
- Region:
- Expected result:
- Actual result:
- Error and fix:
- Resources cleaned up:
