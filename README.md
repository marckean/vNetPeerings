## The Azure 3 Tier Network
This is a 5 part series of templates to deploy a glorified 3 tier Azure network
1. https://github.com/marckean/Azure-T1-Network
    - Resource Group based template
2. https://github.com/marckean/Azure-T2-Network
    - Resource Group based template
1. https://github.com/marckean/Azure-T3-Network
    - Resource Group based template
1. https://github.com/marckean/Azure-T3plus-Network
    - Resource Group based template
1. https://github.com/marckean/vNetPeerings
    - Subscription based template

| Description |
|---------|
|Resource group deployments deploy to resource groups and use schema: `https://schema.management.azure.com/schemas/2015-01-01/deploymentTemplate.json#`<br><br>Subscription deployments deploy to subscriptions and use schema: `https://schema.management.azure.com/schemas/2018-05-01/subscriptionDeploymentTemplate.json#`|

For the serious security concious, this is one way to achieve super tight network security within Azure. In brief:
- the T1 vNet can't talk directly with the T3 Transit Hub vNet 
- the T3 Transit Hub vNet can't talk directly with the T1 vNet

<p align="center">
  <img src="AzureNetworkT1,T2,T3.jpg" width=80%>
</p>

# Part 5

## Azure-T2-Network
This repo is for the Tier 2 part of the 3 tier network.

![AzureNetworkT2.jpg](AzureNetworkT2.jpg)

To deploy the middle T2 layer of this Azure network:

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmarckean%2FvNetPeerings%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fmarckean%2FvNetPeerings%2Fmaster%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>