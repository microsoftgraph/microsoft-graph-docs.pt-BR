---
title: tipo de recurso emailActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cd78b80d97a6dfcaa4c7b97085e89daa4f8a8523
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972198"
---
# <a name="emailactivityuserdetail-resource-type"></a>tipo de recurso emailActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo              |
| :---------------- | :---------------- |
| reportRefreshDate | Data              |
| userPrincipalName | String            |
| displayName       | String            |
| isDeleted         | Booliano           |
| deletedDate       | Data              |
| lastActivityDate  | Data              |
| sendCount         | Int64             |
| receiveCount      | Int64             |
| readCount         | Int64             |
| assignedProducts  | Coleção de cadeias de caracteres |
| reportPeriod      | String            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
