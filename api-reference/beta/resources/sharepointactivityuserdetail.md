---
title: tipo de recurso sharePointActivityUserDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 20b99e3c6431d945200db868cc02302600e0e76c
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807112"
---
# <a name="sharepointactivityuserdetail-resource-type"></a>tipo de recurso sharePointActivityUserDetail

Namespace: microsoft.graph

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
| visitedPageCount          | Int64             |
| assignedProducts          | Coleção de cadeia de caracteres |
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
