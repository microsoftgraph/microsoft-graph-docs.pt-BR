---
title: tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2188cf1ad583ba66fffb1d7b86009f49fba3f8fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046071"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>tipo de recurso yammerGroupsActivityDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo    |
| :----------------- | :------ |
| reportRefreshDate  | Data    |
| groupDisplayName   | Cadeia de caracteres  |
| isDeleted          | Booliano |
| ownerPrincipalName | Cadeia de caracteres  |
| lastActivityDate   | Data    |
| groupType          | Cadeia de caracteres  |
| office365Connected | Booliano |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| networkDisplayName | Cadeia de caracteres  |
| reportPeriod       | Cadeia de caracteres  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024,
  "networkDisplayName": "String",
  "reportPeriod": "String"
}
```


