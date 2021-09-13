---
title: Tipo de recurso yammerGroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 1cb26b450d5007caf42521a2265c25a57c8d7793
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128470"
---
# <a name="yammergroupsactivitydetail-resource-type"></a>Tipo de recurso yammerGroupsActivityDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo    |
| :----------------- | :------ |
| reportRefreshDate  | Data    |
| groupDisplayName   | Cadeia de Caracteres  |
| isDeleted          | Boleano |
| ownerPrincipalName | Cadeia de Caracteres  |
| lastActivityDate   | Data    |
| groupType          | Cadeia de Caracteres  |
| office365Connected | Boleano |
| memberCount        | Int64   |
| postedCount        | Int64   |
| readCount          | Int64   |
| likedCount         | Int64   |
| networkDisplayName | Cadeia de Caracteres  |
| reportPeriod       | Cadeia de Caracteres  |

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


