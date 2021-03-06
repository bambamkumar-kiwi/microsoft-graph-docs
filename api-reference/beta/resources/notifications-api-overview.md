---
title: "Use the notifications REST API in Microsoft Graph"
description: "You can use the notifications API in Microsoft Graph to send push notifications to a user. Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints. Notifications API requests are performed on behalf of a user via delegated permissions and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts."
localization_priority: Priority
ms.prod: "project-rome"
---

# Use the notifications REST API in Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

You can use the notifications API in Microsoft Graph to send push notifications to a user. Simply target a user account to send a notification to, and the platform will deliver the notification to all device endpoints. Notifications API requests are performed on behalf of a user via [delegated permissions](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) and the [notification permission]( /graph/permissions_reference), which can be used with either Microsoft accounts or work or school accounts.
This type of user-centric notification is represented by the [notification](../resources/projectrome-notification.md) resource and is stored in Microsoft Graph. It can then be accessed and managed by the publishing app via the [Project Rome SDK APIs](https://github.com/Microsoft/project-rome). 

## Next steps
- See the [notification resource](../resources/projectrome-notification.md) and create notifications to engage with your users. 
- Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/notifications-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
