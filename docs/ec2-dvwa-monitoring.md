# EC2, DVWA & Monitoring Lab

The recovered CYT160 Lab 4 material describes a controlled AWS security lab built around an Ubuntu EC2 instance hosting DVWA.

## Architecture

```text
Administrator
    |
   SSH
    |
Ubuntu EC2
├── Apache / PHP
├── MySQL
└── DVWA

Monitoring:
EC2 -> EventBridge / CloudWatch -> SNS notification
```

## Monitoring Workflow

The lab configured an SNS topic for notifications, an EventBridge rule for EC2 instance state-change events, and a CloudWatch CPUUtilization alarm to identify an idle instance.

## Validation Goals

- Confirm EC2 instance reachability
- Confirm DVWA application availability
- Confirm state-change notifications
- Confirm idle-instance alarm behavior
- Review monitoring events after test conditions

## Security Handling

The original training document contains example credentials intended only for the vulnerable lab. They are deliberately excluded from this public repository. No real keys, passwords, or student identifiers are stored here.