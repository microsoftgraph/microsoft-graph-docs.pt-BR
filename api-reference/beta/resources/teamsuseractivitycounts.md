---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 68eb66cbd0e076d9cf2559170fee4c81dca1e65c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046339"
---
# <a name="teamsuseractivitycounts-resource-type"></a>tipo de recurso teamsUserActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   |
| :------------------ | :----- |
| reportRefreshDate   | Data   |
| reportDate          | Data   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| calls               | Int64  |
| treinamento            | Int64  |
| reportPeriod        | Cadeia de caracteres |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```


