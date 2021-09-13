---
title: Tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: e9b52be3048ce3625ebf98f7167c99f93c4fb4cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068428"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>Tipo de recurso sharePointActivityUserDetail

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo              |
| :------------------------ | :---------------- |
| reportRefreshDate         | Data              |
| userPrincipalName         | Cadeia de caracteres            |
| isDeleted                 | Boolean           |
| deletedDate               | Data              |
| lastActivityDate          | Data              |
| viewedOrEditedFileCount   | Int64             |
| syncedFileCount           | Int64             |
| sharedInternallyFileCount | Int64             |
| sharedExternallyFileCount | Int64             |
| visitPageCount          | Int64             |
| assignedProducts          | String collection |
| reportPeriod              | String            |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
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
  "visitedPageCount": 1024,
  "assignedProducts": ["String"],
  "reportPeriod": "String"
}
```


