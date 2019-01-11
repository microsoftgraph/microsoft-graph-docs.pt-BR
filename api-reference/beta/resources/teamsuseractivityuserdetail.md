---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823650"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>tipo de recurso de teamsUserActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Data              |
| userPrincipalName       | Cadeia de caracteres            |
| lastActivityDate        | Data              |
| isDeleted               | Booliano           |
| deletedDate             | Data              |
| assignedProducts        | String collection |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Booliano           |
| reportPeriod            | Cadeia de caracteres            |

## <a name="json-representation"></a>Representação JSON

A seguir está uma representaion JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
