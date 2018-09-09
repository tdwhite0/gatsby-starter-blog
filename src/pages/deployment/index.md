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