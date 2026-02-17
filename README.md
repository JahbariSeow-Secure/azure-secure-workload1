# Azure App Service Monitoring & Security Lab

## Overview
This project demonstrates deploying a real Azure App Service workload and configuring
enterprise-style monitoring, alerting, and security.

The focus of this lab is cloud operations, visibility, and security—not application development.

## Architecture / Workflow
Users (Allowed IPs) → Azure App Service  
App logs → Log Analytics Workspace  
Metrics & logs → Alert Rules → Action Groups (Email)  
App Service → Defender for Cloud (Security Monitoring)

## What I Implemented
- Azure App Service deployment
- IP access restrictions
- Application & HTTP logs sent to Log Analytics
- CPU utilization alert with Action Group notifications
- Microsoft Defender for Cloud enabled for security posture monitoring

## Monitoring & Alerts
- Log Analytics Workspace collects application and HTTP logs
- Metric-based alert for CPU percentage
- Action Group configured to notify via email when thresholds are exceeded

## Security
- IP-based access restrictions to limit exposure
- Defender for Cloud enabled to monitor security posture and recommendations

## Screenshots
(Insert screenshots here)
- App Service overview
- IP restriction rule
- Log Analytics queries
- Alert rule configuration
- Defender for Cloud dashboard

## Next Steps
- Convert the deployment to Infrastructure as Code (Terraform)
- Add CI/CD using GitHub Actions
- Implement authentication with Microsoft Entra ID
![Resource Group Creation](./screenshots/01-resource-group-creation.png)
![App Service Configuration](./screenshots/02-app-service-configuration.png)
![App Running](./screenshots/03-app-running.png)
![IP Access Restrictions](./screenshots/04-ip-access-restrictions.png)
![Diagnostic Settings](./screenshots/05-diagnostic-settings-log-analytics.png)
![Log Analytics Workspace](./screenshots/06-log-analytics-workspace.png)
![Action Group](./screenshots/07-action-group.png)
![Alert Rule – Action Group](./screenshots/08-alert-rule-action-group.png)
![CPU Alert Rule](./screenshots/09-cpu-alert-rule.png)
![HTTP Logs](./screenshots/10-http-logs.png)

