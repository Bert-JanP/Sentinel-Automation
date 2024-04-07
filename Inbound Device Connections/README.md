# Inbound Device Connections
This automation flow collects the last 10 inbound connections to a device that has been mentioned in the incident entities. This can help to identify lateral movement to the device.

## Deploy
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FBert-JanP%2FSentinel-Automation-Test%2Fmain%2FCISA-Exploited-Vulnerabilities%2Fazuredeploy.json%3Ftoken%3DGHSAT0AAAAAACHLUUGQNDW2XC7H3RT2OZD4ZQS2E7A)

## Logic App Overview
![Alt text](./Images/LogicAppOverview.png "Inbound Device Connections Overview")

## Results
![Alt text](./Images/Results.png "Inbound Device Connections Results")

## Requirements
- Ingest DeviceNetworkEvents to Sentinel