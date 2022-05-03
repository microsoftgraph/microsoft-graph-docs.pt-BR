---
title: Tipo de recurso printPageRange
description: Especifica o intervalo de páginas a serem impressas.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: a8bd855bc4b7d561d9157923d7ce3ace8323b899
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176887"
---
# <a name="printpagerange-resource-type"></a>Tipo de recurso printPageRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o intervalo de páginas a serem impressas.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Startpage|Int32|A página inicial (inclusive) do intervalo. Somente leitura.|
|Endpage|Int32|A página final (inclusive) do intervalo. Somente leitura.|

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


