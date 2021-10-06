---
title: "Update unifiedRbacResourceNamespace"
description: "Update the properties of an unifiedRbacResourceNamespace object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update unifiedRbacResourceNamespace
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) object.

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
PATCH /unifiedRbacResourceNamespace
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) object.

The following table shows the properties that are required when you update the [unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [unifiedRbacResourceNamespace](../resources/unifiedrbacresourcenamespace.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unifiedrbacresourcenamespace"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/unifiedRbacResourceNamespace
Content-Type: application/json
Content-length: 91

{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceNamespace",
  "name": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.unifiedRbacResourceNamespace",
  "id": "764fcfe7-cfe7-764f-e7cf-4f76e7cf4f76",
  "name": "String"
}
```

