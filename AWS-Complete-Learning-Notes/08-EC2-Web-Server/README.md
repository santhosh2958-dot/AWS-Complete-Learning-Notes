# 08. Create an Ubuntu Web Server on EC2

[⬅ Back to AWS Learning Home](../README.md)

## 1. Introduction

Install and publish a basic Nginx website on an EC2 Linux instance.

**Why this matters for Linux/DevOps:** Understanding this topic helps you build, secure, automate, monitor, or troubleshoot production infrastructure.

## 2. Concepts to Understand

- **Security group inbound HTTP 80** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **SSH 22 restricted** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **Nginx** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **systemctl** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **user data** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **public IP** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **DNS** — research the definition, purpose, configuration choices, limitations, and operational impact.
- **troubleshooting** — research the definition, purpose, configuration choices, limitations, and operational impact.

## 3. Hands-on Lab (Step by Step)

**Prerequisites:** AWS account with appropriate permissions, a selected Region, an approved budget, and a disposable test environment.

1. Read the concepts above and identify the AWS service in the console.
2. Check service pricing and whether your account plan permits this lab.
3. Launch Ubuntu EC2; install Nginx with sudo apt update && sudo apt install -y nginx; sudo systemctl enable --now nginx; echo a test page using sudo tee /var/www/html/index.html; allow HTTP 80; browse http://PUBLIC_IP; inspect logs; delete instance when finished.
4. Record the AWS resource IDs, Region, screenshots (without secrets), and what you observed.
5. Validate the expected result and record any errors and fixes.
6. **Cleanup:** Delete or stop all resources created for the lab, including dependent volumes, snapshots, IPs, log groups and other billable resources where applicable. Confirm deletion and inspect Billing.

## 4. Commands / CLI Practice

Replace placeholder values with your own test resources. Do not paste credentials into Git.

```bash
sudo apt update
sudo apt install -y nginx
sudo systemctl enable --now nginx
curl -I http://localhost
sudo journalctl -u nginx --no-pager -n 30
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

**Q1. Why does localhost work but public IP fail?**

**Answer:** Check security group, subnet route, public IP, network ACL and host firewall.

**Q2. What does systemctl enable do?**

**Answer:** Configures a service to start at boot.

## 7. Scenario Question

**Q. You are asked to implement create an ubuntu web server on ec2 for a production team. What is your approach?**

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
