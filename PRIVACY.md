# Privacy

When you deploy this template, Microsoft is able to identify the installation of the software with the Azure resources that are deployed. Microsoft is able to correlate the Azure resources that are used to support the software. Microsoft collects this information to provide the best experiences with their products and to operate their business. The data is collected and governed by Microsoft's privacy policies, which can be found at [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?LinkID=824704).

To disable this, simply remove the following section from [deploy.json](./Deployment/deploy.json), [deploykeyvault.json](.Deployment/deploykeyvault.json) and [deploykeyvaultm365.json](./Deployment/deploykeyvaultm365.json) before deploying the resources to Azure:

```json
{ 
    "apiVersion": "2020-10-01",
    "name": "pid-402d4599-92d7-5c69-b137-24515b597ec2",
    "type": "Microsoft.Resources/deployments",
    "properties": {
        "mode": "Incremental",
        "template": {
            "$schema": "https://schema.management.azure.com/schemas/2019-04-01/deploymentTemplate.json#",
            "contentVersion": "1.0.0.0",
            "resources": []
        }
    }
}
```

You can see more information on this at https://docs.microsoft.com/en-us/azure/marketplace/azure-partner-customer-usage-attribution.