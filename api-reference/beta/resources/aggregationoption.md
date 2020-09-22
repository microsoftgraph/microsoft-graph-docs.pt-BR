---
title: tipo de recurso aggregationOption
description: Especifica a entidade aggregationOption
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c18cc1801e5eac76d2fa4396f809ff68f59a78fe
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193831"
---
# <a name="aggregationoption-resource-type"></a>tipo de recurso aggregationOption

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quais agregações devem ser retornadas junto com os resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|campo|String|Especifica o campo no esquema do tipo de entidade especificado em que a agregação deve ser calculada. Obrigatório.|
|size|Int32|O número de recursos [searchBucket](searchBucket.md) a serem retornados. Isso não é necessário quando o intervalo é fornecido manualmente na solicitação de pesquisa. Opcional.|
|bucketDefinition|[bucketAggregationDefinition](bucketaggregationdefinition.md)|Especifica os critérios para calcular uma agregação. Opcional.|

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