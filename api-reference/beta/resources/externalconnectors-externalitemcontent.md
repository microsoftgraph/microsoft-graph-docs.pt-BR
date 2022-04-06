---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de uma Pesquisa da Microsoft conexão.
ms.localizationpriority: medium
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 36ca1d19e9be37d7c47c9195fc2c63f677673c0e
ms.sourcegitcommit: f5382652b6880fab42040df40a08de7cb2d74d35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2022
ms.locfileid: "63560088"
---
# <a name="externalitemcontent-resource-type"></a>Tipo de recurso externalItemContent

Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O conteúdo de [um externalItem](externalconnectors-externalitem.md) indexado por meio de Pesquisa da Microsoft [conexão](externalconnectors-externalconnection.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo   | Descrição                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| valor    | Cadeia de caracteres | O conteúdo do externalItem. Obrigatório.                                                 |
| type     | Cadeia de caracteres | O tipo de conteúdo na propriedade value. Os valores possíveis são: `text` e `html`. Esses são os tipos de conteúdo que o indexador suporta e não os tipos de extensão de arquivo permitidos. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
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
