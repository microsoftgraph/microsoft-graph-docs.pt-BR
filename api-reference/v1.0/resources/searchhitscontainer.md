---
title: tipo de recurso searchHitsContainer
description: Representa a lista de resultados de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f32fa198624c04da6eadfc828b60350164cbdddc
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377982"
---
# <a name="searchhitscontainer-resource-type"></a>tipo de recurso searchHitsContainer

Namespace: microsoft.graph

Representa a lista de resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|falta|coleção [searchHit](searchhit.md)|Uma coleção dos resultados da pesquisa.|
|moreResultsAvailable|Boolean|Fornece informações se mais resultados estiverem disponíveis. Com base nessas informações, você pode ajustar as propriedades **from** e **size** do [searchRequest](searchrequest.md) adequadamente.|
|total|Int32|O número total de resultados. Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.|


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
  "total": 1024
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


