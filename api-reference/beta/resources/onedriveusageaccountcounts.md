---
title: tipo de recurso de oneDriveUsageAccountCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 959d6602cec98f7351ec3d9819fb9a59599d3e6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037007"
---
# <a name="onedriveusageaccountcounts-resource-type"></a>tipo de recurso de oneDriveUsageAccountCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| siteType          | String |
| total             | Int64  |
| ativo            | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
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
