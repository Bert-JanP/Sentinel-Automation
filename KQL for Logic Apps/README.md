# KQL for Logic Apps
Logic App to show the KQL capabilities of the Graph API, Azure Monitor API and Defender API.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FKQL%2520for%2520Logic%2520Apps%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FKQL%2520for%2520Logic%2520Apps%2Fazuredeploy.json)

## Requirements
- Application with ThreatHunting.Read.All Graph permissions
- Application with Data.Read Log Analytics API permissions
- Application with AdvancedQuery.Read.All Defender ATP permissions
- Managed Identity on the Logic App that has *Key Vault Secrets User* permission on the KeyVault.

[Blog related to the permissions](https://kqlquery.com/posts/hunting-api-kql/)

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 11/7/2025 |
| 1.1 | Adjust query and update README | 14/7/2025 |