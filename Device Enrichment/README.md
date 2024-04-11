# Device Information Enrichment
This automation flow enriches the incident with device information. The information that is collected: DeviceName, OSPlatform, OSVersionInfo, PublicIP, DeviceType, JoinType and ExposureLevel.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fazuredeploy.json)

## Configuration
1. Configure Sentinel Connection
2. Configure Azure Monitor Connection
3. Configure Azure Monitor Query Location

## Logic App Overview
![Alt text](./Images/LogicAppOverview.png)

## Results
![Alt text](./Images/Results.png "Device Information Enrichment Results")

## Requirements
- Ingest DeviceInfo to Sentinel

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 4/11/2024 |