---
title: tipo de recurso de siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879923"
---
# <a name="siteusagestorage-resource-type"></a>tipo de recurso de siteUsageStorage

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| reportRefreshDate  | Data   |
| siteType           | Cadeia de caracteres |
| storageUsedInBytes | Int64  |
| reportDate         | Data   |
| reportPeriod       | Cadeia de caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
