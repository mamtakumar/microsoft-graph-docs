---
title: "meetingActivityStatistics resource type"
description: "Gets information about meeting activities for MyAnalytics users."
localization_priority: Normal
author: "madehmer"
ms.prod: "insights"
doc_type: "resourcePageType"
---

# meetingActivityStatistics resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gets the following additional details about meeting activities for MyAnalytics users. These are in addition to the standard activity properties pulled for all activities, such as startDate and endDate, which are described in [activityStatistics Properties](../resources/activitystatistics.md#Properties).

## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
| [Update](../api/meetingactivitystatistics-update.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Update meetingActivityStatistics object. |
| [Delete](../api/meetingactivitystatistics-delete.md) | None | Delete meetingActivityStatistics object. |

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|afterHours|Duration|Time spent on meetings outside of working hours.|
|conflicting|Duration|Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).|
|long|Duration|Time spent in long meetings (more than an hour in duration).|
|multitasking|Duration|Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).|
|organized|Duration|Time spent in meetings organized by the user.|
|recurring|Duration|Time spent on recurring meetings.|

## Relationships

None

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics",
  "baseType": ""
}-->

```json
{
  "afterHours": "String (timestamp)",
  "conflicting": "String (timestamp)",
  "long": "String (timestamp)",
  "multitasking": "String (timestamp)",
  "organized": "String (timestamp)",
  "recurring": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->