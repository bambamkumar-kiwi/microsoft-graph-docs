---
title: "plannerPlanDetails resource type"
description: "The **plannerPlanDetails** resource represents the additional information about a plan. Each plan object has a details object."
localization_priority: Normal
author: "TarkanSevilmis"
ms.prod: "planner"
---

# plannerPlanDetails resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.


## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails-get.md) | [plannerPlanDetails](plannerplandetails.md) |Read the properties and relationships of a **plannerPlanDetails** object.|
|[Update](../api/plannerplandetails-update.md) | [plannerPlanDetails](plannerplandetails.md)	|Update a **plannerPlanDetails** object. |

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|An object that specifies the descriptions of the six categories that can be associated with tasks in the plan|
|id|String| Read-only. The ID of the plan details. It is 28 characters long and case-sensitive. [Format validation](tasks-identifiers-disclaimer.md) is done on the service.|
|sharedWith|[plannerUserIds](planneruserids.md)|The set of user IDs that this plan is shared with. If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group. |
|contextDetails|[plannerPlanContextDetailsCollection](plannerplancontextdetailscollection.md)|Read-only. A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container. |

## Relationships
None.


## JSON representation
The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
