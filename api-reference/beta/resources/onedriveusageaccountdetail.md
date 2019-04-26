---
title: tipo de recurso oneDriveUsageAccountDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563541"
---
# <a name="onedriveusageaccountdetail-resource-type"></a>tipo de recurso oneDriveUsageAccountDetail

## <a name="properties"></a>Propriedades

| Propriedade                | Tipo    |
| :---------------------- | :------ |
| reportRefreshDate       | Data    |
| siteUrl                 | String  |
| ownerDisplayName        | String  |
| isDeleted               | Booliano |
| lastActivityDate        | Data    |
| Contagem de FileCount               | Int64   |
| activeFileCount         | Int64   |
| storageUsedInBytes      | Int64   |
| storageAllocatedInBytes | Int64   |
| reportPeriod            | String  |

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
