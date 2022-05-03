---
title: Tipo de recurso printMargin
description: Especifica as larguras de margem a serem usadas durante a impressão.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 7d6d2e0d1f83cb0da747fb0bb901ba21547612c4
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176669"
---
# <a name="printmargin-complex-type"></a>Tipo complexo printMargin

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica as larguras de margem a serem usadas durante a impressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|top|Int32|A margem em mícrons da borda superior.|
|Fundo|Int32|A margem em mícrons da borda inferior.|
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


