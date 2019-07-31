---
title: tipo de recurso teamsUserActivityUserDetail
description: Veja a seguir uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbe6297388907f28f8841e0a1dcb2ec3ae788844
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964351"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>tipo de recurso teamsUserActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Data              |
| userPrincipalName       | String            |
| lastActivityDate        | Data              |
| isDeleted               | Booliano           |
| deletedDate             | Data              |
| assignedProducts        | Coleção de cadeias de caracteres |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Booliano           |
| reportPeriod            | String            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representaion JSON do recurso.

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
