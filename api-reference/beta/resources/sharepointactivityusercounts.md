---
title: Tipo de recurso sharePointActivityUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 14a179e5978cf443132684fc3c99bffa2a2ec807
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068442"
---
# <a name="sharepointactivityusercounts-resource-type"></a>Tipo de recurso sharePointActivityUserCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| reportRefreshDate | Data   |
| visitPage       | Int64  |
| viewedOrEdited    | Int64  |
| sincronizado            | Int64  |
| sharedInternally  | Int64  |
| sharedExternally  | Int64  |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "visitedPage": 1024,
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


