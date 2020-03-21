---
title: tipo de recurso printPageRange
description: Especifica o intervalo de páginas a serem impressas.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 65e2455438dbdb8c7bef3ef3439f846e737ebba0
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895472"
---
# <a name="printpagerange-resource-type"></a>tipo de recurso printPageRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o intervalo de páginas a serem impressas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Inicial|Int32|A página inicial (inclusive) do intervalo. Somente leitura.|
|Página de fim|Int32|A página final (inclusive) do intervalo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printPageRange"
}-->

```json
{
  "startPage": 123456,
  "endPage": 123456
}
```
