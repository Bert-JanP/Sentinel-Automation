# New Action Found Entra Admin
This logic app sends a weekly report with the new actions found in identity related tables, this is aimed for identity/entra administrators.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FEntra%2520ID%2520Admin%2520Report%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FEntra%2520ID%2520Admin%2520Report%2Fazuredeploy.json)

## Configuration
1. Initialize tenant and application ID
2. Connect KeyVault for retrieval of Service Principal secret.
3. Required Graph API permissions see: [Hunting Through APIs](https://kqlquery.com/posts/hunting-api-kql/)

## Requirements
- Run Sentinel

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 18/11/2025 |