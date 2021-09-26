---
title: Tipo de recurso aggregationOption
description: Especifica quais agregaçãos devem ser retornadas juntamente com os resultados da pesquisa
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c7cf67209fe7b043dcbf391322d3cc65db2a9b3a
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766016"
---
# <a name="aggregationoption-resource-type"></a>Tipo de recurso aggregationOption

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais agregaçãos devem ser retornadas juntamente com os resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------| 
|bucketDefinition|[bucketAggregationDefinition](bucketaggregationdefinition.md)|Especifica os critérios para calcular uma agregação. Opcional.|
|campo|String|Calcula a agregação no campo enquanto o campo existe no tipo de entidade atual. Obrigatório.|
|size|Int32|O número de [recursos searchBucket](searchBucket.md) a serem retornados. Isso não é necessário quando o intervalo é fornecido manualmente na solicitação de pesquisa. Opcional.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.aggregationOption",
  "baseType": null
}-->

```json
{
  "field": "String",
  "size": 1024,
  "bucketDefinition": {"@odata.type": "microsoft.graph.bucketAggregationDefinition"}
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