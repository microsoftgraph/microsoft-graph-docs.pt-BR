---
title: tipo de recurso de oneDriveActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035852"
---
# <a name="onedriveactivityuserdetail-resource-type"></a>tipo de recurso de oneDriveActivityUserDetail

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo              |
| :------------------------ | :---------------- |
| reportRefreshDate         | Data              |
| userPrincipalName         | String            |
| isDeleted                 | Booliano           |
| deletedDate               | Data              |
| lastActivityDate          | Data              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| assignedProducts          | String collection |
| reportPeriod              | String            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
