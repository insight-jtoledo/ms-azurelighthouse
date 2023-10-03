# AzureLightHouse

Azure Lighthouse enables multi-tenant management with scalability, higher automation, and enhanced governance across resources.

Azure Lighthouse will support Insight to be more responsive and efficient whilst providing you transparency into Insight’s access and the actions we take. Azure Lighthouse also enables you to have more a granular access management experience across your Azure estate. All without sacrificing any of the existing controls and visibility client currently have over who has access to your environment and individual resources. 

This repository holds the code to perform Azure Lighthouse enablement for Insight Azure Guardian deployments.

![design](./Image/Azure%20Lighthouse%20design.jpg)

Steps to perform Azure Lighthouse deployment

## Pre-requisites

1. User account running this script should have owner permission on the root azure management group.

## Steps

1. Open Cloudshell
2. Git clone https://github.com/Insight-Services-APAC/ms-azurelighthouse.git
3. cd ms-azurelighthouse
4. ./Deploy-AzureLighthouse.ps1
5. Provide the parameters required (Management Group Name, Subscription ID, Resource Group Name, Location, and Country)

|  Parameter Name | Description | Example |
| --- | --- | --- |
| ManagementGroupName | Management group name containing all subscriptions that will be assessed | Tenant Root Group |
| SubscriptionID | The Subscription ID where Azure Guardian solution is deployed | xxxx-xxxx-xxxx-xxxx |
| ResourceGroupName | Resource group where Azure Guardian solution is deployed | prodaeazureguardianrg |
| Location | Location where datacentre is located or preferred | australiaeast or australiasoutheast |
| Country | Primary country where organization resides | AU or NZ |

