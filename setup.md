# CloudGuard – Setup Guide

## Overview

This document provides step-by-step instructions to deploy and run the CloudGuard misconfiguration scanner on an Azure subscription using Python and Azure-native services.

## Prerequisites

- Azure account with access to Storage, VMs, NSGs, AD
- Azure CLI installed
- Python 3.8+
- Azure SDK for Python (`pip install azure-mgmt-resource azure-identity`)
- Power BI Desktop or Power BI Online
- Microsoft Teams webhook URL (for alert delivery)

---


## 1. Clone the Repo

```bash 
git clone https://github.com/RohitShardaRohit/CloudGuard-Azure-Misconfig-Scanner
cd CloudGuard-Azure-Misconfig-Scanner
---
```

## 2. Install Dependencies

Install Azure SDK libraries and general-purpose packages:

```bash
pip install azure-identity azure-mgmt-resource pandas requests
```
## 3. Authenticate with Azure
Log in to Azure via the CLI:
```bash
az login
 ```
Confirm your subscription is active:
```bash
az account show
 ```
If you're simulating this setup, use placeholder environment variables or dummy credentials in code.

## 4. (Simulated) First Scan Execution
Run the scanning script locally:
```bash
python cloudguard_scan.py
```
## 5. Setup Scan Automation (Azure Function - Simulated)
Create a placeholder Azure Function to mimic automation:
```bash
# (Optional) Set up Azure Function CLI
func init cloudguard-function --python
```
## 6. Teams Webhook Integration

```bash
{
  "title": "CloudGuard Alert",
  "summary": "8 misconfigured Storage accounts found with public access enabled.",
  "timestamp": "2025-04-27T15:32:00Z"
}
```
## 7. Power BI Dashboard 
Create a Power BI report using the exported JSON or CSV data:
Import
```bash
logs/misconfig_summary.json
```
Create visuals:

-Donut chart of misconfig types

-Time-based chart of finding count

-Table of top risks by severity

This step demonstrates reporting automation even if the data is manually seeded.

## Licensing
This simulated configuration is for demonstration and educational use only.
