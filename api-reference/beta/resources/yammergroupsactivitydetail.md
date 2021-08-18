---
title: Tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 7c3b10b7b96c40ae7b7404eee2c9af99ea4bc2d602c93f9f6c68ef2ed7ad8cbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176082"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Tipo de recurso yammerGroupsActivityDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo    |
| :----------------- | :------ |
| reportRefreshDate  | Data    |
| groupDisplayName   | Cadeia de caracteres  |
| isDeleted          | Boolean |
| ownerPrincipalName | Cadeia de caracteres  |
| lastActivityDate   | Data    |
| groupType          | Cadeia de caracteres  |
| office365Connected | Boolean |
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


