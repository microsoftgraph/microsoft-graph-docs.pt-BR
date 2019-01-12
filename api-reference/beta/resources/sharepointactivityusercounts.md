---
title: tipo de recurso de sharePointActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9656b39572eac5b6474dd7884eb7d1d2edb17310
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984721"
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
