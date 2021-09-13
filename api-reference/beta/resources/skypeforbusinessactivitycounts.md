---
title: Tipo de recurso skypeForBusinessActivityCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: 8591596604e53d077f2f966dc794c7f346f42c9b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074546"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a>Tipo de recurso skypeForBusinessActivityCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   |
| :---------------- | :----- |
| peerToPeer        | Int64  |
| organizado         | Int64  |
| participado      | Int64  |
| reportRefreshDate | Data   |
| reportDate        | Data   |
| reportPeriod      | Cadeia de caracteres |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024,
  "organized": 1024,
  "participated": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


