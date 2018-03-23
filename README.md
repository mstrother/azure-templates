# azure-templates

###PowerShell
.\Select-AzureRmSubscription -SubscriptionId $subscriptionId
.\New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force -Verbose
.\New-AzureRmResourceGroupDeployment -Name $resourceGroupDeploymentName -ResourceGroupName $resourceGroupName -TemplateFile $template -Verbose -TemplateParameterFile $templateParametersFile -Force
