---
title: tipo de recurso searchQueryString
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 59809860bd2d0954ee8323f9c8e4fe982fb4faa7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703823"
---
# <a name="searchquerystring-resource-type"></a>tipo de recurso searchQueryString

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Os termos de pesquisa da consulta.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|consulta|String|Contém os termos de pesquisa reais da solicitação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQueryString",
  "baseType": null
}-->

```json
{
  "query": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQueryString resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->