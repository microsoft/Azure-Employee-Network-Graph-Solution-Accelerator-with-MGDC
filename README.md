---
page_type: sample
languages:
- python
products:
- azure-synapse-analytics
- microsoft-graph-data-connect-api
- power-bi
---

![EmployeeNetworkGrpah](./Deployment/img/EmployeeNetworkGraph.png)
# Azure Employee Network Graph Solution Accelerator with MGDC
Organizations that can tap into the large datasets powering Microsoft 365, CRM and sales systems can gain tremendous insights into the challenges and opportunities they may encounter. Employee network graphs and data insights from interactions can improve sales productivity, enable organizational optimization and intelligent workflows, and ensure compliance.

This solution connects Microsoft 365 data with Azure Synapse Analytics using Microsoft Graph Data Connect. The accelerator automates the end-to-end pipeline to set up initial and delta loads at scale. This solution takes a privacy by design approach and comes with folder filter capability where a user can choose which folders data is extracted and used in analysis.

![SAIntroduction](./Deployment/img/SAIntroduction.png "SA Introduction")

## Prerequisites
To use this solution accelerator, you will need access to an [Azure subscription](https://azure.microsoft.com/free/), Microsoft 365 account and Microsoft Graph Data Connect(MGDC) enabled.

For additional training and support, please see:

1. [Azure Synapse Analytics](https://azure.microsoft.com/en-us/services/synapse-analytics/) 
2. [Microsoft Graph Data Connect](https://docs.microsoft.com/en-us/graph/)
3. [Azure Cosmos DB](https://azure.microsoft.com/en-us/services/cosmos-db/)
4. [Azure Text Analytics](https://azure.microsoft.com/en-us/services/cognitive-services/text-analytics/)
3. [Power BI](https://docs.microsoft.com/en-us/power-bi/)

## Getting Started
Start by deploying the required resources to Azure. The button below will deploy Azure Synapse Analytics, Azure Data Lake Storage, Azure Cosmos DB, Azure Language Service, Azure Key Vault and its related resources:

> **Note**: 
> * Azure Cogntive Services require to accept the terms and conditions of Responsible AI when they are first provisioned in an Azure subscription. If none of the Cognitive Services were provisioned previously in the Azure subscription, it is necessary to create a temporary cognitive service (for example Language Service) to accept the AI license terms. The service can be dropped after the creation. Once the requirements are in place, the deploy to Azure button can be used to deploy and configure the solution.
> * We are deploying tier 0. If you are loading more data you will need to increase the tier to match your data laod needs.


[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmicrosoft%2FAzure-Employee-Network-Graph-Solution-Accelerator-with-MGDC%2Fmain%2FDeployment%2Fdeploy.json)

* Go to the [Deployment guide](./Deployment/Deployment.md) to set up your Azure resources for this solution.  

## Architecture

The architecture diagram below details what you will be building for this Solution Accelerator.

![Employee Network Graph Architecture Diagram](./Deployment/img/EmployeeNetworkGraphSAArchitectire.png "Employee Network Graph Architecture Diagram")


## Power BI Dashboards

The organization summary dashboard shows all internal and external contacts for a specific account, their connectivity scores and event timeline.

![Organization Network Graph Dashboard](./Deployment/img/OrganizationNetworkOverview.png "Organization Network Graph Dashboard")

The organization detail dashboard shows top contacts at an account, a network of internal and external contacts and an event tracker.

![Organization Network Graph Dashboard](./Deployment/img/OrganizationNetworkGraphDetail.png "Organization Network Graph Dashboard")


The employee summary dashboard shows the all accounts and external contacts the employee is connected with, their connectivity scores and event timeline.

![Employee Network Graph Details Page](./Deployment/img/EmployeeNetworkGraphDetail.png "Employee Network Graph Details Page")

The employee detail dashboard shows top contacts at all account, a network of internal and external contacts and entities.

![Employee Network Graph Details Page](./Deployment/img/EmployeeNetworkGraphDetailEntity.png "Employee Network Graph Details Page")

## License
MIT License

Copyright (c) Microsoft Corporation.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE

## Note about Libraries with MPL-2.0 License
The following libraries are not explicitly included in this repository, but users who use this Solution Accelerator may need to install them locally and in Azure Synapse Analytics to fully utilize this Solution Accelerator. However, the actual binaries and files associated with the libraries are not included as part of this repository, but they are available for installation via the PyPI library using the pip installation tool.

Libraries: certifi

## Contributing
This project welcomes contributions and suggestions.  Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks
This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general). Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship. Any use of third-party trademarks or logos are subject to those third-party's policies.

## Data Collection
The software may collect information about you and your use of the software and send it to Microsoft. Microsoft may use this information to provide services and improve our products and services. You may turn off the telemetry as described in the repository. There are also some features in the software that may enable you and Microsoft to collect data from users of your applications. If you use these features, you must comply with applicable law, including providing appropriate notices to users of your applications together with a copy of Microsoft's privacy statement. Our privacy statement is located at https://go.microsoft.com/fwlink/?LinkID=824704. You can learn more about data collection and use in the help documentation and our privacy statement. Your use of the software operates as your consent to these practices.

