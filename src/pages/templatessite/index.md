---
title: The Templates Site Collection
date: "2018-09-09T23:46:37.121Z"
---

# Template Site Collection usage

The solution requires a special site collection on the tenant. This site collection serves two purposes. The first is a repository for page templates. When you click the Create a Spark Page button, this site is queried for pages and the user can select one to use as a starting point for their page. The second is a repository for Provisioning Templates. The templates in this library become available for selection by the Flow actions.

**Important: This site collection must be assigned Read access to all users**

## Creating a template
Templates are provisioned using PnP Provisioning. The Apply a Spark Template action attempts to provision the selected template against the given site collection. If the template is invalid or errors during the provisioning process, the Flow action will error and provide the error message.  
