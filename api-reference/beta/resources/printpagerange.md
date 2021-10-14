---
title: Tipo de recurso printPageRange
description: Especifica o intervalo de páginas a serem impressas.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 229b13a398a01412a7c85e1df954dcddffb2ed9c
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2021
ms.locfileid: "60354732"
---
# <a name="printpagerange-resource-type"></a>Tipo de recurso printPageRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o intervalo de páginas a serem impressas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|startPage|Int32|A página inicial (inclusive) do intervalo. Apenas leitura.|
|endPage|Int32|A página final (inclusive) do intervalo. Somente leitura.|

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
  "startPage": "Int32",
  "endPage": "Int32"
}
```


