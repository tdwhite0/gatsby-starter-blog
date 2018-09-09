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




# Azure Function App
The Function App is a thing.