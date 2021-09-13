---
title: Tipo de recurso siteUsageStorage
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: c8c6013da34233a9cb58baa067abe1c3ea4901b6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033193"
---
# <a name="siteusagestorage-resource-type"></a>Tipo de recurso siteUsageStorage

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo   |
| :----------------- | :----- |
| reportRefreshDate  | Data   |
| siteType           | Cadeia de Caracteres |
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


