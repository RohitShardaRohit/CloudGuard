# CloudGuard – Automated Cloud Misconfiguration Scanner

## Overview
CloudGuard is a Python-based tool that automates security misconfiguration scanning across Azure services and reports findings in real time. It integrates DevOps and cloud security practices to support continuous compliance, visibility, and rapid response.

## Technologies Used

| Tool                   | Purpose                                        |
|------------------------|------------------------------------------------|
| Azure SDK for Python   | Resource scanning and automation               |
| Azure Functions        | Scheduled, serverless scan execution           |
| Azure Monitor          | Logs and alert triggering                      |
| Power BI               | Dashboarding scan results                      |
| Microsoft Teams Webhook| Push real-time alerts to Teams channels        |
| Python, Pandas         | Data extraction, parsing, reporting            |

## Key Results

- Detected and flagged over **40+ misconfigurations** across services like Azure Storage, AD, VMs, and NSGs
- Reduced excessive access privileges by **60%** through automated least-privilege enforcement
- Reduced remediation time by **70%** using Power BI and Teams integration

## Features

- Scans Azure resources for:
  - Publicly accessible storage
  - Open NSG rules
  - Overprivileged RBAC roles
- Automatically schedules scans via Azure Functions
- Sends real-time alerts to Microsoft Teams
- Generates a Power BI dashboard for visual reporting

## Screenshots

- Azure Monitor Alert Trigger  
  ![Azure Monitor](screenshots/azure_monitor_alert.png)
- Power BI Dashboard  
  ![Power BI](screenshots/powerbi_dashboard_sample.png)
- Teams Webhook Notification  
  ![Teams Webhook](screenshots/teams_webhook_alert.png)

## Output Samples

- [cloudguard_scan_output.txt](logs/cloudguard_scan_output.txt)  
- [misconfig_summary.json](logs/misconfig_summary.json)

## Setup Instructions

See [setup.md](./setup.md) for full installation and configuration steps.

## Contact

Built by Rohit Sharda  
[LinkedIn](https://linkedin.com/in/rohitsharda) | rohitsharda.dev@gmail.com
