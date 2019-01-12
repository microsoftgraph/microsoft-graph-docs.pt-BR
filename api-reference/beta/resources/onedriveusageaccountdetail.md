---
title: tipo de recurso de oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957393"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>tipo de recurso de oneDriveUsageAccountDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteUrl                 | Cadeia de caracteres  |
| ownerDisplayName        | Cadeia de caracteres  |
| isDeleted               | Booliano |
| lastActivityDate        | Data    |
| fileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | Cadeia de caracteres  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
