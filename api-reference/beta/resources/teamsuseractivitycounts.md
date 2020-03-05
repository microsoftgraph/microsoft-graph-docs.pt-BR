---
title: tipo de recurso teamsUserActivityCounts
description: Veja a seguir uma representação JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3066877d109e7dd61243b7cd2f4c105b03c0c533
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519824"
---
# <a name="teamsuseractivitycounts-resource-type"></a>tipo de recurso teamsUserActivityCounts

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   |
| :------------------ | :----- |
| reportRefreshDate   | Data   |
| reportDate          | Data   |
| teamChatMessages    | Int64  |
| privateChatMessages | Int64  |
| calls               | Int64  |
| treinamento            | Int64  |
| reportPeriod        | String |


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
