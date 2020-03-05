---
title: tipo de recurso searchHitsContainer
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 750bd79dad9758f3ffe883fd87713c42c29c0917
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520918"
---
# <a name="searchhitscontainer-resource-type"></a>tipo de recurso searchHitsContainer

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a lista de resultados de pesquisa.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|falta|coleção [searchHit](searchhit.md)|Encasulate os resultados da pesquisa.|
|moreResultsAvailable|Boolean|Fornece informações se mais resultados estiverem disponíveis. Nesse caso, você pode aumentar o deslocamento "de" e "para".|
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