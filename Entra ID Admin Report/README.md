# Entra Admin Report
Schedules a weekly email listing sign-in trend, Conditional Access Policy changes and high priviliged Graph API assignments

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FSLA%2520Reporting%2520Mail%2520Report%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FSLA%2520Reporting%2520Mail%2520Report%2Fazuredeploy.json)

## Configuration
1. Initialize Subscription, Resource Group and Sentinel Instance of your Sentinel environment
2. Set recipient(s) of the report
3. Connect KeyVault for retrieval of Service Principal secret.

## Requirements
- Run Sentinel

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 18/11/2025 |