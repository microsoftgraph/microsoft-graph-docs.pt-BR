---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331938"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>tipo de recurso de teamsUserActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Data              |
| userPrincipalName       | String            |
| lastActivityDate        | Data              |
| isDeleted               | Boolean           |
| deletedDate             | Data              |
| assignedProducts        | String collection |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Boolean           |
| reportPeriod            | String            |

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
