---
title: tipo de recurso teamsUserActivityUserDetail
description: Veja a seguir uma representaion JSON do recurso.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582903"
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
