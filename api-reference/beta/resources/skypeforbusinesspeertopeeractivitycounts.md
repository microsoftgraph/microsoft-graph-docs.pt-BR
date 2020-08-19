---
title: tipo de recurso skypeForBusinessPeerToPeerActivityCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 6bdcd96a8c6eb3dff29304bf8dc1dd8956d9063d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811039"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a>tipo de recurso skypeForBusinessPeerToPeerActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| respectiva                | Int64  |
| audio             | Int64  |
| video             | Int64  |
| appSharing        | Int64  |
| transferência de      | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | String |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024,
  "audio": 1024,
  "video": 1024,
  "appSharing": 1024,
  "fileTransfer": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
