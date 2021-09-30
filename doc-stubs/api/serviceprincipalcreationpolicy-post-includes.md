---
title: "Create servicePrincipalCreationConditionSet"
description: "Create a new servicePrincipalCreationConditionSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create servicePrincipalCreationConditionSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new servicePrincipalCreationConditionSet object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /servicePrincipalCreationPolicy/includes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object.

The following table shows the properties that are required when you create the [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|applicationIds|String collection|**TODO: Add Description**|
|applicationTenantIds|String collection|**TODO: Add Description**|
|applicationPublisherIds|String collection|**TODO: Add Description**|
|applicationsFromVerifiedPublisherOnly|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [servicePrincipalCreationConditionSet](../resources/serviceprincipalcreationconditionset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_serviceprincipalcreationconditionset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/servicePrincipalCreationPolicy/includes
Content-Type: application/json
Content-length: 289

{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipalCreationConditionSet",
  "applicationIds": [
    "String"
  ],
  "applicationTenantIds": [
    "String"
  ],
  "applicationPublisherIds": [
    "String"
  ],
  "applicationsFromVerifiedPublisherOnly": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.servicePrincipalCreationConditionSet"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.servicePrincipalCreationConditionSet",
  "id": "15a5fe7c-fe7c-15a5-7cfe-a5157cfea515",
  "applicationIds": [
    "String"
  ],
  "applicationTenantIds": [
    "String"
  ],
  "applicationPublisherIds": [
    "String"
  ],
  "applicationsFromVerifiedPublisherOnly": "Boolean"
}
```

