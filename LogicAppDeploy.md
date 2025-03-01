# Logic App Deployment Steps
If you want to create logic app templates just as I have done in this repository you can follow the steps below.

If you publish your Logic Apps/Playbooks publicly keep in mind that you should remove all the private information from your logic app, if dont it may introduce a security risk.

## Create ARM Template
1. Download the ARM Template Generator: [Link](https://aka.ms/Playbook-ARM-Template-Generator)
2. Execute the ARM Template Generator and safe the AzureDeploy.json file in your prefered location.
3. Push the AzureDeploy.json to github.
4. Copy the link of the raw file location
5. Use the PowerShell Script below to format the URL for deploy to Azure button
```PowerShell
$url = "https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/quickstarts/microsoft.storage/storage-account-create/azuredeploy.json"
[uri]::EscapeDataString($url)
```
6. Copy the URL and link it to your deploy button:
```Markdown
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fdev.azure.com%2Forgname%2Fprojectname%2F_apis%2Fgit%2Frepositories%2Freponame%2Fitems%3FscopePath%3D%2freponame%2fazuredeploy.json%26api-version%3D6.0)
```