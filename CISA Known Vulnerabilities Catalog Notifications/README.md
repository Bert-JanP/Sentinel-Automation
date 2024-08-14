# Automate CISA Known Exploited Vulnerabilities Catalog Notifications
This automation flow creates email, Teams and Sentinel notifications based on new entries to the CISA Known Exploited Vulnerabilities Catalog.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FDevice%2520Enrichment%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FDevice%2520Enrichment%2Fazuredeploy.json)

## Configuration
1. Set Variables
2. Configure Azure Monitor Connection
3. Configure Azure Monitor Query Location
4. Configure Exchange Online Connection
5. Configure Sentinel Connection

## Logic App Overview
![Alt text](./Images/LogicAppOverview1.png)
![Alt text](./Images/LogicAppOverview2.png)

## Results
![Alt text](./Images/email.png "Email notification")
![Alt text](./Images/teams.png "Teams notification")
![Alt text](./Images/sentinel.png "Sentinel Incident")

## Requirements
- Email: Log Analytics Workspace
- Teams: Log Analytics Workspace
- Sentinel Incidents: Active Sentinel Environment

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 14/8/2024 |