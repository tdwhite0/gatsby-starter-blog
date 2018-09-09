---
title: Function App Setup
date: "2018-09-08T23:46:37.121Z"
---

## What it Does
The Function App component of the solution handles the HTTP requests that are sent by Microsoft Flow. In most cases, the function executes the requested action itself, but in the case of applying a PnP Provisioning Template it delegates to the WebJob for processing.

The custom Flow connector file maps the Flow Actions to inputs and outputs of the functions.

## Setup Guide
If your Azure resources have already been created using the ARM template, all you need to do is deploy the function project zip file to the Function App in Azure, and update its App Settings to match your environment.

You can configure a Release pipeline in VSTS to deploy the app automatically, or you can publish from source using the Azure CLI.

## Configuring the Release Pipeline
Information to configure a new target to come soon.

## Troubleshooting

## Technical Considerations