---
title: tipo de recurso de yammerGroupsActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: a308b6180eaf91614247b0b5f47064ae7e7de2b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039807"
---
# <a name="yammergroupsactivitycounts-resource-type"></a>tipo de recurso de yammerGroupsActivityCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| curtidas             | Int64  |
| lançada            | Int64  |
| leitura              | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
