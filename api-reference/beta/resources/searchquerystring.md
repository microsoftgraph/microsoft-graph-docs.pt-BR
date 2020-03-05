---
title: tipo de recurso searchQueryString
description: searchQueryString
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b273d9ec15b949019b780dd5ce9f1a6184191763
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520903"
---
# <a name="searchquerystring-resource-type"></a>tipo de recurso searchQueryString

Namespace: Microsoft. Graph

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