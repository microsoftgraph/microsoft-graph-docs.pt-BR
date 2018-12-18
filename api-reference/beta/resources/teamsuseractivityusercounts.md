---
title: tipo de recurso de teamsUserActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330454"
---
# <a name="teamsuseractivityusercounts-resource-type"></a>tipo de recurso de teamsUserActivityUserCounts

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   |
| :------------------ | :----- |
| reportRefreshDate   | Data   |
| reportDate          | Data   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| chamadas               | Int64  |
| reuniões            | Int64  |
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
