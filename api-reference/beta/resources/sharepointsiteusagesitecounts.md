---
title: tipo de recurso sharePointSiteUsageSiteCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 96bb3c9835ea6490893c41595a89a08601e9e88c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965100"
---
# <a name="sharepointsiteusagesitecounts-resource-type"></a>tipo de recurso sharePointSiteUsageSiteCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| sitetype          | String |
| total             | Int64  |
| active            | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
