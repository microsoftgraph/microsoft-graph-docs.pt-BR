---
title: tipo de recurso de sharePointActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: ffbbb8c4d33c94678e8d57d1d9e69da91b22fb39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819927"
---
# <a name="sharepointactivityusercounts-resource-type"></a>tipo de recurso de sharePointActivityUserCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| visitedPage       | Int64  |
| viewedOrEdited    | Int64  |
| sincronizados            | Int64  |
| sharedInternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | Data   |
| reportPeriod      | Cadeia de caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "visitedPage": 1024, 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
