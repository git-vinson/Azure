# Get-VirusTotalIPReport
author: Nicholas DiCola

This playbook will take each IP entity and query VirusTotal for IP Address Report (https://developers.virustotal.com/v3.0/reference#ip-info). It will write the results to Log Analytics and add a comment to the incident.

## Quick Deployment
**Deploy with incident trigger** (recommended)

After deployment, attach this playbook to an **automation rule** so it runs when the incident is created.

[Learn more about automation rules](https://docs.microsoft.com/azure/sentinel/automate-incident-handling-with-automation-rules#creating-and-managing-automation-rules)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2FAzure-Sentinel%2Fmaster%2FSolutions%2FVirusTotal%2FPlaybooks%2FGet-VirusTotalIPReport%2Fincident-trigger%2Fazuredeploy.json) [![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2FAzure-Sentinel%2Fmaster%2FSolutions%2FVirusTotal%2FPlaybooks%2FGet-VirusTotalIPReport%2Fincident-trigger%2Fazuredeploy.json)

**Deploy with alert trigger**

After deployment, you can run this playbook manually on an alert or attach it to an **analytics rule** so it will run when an alert is created.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2FAzure-Sentinel%2Fmaster%2FSolutions%2FVirusTotal%2FPlaybooks%2FGet-VirusTotalIPReport%2Falert-trigger%2Fazuredeploy.json) [![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2FAzure-Sentinel%2Fmaster%2FSolutions%2FVirusTotal%2FPlaybooks%2FGet-VirusTotalIPReport%2Falert-trigger%2Fazuredeploy.json)

## Prerequisites

- You will need to register to Virus Total community for an API key

## Screenshots
**Incident Trigger**
![Incident Trigger](https://raw.githubusercontent.com/Azure/Azure-Sentinel/master/Solutions/VirusTotal/Playbooks/Get-VirusTotalIPReport/incident-trigger/images/designerLight.png)

**Alert Trigger**
![Alert Trigger](https://raw.githubusercontent.com/Azure/Azure-Sentinel/master/Solutions/VirusTotal/Playbooks/Get-VirusTotalIPReport/alert-trigger/images/Get-VirusTotalIPReport_alert.png)
