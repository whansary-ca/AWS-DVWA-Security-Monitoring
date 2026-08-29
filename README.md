# AWS DVWA Security Monitoring

AWS security coursework centered on deploying Damn Vulnerable Web Application (DVWA) on EC2, monitoring the instance, placing it behind an Application Load Balancer, and applying AWS security-monitoring controls with WAF and GuardDuty.

## Recovered Lab Scope

### Lab 4 — DVWA on EC2 & Monitoring

- Ubuntu EC2 instance
- Apache, PHP, MySQL and DVWA
- Security-group configuration for controlled lab access
- CloudWatch monitoring
- EventBridge rule for EC2 state-change events
- SNS email notifications
- CPU-utilization alarm for idle-instance monitoring

### Lab 5 — WAF & GuardDuty

- Application Load Balancer and target group
- DVWA health-check path
- AWS WAF Web ACL associated with the ALB
- AWS managed SQL-injection protection rules
- Account-takeover-protection rule group / CAPTCHA workflow
- WAF request/log review
- GuardDuty enablement and detector verification
- Authorized lab traffic generation with Nmap to observe security findings

## Evidence Status

A recovered Lab 5 submission document contains result sections for ALB configuration, WAF SQL-injection testing, login-page managed rules, WAF monitoring, GuardDuty detector verification, and GuardDuty findings. The original screenshots are not currently recoverable as standalone image files, so this repo does not fabricate visual evidence.

## Security Note

This repository documents intentionally vulnerable training infrastructure used only in an authorized academic lab. Example passwords, student identifiers, private IPs, and credentials are intentionally omitted.

## Documentation

- `docs/ec2-dvwa-monitoring.md`
- `docs/waf-guardduty.md`
- `docs/evidence-status.md`

## Project Type

Academic cloud-security lab — Seneca Polytechnic, CYT160.