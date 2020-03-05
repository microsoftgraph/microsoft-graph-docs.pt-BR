---
title: tipo de recurso skypeForBusinessPeerToPeerActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2df9cd9e7887c955190c8478cd8075a077929133
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520454"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a>tipo de recurso skypeForBusinessPeerToPeerActivityUserCounts

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| respectiva                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| appSharing        | Int64  |
| transferência de      | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
