---
title: tipo de recurso de mailboxUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840737"
---
# <a name="mailboxusagestorage-resource-type"></a>tipo de recurso de mailboxUsageStorage

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| reportRefreshDate  | Data   |
| storageUsedInBytes | Int64  |
| reportDate         | Data   |
| reportPeriod       | Cadeia de caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
