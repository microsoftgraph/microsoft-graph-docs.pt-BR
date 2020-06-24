---
title: tipo de recurso de multimargem
description: Especifica as larguras de margem a serem usadas ao imprimir.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d7399f45138d6ab7d82f33e6577e7d08967ad15
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863695"
---
# <a name="printmargin-complex-type"></a>tipo complexo de transmargem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as larguras de margem a serem usadas ao imprimir.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|top|Int32|A margem em mícrons da borda superior.|
|bottom|Int32|A margem em mícrons da borda inferior.|
|Certo|Int32|A margem em mícrons da borda direita.|
|left|Int32|A margem em mícrons da borda esquerda.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printMargin"
}-->

```json
{
  "top": 123456,
  "bottom": 123456,
  "right": 123456,
  "left": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printMargin resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
