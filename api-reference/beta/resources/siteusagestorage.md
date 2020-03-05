---
title: tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 33d78540a6dd5b3c15cb6d8fce80496be19f0711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520517"
---
# <a name="siteusagestorage-resource-type"></a>tipo de recurso siteUsageStorage

Namespace: Microsoft. Graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| reportRefreshDate  | Data   |
| sitetype           | String |
| storageUsedInBytes | Int64  |
| reportDate         | Data   |
| reportPeriod       | String |

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
