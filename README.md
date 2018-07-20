# adsl-speed-tracker-deploy
ARM templates and other deployment-related gaff for my adsl speed tracker

Deploy the arm template with:

```
Login-AzureRmAccount
New-AzureRmResourceGroup -Name adsl-speed-tracker -location "Australia East"   --If needed
New-AzureRmResourceGroupDeployment -Name {deployment-name} -ResourceGroupName adsl-speed-tracker -TemplateFile .\arm-template.jso
n -TemplateParameterFile .\parameters.json
```
