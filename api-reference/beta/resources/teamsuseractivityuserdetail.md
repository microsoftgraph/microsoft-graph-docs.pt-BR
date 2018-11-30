---
title: tipo de recurso de teamsUserActivityUserDetail
description: A seguir está uma representaion JSON do recurso.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039809"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>tipo de recurso de teamsUserActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo              |
| :---------------------- | :---------------- |
| reportRefreshDate       | Data              |
| userPrincipalName       | String            |
| lastActivityDate        | Data              |
| isDeleted               | Booliano           |
| deletedDate             | Data              |
| assignedProducts        | String collection |
| teamChatMessageCount    | Int64             |
| privateChatMessageCount | Int64             |
| callCount               | Int64             |
| meetingCount            | Int64             |
| hasOtherAction          | Booliano           |
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
