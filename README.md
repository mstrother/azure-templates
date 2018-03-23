# Azure Resource Manager QuickStart Tempates

This repo contains Azure Resource Manager templates that I've created and found useful.

Every deployment tempalte and its associated files is contained in its own folder. The folder name describes what the template does. Usually this naming pattern looks like **ase-create**.

### PowerShell
```
Login-AzureRmAccount
Select-AzureRmSubscription -SubscriptionId $subscriptionId
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force -Verbose
New-AzureRmResourceGroupDeployment -Name $resourceGroupDeploymentName -ResourceGroupName $resourceGroupName -TemplateFile $template -Verbose -TemplateParameterFile $templateParametersFile -Force
```