---
title: tipo de recurso searchHitsContainer
description: Representa a lista de resultados de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192781"
---
# <a name="searchhitscontainer-resource-type"></a>tipo de recurso searchHitsContainer

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a lista de resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|falta|coleção [searchHit](searchhit.md)|Uma coleção dos resultados da pesquisa.|
|moreResultsAvailable|Booliano|Fornece informações se mais resultados estiverem disponíveis. Com base nessas informações, você pode ajustar as propriedades **from** e **size** do [searchRequest](searchrequest.md) adequadamente.|
|total|Int32|O número total de resultados. Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.|
|Aggregations|coleção [searchAggregation](searchaggregation.md)|Contém a coleção de agregações computadas com base no [aggregationOption](aggregationoption.md) fornecido especificado na solicitação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->


```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


