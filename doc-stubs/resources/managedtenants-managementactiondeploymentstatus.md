---
title: "managementActionDeploymentStatus resource type"
description: "Represents the deployment status for a given management action."
author: "idwilliams"
ms.localizationpriority: medium
ms.prod: "microsoft-365-lighthouse"
doc_type: resourcePageType
---

# managementActionDeploymentStatus resource type

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents the deployment status for a given management action

## Properties
|Property|Type|Description|
|:---|:---|:---|
|managementActionId|String|The unique identifier for the management action. Required. Read-only.|
|managementTemplateId|String|The unique identifier for the management template. Required. Read-only.|
|managementTemplateVersion|Int32|The version for the management template. Required. Read-only.|
|status|managementActionStatus|The deployment status for this management action.. The possible values are: `toAddress`, `completed`, `error`, `timeOut`, `inProgress`, `planned`, `resolvedBy3rdParty`, `resolvedThroughAlternateMitigation`, `riskAccepted`, `unknownFutureValue`. Required.|
|workloadActionDeploymentStatuses|[microsoft.graph.managedTenants.workloadActionDeploymentStatus](../resources/managedtenants-workloadactiondeploymentstatus.md) collection|The collection of workload action deployment statues for the given management action. Optional.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionDeploymentStatus",
  "managementTemplateId": "String",
  "managementTemplateVersion": "Integer",
  "managementActionId": "String",
  "status": "String",
  "workloadActionDeploymentStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadActionDeploymentStatus"
    }
  ]
}
```
