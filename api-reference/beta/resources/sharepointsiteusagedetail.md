---
title: tipo de recurso sharePointSiteUsageDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e0827f6b6b991136198fc174e01e7d0e1f91c259
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583995"
---
# <a name="sharepointsiteusagedetail-resource-type"></a>tipo de recurso sharePointSiteUsageDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteId                  | Guid  |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
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
