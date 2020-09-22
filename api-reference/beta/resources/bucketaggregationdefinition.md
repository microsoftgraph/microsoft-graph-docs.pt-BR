---
title: tipo de recurso bucketAggregationDefinition
description: Fornece os detalhes sobre como o agregations deve ser gerado nos resultados
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1f9fdadefc43b99b8772217db9a9b101357a1c9c
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193837"
---
# <a name="bucketaggregationdefinition-resource-type"></a>tipo de recurso bucketAggregationDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica detalhes para agregar resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|sortBy|bucketAggregationSortProperty| Os valores possíveis são `count` classificados pelo número de correspondências na agregação `keyAsString` para classificar o alphabeticaly com base na chave da agregação, `keyAsNumber` para a classificação numérica com base na chave da agregação. Obrigatório.
|isDescending|Booliano|`True` para especificar a ordem de classificação como decrescente. O padrão é `false` , com a ordem de classificação como crescente. Opcional.|
|prefixFilter|String|Um filtro para definir um critério de correspondência. A chave deve começar com o prefixo especificado a ser retornado na resposta. Opcional.|
|minimumCount|Int32|O número mínimo de itens que devem estar presentes na agregação a serem retornados em um Bucket. Opcional.|
|ranges|coleção [bucketAggregationRange](bucketaggregationrange.md)|Especifica os intervalos manuais para calcular as agregações. Isso é válido apenas para refinadores que não são de cadeia de caracteres do tipo data ou numérico. Opcional.|

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