---
title: "Update user"
description: "Update the properties of a user object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update user
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [user](../resources/user.md) object.

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
PATCH /me
PATCH /users/{usersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [user](../resources/user.md) object.

The following table shows the properties that are required when you update the [user](../resources/user.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|temporaryAccessPass|[Microsoft.DirectoryServices.temporaryAccessPass](../resources/temporaryaccesspass.md)|**TODO: Add Description**|
|accountEnabled|Boolean|**TODO: Add Description**|
|ageGroup|String|**TODO: Add Description**|
|assignedLicenses|[Microsoft.DirectoryServices.assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[Microsoft.DirectoryServices.assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|consentProvidedForMinor|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|creationType|String|**TODO: Add Description**|
|customSecurityAttributes|[Microsoft.DirectoryServices.customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|deviceKeys|[Microsoft.DirectoryServices.deviceKey](../resources/devicekey.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|employeeHireDate|DateTimeOffset|**TODO: Add Description**|
|employeeId|String|**TODO: Add Description**|
|employeeOrgData|[Microsoft.DirectoryServices.employeeOrgData](../resources/employeeorgdata.md)|**TODO: Add Description**|
|employeeType|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|identities|[Microsoft.DirectoryServices.objectIdentity](../resources/objectidentity.md) collection|**TODO: Add Description**|
|imAddresses|String collection|**TODO: Add Description**|
|infoCatalogs|String collection|**TODO: Add Description**|
|isManagementRestricted|Boolean|**TODO: Add Description**|
|isResourceAccount|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|lastPasswordChangeDateTime|DateTimeOffset|**TODO: Add Description**|
|legalAgeGroupClassification|String|**TODO: Add Description**|
|licenseAssignmentStates|[Microsoft.DirectoryServices.licenseAssignmentState](../resources/licenseassignmentstate.md) collection|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|onPremisesDistinguishedName|String|**TODO: Add Description**|
|onPremisesExtensionAttributes|[Microsoft.DirectoryServices.onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description**|
|onPremisesImmutableId|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[Microsoft.DirectoryServices.onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesSamAccountName|String|**TODO: Add Description**|
|onPremisesUserPrincipalName|String|**TODO: Add Description**|
|otherMails|String collection|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[Microsoft.DirectoryServices.passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredDataLocation|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|provisionedPlans|[Microsoft.DirectoryServices.provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|refreshTokensValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|signInSessionsValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|streetAddress|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|externalUserState|String|**TODO: Add Description**|
|externalUserStateChangeDateTime|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [user](../resources/user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_user"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me
Content-Type: application/json
Content-length: 3085

{
  "@odata.type": "#microsoft.graph.user",
  "deletedDateTime": "String (timestamp)",
  "temporaryAccessPass": {
    "@odata.type": "microsoft.graph.temporaryAccessPass"
  },
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "creationType": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "department": "String",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey"
    }
  ],
  "displayName": "String",
  "employeeHireDate": "String (timestamp)",
  "employeeId": "String",
  "employeeOrgData": {
    "@odata.type": "microsoft.graph.employeeOrgData"
  },
  "employeeType": "String",
  "faxNumber": "String",
  "givenName": "String",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "infoCatalogs": [
    "String"
  ],
  "isManagementRestricted": "Boolean",
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesDomainName": "String",
  "onPremisesSamAccountName": "String",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "externalUserState": "String",
  "externalUserStateChangeDateTime": "String",
  "userType": "String"
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
  "@odata.type": "#microsoft.graph.user",
  "id": "baa047d2-47d2-baa0-d247-a0bad247a0ba",
  "deletedDateTime": "String (timestamp)",
  "temporaryAccessPass": {
    "@odata.type": "microsoft.graph.temporaryAccessPass"
  },
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "String (timestamp)",
  "creationType": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "department": "String",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey"
    }
  ],
  "displayName": "String",
  "employeeHireDate": "String (timestamp)",
  "employeeId": "String",
  "employeeOrgData": {
    "@odata.type": "microsoft.graph.employeeOrgData"
  },
  "employeeType": "String",
  "faxNumber": "String",
  "givenName": "String",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "infoCatalogs": [
    "String"
  ],
  "isManagementRestricted": "Boolean",
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesDomainName": "String",
  "onPremisesSamAccountName": "String",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": "Boolean",
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "externalUserState": "String",
  "externalUserStateChangeDateTime": "String",
  "userType": "String"
}
```

