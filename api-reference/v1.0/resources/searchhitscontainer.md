---
title: Tipo de recurso searchHitsContainer
description: Represente a lista de resultados da pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 42abefb12b0ae1953caf9ecbfa04cd2bc29b69d8c9d8ca2a0797497efb8d6271
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54134956"
---
# <a name="searchhitscontainer-resource-type"></a>Tipo de recurso searchHitsContainer

Namespace: microsoft.graph

Represente a lista de resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hits|[Coleção searchHit](searchhit.md)|Uma coleção dos resultados da pesquisa.|
|moreResultsAvailable|Booliano|Fornece informações se mais resultados estão disponíveis. Com base nessa informação, você pode ajustar as **propriedades from** e **size** da [searchRequest](searchrequest.md) de acordo.|
|total|Int32|O número total de resultados. Observe que esse não é o número de resultados na página, mas o número total de resultados que satisfazem a consulta.|


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


