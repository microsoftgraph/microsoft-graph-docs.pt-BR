---
title: tipo de recurso de yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816398"
---
# <a name="yammeractivityuserdetail-resource-type"></a>tipo de recurso de yammerActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | Cadeia de caracteres            |
| displayName       | Cadeia de caracteres            |
| userState         | Cadeia de caracteres            |
| stateChangeDate   | Data              |
| lastActivityDate  | Data              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | String collection |
| reportPeriod      | Cadeia de caracteres            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
