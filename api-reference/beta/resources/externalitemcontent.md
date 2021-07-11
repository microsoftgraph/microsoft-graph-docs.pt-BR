---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 036b2e2d4081160680b7f5471bd2707ee503bc4a
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366538"
---
# <a name="externalitemcontent-resource-type"></a>Tipo de recurso externalItemContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O conteúdo de [um externalItem](externalitem.md) indexado por meio de uma conexão Pesquisa da Microsoft [.](externalconnection.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| valor    | Cadeia de caracteres | O conteúdo do externalItem. Obrigatório.                                                 |
| tipo     | String | O tipo de conteúdo na propriedade value. Os valores possíveis são: `text` e `html`. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


