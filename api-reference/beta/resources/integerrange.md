---
title: tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ee879104878189ddcaf51f65e4e127a61798c811
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986053"
---
# <a name="integerrange-resource-type"></a>tipo de recurso integerRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|iniciar|Int64|O limite inferior inclusivo do intervalo de inteiros.|
|end|Int64|O limite superior inclusivo do intervalo de inteiros.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "start": 12345,
    "end": 12345
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "integerRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

