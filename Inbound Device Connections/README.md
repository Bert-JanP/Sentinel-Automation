# Inbound Device Connections
This automation flow collects the last 10 inbound connections to a device that has been mentioned in the incident entities. This can help to identify lateral movement to the device.

## Deploy Public Inbound Device Connections
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fazuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fazuredeploy.json)

## Deploy All Inbound Device Connections
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fall_azuredeploy.json)

[![Deploy to Azure Gov](https://aka.ms/deploytoazuregovbutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2Fall_azuredeploy.json)

## Configuration
1. Configure Sentinel Connection
2. Configure Azure Monitor Connection
3. Configure Azure Monitor Query Location

## Logic App Overview
![Alt text](./Images/LogicAppOverview.png "Inbound Device Connections Overview")

## Results
![Alt text](./Images/Results.png "Inbound Device Connections Results")

## Requirements
- Ingest DeviceNetworkEvents to Sentinel

# Version
| Version | Description | Date |
| ------- | ---------- | ----- |
| 1.0 | Initial Version | 4/9/2024 |
| 1.1 | Include different version Public and All inbound connections | 10/9/2024 |