# Monitoring, Alerting, and Incident Response on AWS

This project sets up monitoring for an already deployed AWS workload, the same way real DevOps teams do in production. It covers centralized logging, dashboards, alarms, and a simulated failure to confirm the alerts actually work.

## What This Project Does

- Centralizes application logs using CloudWatch Logs
- Tracks key production metrics, including CPU, memory, errors, and latency
- Creates CloudWatch dashboards for at a glance visibility
- Configures CloudWatch Alarms that trigger on real failure conditions
- Sends alert notifications using Amazon SNS
- Simulates a failure and confirms the alert actually fires
- Uses logs and metrics together to investigate the simulated issue

## Architecture

```
Application workload
        |
        v
CloudWatch Logs (centralized logging)
        |
        v
CloudWatch Metrics and Dashboards
        |
        v
CloudWatch Alarms
        |
        v
Amazon SNS
        |
        v
Email or notification
```
