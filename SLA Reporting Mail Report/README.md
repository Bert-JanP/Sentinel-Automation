# SLA Reporting Mail
This automation flow creates a daily report of how many incidents from the previous day met the SLA, what the SLA timelines are and what incidents failed to meet the SLA.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FReport%2520New%2520Actions%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FReport%2520New%2520Actions%2Fazuredeploy.json)

## Configuration
1. Initialize Subscription, Resource Group and Sentinel Instance of your Sentinel environment
2. Set recipient(s) of the report
3. Configure Azure Monitor Connection
4. Configure Exchange Online connection

## Logic App Overview
![Alt text](./Images/LogicApp.png)

## Results

Demo video: [Video](./Images/SLA%20Reporting%20Mail.mp4)

## Requirements
- Run Sentinel

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 1/3/2025 |