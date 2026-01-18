# Monitor New Actions in Sentinel & Defender XDR (V2)
After deployment, the Logic App sends a weekly HTML report summarizing new actions detected in the last 7 days. The report includes: 
 - TableName: Source table (e.g., DeviceEvents, SecurityEvent)  
 - Action: Newly observed operation or event type  
 - TotalEntries: Count of occurrences Logic App steps involved: 

## Prerequisites
The logic apps needs the following permissions to run.
 - Office 365 Connection: Enables email delivery of reports. 

**For Managed Identity Graph API Authentication (recommended):**
- Enable SystemAssigned identity for Logic App.    
- Assign ThreatHunting.Read.All permissions via Microsoft Graph to the Managed Identity ([Example](https://ourcloudnetwork.com/assign-permissions-to-a-managed-identity-with-graph-powershell/)). 

**For Application based Graph API Authentication:**
- Register Azure AD App with ThreatHunting.Read.All permissions.    
- Store secrets in Azure Key Vault to avoid plaintext credentials. 

## Configuration
The variables in the logic app should be adjusted to get it configured for your tenant. The Managed Identity Authentication is preferred as it is the safer option, requires less management, and for this specific logic app requires less configuration.
The query and email body variables do not require changes.

### Managed Idenity Authentication
- The recurrence can be set to a preferred day and time at which the report should be delivered.
- RecipientAddress sets one or more recipients of the report.

### Application Authentication
The variables in the logic app should be adjusted to get it configured for your tenant.

- The recurrence can be set to a preferred day and time at which the report should be delivered.
- RecipientAddress sets one or more recipients of the report.
- TenantId should be set to your tenantId.
- ClientID is the id of the Application that connects to the Graph API.

# Deploy Managed Idenity Authentication
Recommended solution.

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FMonitor%2520New%2520Actions%2520in%2520Sentinel%2520%2526%2520Defender%2520XDR%2520(V2)%2Fazuredeploy_mi.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FMonitor%2520New%2520Actions%2520in%2520Sentinel%2520%2526%2520Defender%2520XDR%2520(V2)%2Fazuredeploy_mi.json)

# Deploy Application Authentication

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FMonitor%2520New%2520Actions%2520in%2520Sentinel%2520%2526%2520Defender%2520XDR%2520(V2)%2Fazuredeploy_appsecret.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Frefs%2Fheads%2Fmain%2FMonitor%2520New%2520Actions%2520in%2520Sentinel%2520%2526%2520Defender%2520XDR%2520(V2)%2Fazuredeploy_appsecret.json)

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 18/1/2026 |