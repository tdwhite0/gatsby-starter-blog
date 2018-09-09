---
title: Overview
date: "2018-09-08T23:46:37.121Z"
---

#Overview

The Spark Provisioning Engine Flow solution is a Microsoft Flow custom connector that provides Flow Actions to perform tasks against a SharePoint Online tenant. Using these actions Flows can be created to provision custom SharePoint Modern Site Collections defined using PnP provisioning template xml.

# Limitations
Currently only SharePoint Modern site collection provisioning is supported.

# Available Actions

* Create a Spark Site Collection
* Apply a Spark Template
* Create Term in Spark TermSet
* Set a Web Property Value

# Technical High Level
The solution is made up of a several pieces including:

* Azure Function app to handle requests from Flow [Jump to Content](#Azure Function App)
* Azure WebJob to handle long running tasks like Apply Template
* OpenAPI definition file of the custom connector

# Template Site Collection usage

The solution requires a special site collection on the tenant. This site collection serves two purposes. The first is a repository for page templates. When you click the Create a Spark Page button, this site is queried for pages and the user can select one to use as a starting point for their page. The second is a repository for Provisioning Templates. The templates in this library become available for selection by the Flow actions.

**Important: This site collection must be assigned Read access to all users**

## Creating a template
Templates are provisioned using PnP Provisioning. The Apply a Spark Template action attempts to provision the selected template against the given site collection. If the template is invalid or errors during the provisioning process, the Flow action will error and provide the error message.  



# Azure Function App
The Function App is a thing.