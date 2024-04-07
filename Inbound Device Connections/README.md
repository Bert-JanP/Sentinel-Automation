# Inbound Device Connections
This automation flow collects the last 10 inbound connections to a device that has been mentioned in the incident entities. This can help to identify lateral movement to the device.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation%2Fmain%2FInbound%2520Device%2520Connections%2FSentinel-Automation-InboundConnections%2Fazuredeploy.json)

## Logic App Overview
![Alt text](./Images/LogicAppOverview.png "Inbound Device Connections Overview")

## Results
![Alt text](./Images/Results.png "Inbound Device Connections Results")

## Requirements
- Ingest DeviceNetworkEvents to Sentinel