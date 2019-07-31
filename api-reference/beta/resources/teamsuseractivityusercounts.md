---
title: tipo de recurso teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f0b6d9d77518b6e40a5793c6715bfbae69600f3c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964358"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>tipo de recurso teamsUserActivityUserCounts

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   |
| :------------------ | :----- |
| reportRefreshDate   | Data   |
| reportDate          | Data   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| calls               | Int64  |
| treinamento            | Int64  |
| otherActions        | Int64  |
| reportPeriod        | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
