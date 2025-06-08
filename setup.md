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

## Step-by-Step

### 1. Clone the Repo
```bash
git clone https://github.com/RohitShardaRohit/CloudGuard-Azure-Misconfig-Scanner
cd CloudGuard-Azure-Misconfig-Scanner
