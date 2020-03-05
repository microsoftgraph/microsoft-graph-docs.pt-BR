---
title: tipo de recurso yammerActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 922ebf14f59d60a988fe77ee36ce04d9c76befec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519026"
---
# <a name="yammeractivityuserdetail-resource-type"></a>tipo de recurso yammerActivityUserDetail

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | String            |
| displayName       | Cadeia de caracteres            |
| userState         | String            |
| stateChangeDate   | Data              |
| lastActivityDate  | Data              |
| postedCount       | Int64             |
| readCount         | Int64             |
| likedCount        | Int64             |
| assignedProducts  | String collection |
| reportPeriod      | String            |

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
