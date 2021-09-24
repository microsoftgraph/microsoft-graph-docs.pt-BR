---
title: Tipo de recurso bucketAggregationDefinition
description: Fornece os detalhes sobre como gerar as agregações nos resultados
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0100852456ec9431e0d0d0bb5cd78d2f236392bb
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507505"
---
# <a name="bucketaggregationdefinition-resource-type"></a>Tipo de recurso bucketAggregationDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes sobre como gerar as agregações nos resultados.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|isDescending|Booliano|`True` para especificar a ordem de classificação como decrescente. O padrão é `false` , com a ordem de classificação como crescente. Opcional.|
|minimumCount|Int32|O número mínimo de itens que devem estar presentes na agregação a ser retornado em um bucket. Opcional.|
|prefixFilter|Cadeia de caracteres|Um filtro para definir um critério correspondente. A chave deve começar com o prefixo especificado a ser retornado na resposta. Opcional.|
|ranges|[Coleção bucketAggregationRange](bucketaggregationrange.md)|Especifica os intervalos manuais para calcular as agregação. Isso só é válido para refinadores que não são de cadeia de caracteres de data ou tipo numérico. Opcional.|
|sortBy|bucketAggregationSortProperty| Os valores possíveis são classificar pelo número de combinações na agregação, classificar alfabética com base na chave na agregação, para classificação numérica com base na chave na `count` `keyAsString` `keyAsNumber` agregação. Obrigatório.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationDefinition",
  "baseType": null
}-->

```json
{
  "sortBy": "String",
  "isDescending": true,
  "prefixFilter": "String",
  "minimumCount": 1024,
  "ranges": [{"@odata.type": "microsoft.graph.bucketAggregationRange"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->