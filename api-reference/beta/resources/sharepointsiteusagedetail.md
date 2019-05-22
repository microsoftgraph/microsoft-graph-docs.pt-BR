---
title: tipo de recurso sharePointSiteUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 10b0f83dc6ed69fc3158e7d5ac6f35e242052042
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344931"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>tipo de recurso sharePointSiteUsageDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| ownerPrincipalName      | String  |
| isDeleted               | Booliano |
| lastActivityDate        | Data    |
| Contagem de FileCount               | Int64   |
| activeFileCount         | Int64   |
| pageViewCount           | Int64   |
| visitedPageCount        | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| rootWebTemplate         | String  |
| reportPeriod            | String  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteId": "Guid", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "ownerPrincipalName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "pageViewCount": 1024, 
  "visitedPageCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "rootWebTemplate": "String", 
  "reportPeriod": "String"
}
```
