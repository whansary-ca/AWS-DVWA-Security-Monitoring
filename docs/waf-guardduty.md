# AWS WAF & GuardDuty Lab

The recovered CYT160 Lab 5 material extends the DVWA EC2 environment with an Application Load Balancer, AWS WAF, and GuardDuty.

## Application Load Balancer

The lab used an internet-facing ALB with an instance target group and a DVWA health-check path so the load balancer could verify application health before forwarding traffic.

## AWS WAF

The Web ACL was associated with the ALB. The lab workflow included AWS managed protections for SQL-injection patterns and account-takeover protection for the login path. Validation involved authorized testing against the intentionally vulnerable training application and reviewing blocked requests in WAF.

## GuardDuty

GuardDuty was enabled in the lab region and detector availability was verified. The lab then generated authorized reconnaissance traffic from a separate system and reviewed GuardDuty findings such as port-scan/reconnaissance indicators.

## Skills Demonstrated

- ALB target-group and health-check concepts
- WAF Web ACL association
- AWS managed rule groups
- Web-request security monitoring
- GuardDuty threat detection
- Cloud-security validation and findings review

This document is defensive training documentation for a deliberately vulnerable academic environment.