---
title: Deploying the Spark Provisioning Engine Flows
date: "2018-09-09T23:46:37.121Z"
---

# High level steps

* Run the ARM template to create Azure Resources
* Update App Settings for both WebJob and Function resources in Azure
* Add Flow custom connector to tenant
  
# Prerequisites
See [Overview](/overview)


# Release Pipeline deployment
Once the inital setup is performed, the intention is to provide a release pipeline in VSTS to automate deployment of changes. Administrators can view code changes in the release to verify their content, then trigger an automated Release to the tenant.

# Azure App Settings
The following settings are required for running the Function App and the WebJobs.
| Name | Example | Remark |
| ------ | ------ | ----- |
| SPTenantUrl | https://rightpoint.sharepoint.com
| Microsoft.ServiceBus.ConnectionString | | Connection string for Azure Service Bus
| ConfigurationStorageAccount |
| ConfigurationStorageAccountKey |
| SPAdminUserName | twhite@rightpoint.onmicrosoft.com | A user account email, DOES NOT have to be a SharePoint Online tenant admin.
| SPAdminPassword
| SPTenantUrl
| SPAdminUrl
| SPTemplateSiteUrl
| ClientId
| ClientSecret
| YammerAppId 
| YammerClientSecret
| YammerDefaultActor
| YammerGlobalAdminToken
| StorageAccountName
| StorageAccountKey
| Disable_YammerJob| 
| Disable_StockTickerJob
| Disable_FlowEventJob
| APPINSIGHTS_INSTRUMENTATIONKEY
| AzureWebJobsDashboard
| AzureWebJobsStorage
| AzureWebJobsServiceBus
