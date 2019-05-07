# ![LOGO](logo.png) StreamAnalyticsManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the StreamAnalyticsManagementClient API (version 2016-03-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/streamanalytics-streamingjobs/2016-03-01/swagger.json<br/>
Generated at: 2019-05-07T17:39:19+03:00

## API Description



## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists all of the available Stream Analytics related operations.

*Tags:* `Operations`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.

### Lists all of the streaming jobs in the given subscription.

*Tags:* `StreamingJobs`

#### Input Parameters
* `$expand` - _optional_ - The $expand OData query parameter. This is a comma-separated list of additional streaming job properties to include in the response, beyond the default set returned when this parameter is absent. The default set is all streaming job properties other than 'inputs', 'transformation', 'outputs', and 'functions'.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Lists all of the streaming jobs in the specified resource group.

*Tags:* `StreamingJobs`

#### Input Parameters
* `$expand` - _optional_ - The $expand OData query parameter. This is a comma-separated list of additional streaming job properties to include in the response, beyond the default set returned when this parameter is absent. The default set is all streaming job properties other than 'inputs', 'transformation', 'outputs', and 'functions'.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.

### Deletes a streaming job.

*Tags:* `StreamingJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Gets details about the specified streaming job.

*Tags:* `StreamingJobs`

#### Input Parameters
* `$expand` - _optional_ - The $expand OData query parameter. This is a comma-separated list of additional streaming job properties to include in the response, beyond the default set returned when this parameter is absent. The default set is all streaming job properties other than 'inputs', 'transformation', 'outputs', and 'functions'.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Updates an existing streaming job. This can be used to partially update (ie. update one or two properties) a streaming job without affecting the rest the job definition.

*Tags:* `StreamingJobs`

#### Input Parameters
* `If-Match` - _optional_ - The ETag of the streaming job. Omit this value to always overwrite the current record set. Specify the last-seen ETag value to prevent accidentally overwriting concurrent changes.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Creates a streaming job or replaces an already existing streaming job.

*Tags:* `StreamingJobs`

#### Input Parameters
* `If-Match` - _optional_ - The ETag of the streaming job. Omit this value to always overwrite the current record set. Specify the last-seen ETag value to prevent accidentally overwriting concurrent changes.
* `If-None-Match` - _optional_ - Set to '*' to allow a new streaming job to be created, but to prevent updating an existing record set. Other values will result in a 412 Pre-condition Failed response.
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Starts a streaming job. Once a job is started it will start processing input events and produce output.

*Tags:* `StreamingJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

### Stops a running streaming job. This will cause a running streaming job to stop processing input events and producing output.

*Tags:* `StreamingJobs`

#### Input Parameters
* `api-version` - _required_ - Client Api Version.
* `subscriptionId` - _required_ - GUID which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.
* `resourceGroupName` - _required_ - The name of the resource group that contains the resource. You can obtain this value from the Azure Resource Manager API or the portal.
* `jobName` - _required_ - The name of the streaming job.

## License

**flow**ground :- Telekom iPaaS / azure-com-streamanalytics-streamingjobs-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
