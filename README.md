# ![LOGO](logo.png) ApiManagementClient **flow**ground Connector

## Description

A generated **flow**ground connector for the ApiManagementClient API (version 2016-10-10).

Generated from: https://api.apis.guru/v2/specs/azure.com/apimanagement-apimauthorizationservers/2016-10-10/swagger.json<br/>
Generated at: 2019-05-13T12:48:26+03:00

## API Description

Use these REST APIs for managing OAuth2 servers configuration in your Azure API Management deployment. OAuth 2.0 can be used to authorize developer accounts for Azure API Management. For more information refer to [How to OAuth2](https://docs.microsoft.com/en-us/azure/api-management/api-management-howto-oauth2).

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Lists a collection of authorization servers defined within a service instance.

*Tags:* `AuthorizationServers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `$filter` - _optional_ - | Field | Supported operators    | Supported functions                         |
|-------|------------------------|---------------------------------------------|
| id    | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
| name  | ge, le, eq, ne, gt, lt | substringof, contains, startswith, endswith |
* `$top` - _optional_ - Number of records to return.
* `$skip` - _optional_ - Number of records to skip.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Deletes specific authorization server instance.

*Tags:* `AuthorizationServers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `authsid` - _required_ - Identifier of the authorization server.
* `If-Match` - _required_ - The entity state (Etag) version of the authentication server to delete. A value of "*" can be used for If-Match to unconditionally apply the operation.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Gets the details of the authorization server specified by its identifier.

*Tags:* `AuthorizationServers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `authsid` - _required_ - Identifier of the authorization server.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Updates the details of the authorization server specified by its identifier.

*Tags:* `AuthorizationServers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `authsid` - _required_ - Identifier of the authorization server.
* `If-Match` - _required_ - The entity state (Etag) version of the authorization server to update. A value of "*" can be used for If-Match to unconditionally apply the operation.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

### Creates new authorization server or updates an existing authorization server.

*Tags:* `AuthorizationServers`

#### Input Parameters
* `resourceGroupName` - _required_ - The name of the resource group.
* `serviceName` - _required_ - The name of the API Management service.
* `authsid` - _required_ - Identifier of the authorization server.
* `api-version` - _required_ - Version of the API to be used with the client request.
* `subscriptionId` - _required_ - Subscription credentials which uniquely identify Microsoft Azure subscription. The subscription ID forms part of the URI for every service call.

## License

**flow**ground :- Telekom iPaaS / azure-com-apimanagement-apimauthorizationservers-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
