---
title: tipo de recurso de teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c7351795f6b3dafbac996844fc1ac11cd24bbc03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886587"
---
# <a name="teamsuseractivitycounts-resource-type"></a>tipo de recurso de teamsUserActivityCounts

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   |
| :------------------ | :----- |
| reportRefreshDate   | Data   |
| reportDate          | Data   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| chamadas               | Int64  |
| reuniões            | Int64  |
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
