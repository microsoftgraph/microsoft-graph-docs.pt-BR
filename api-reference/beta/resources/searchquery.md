---
title: Tipo de recurso searchQuery
description: searchQuery
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0c437bcb8fd7462d8c4bc85514c40d47311155de
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589314"
---
# <a name="searchquery-resource-type"></a>Tipo de recurso searchQuery

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|queryString|Cadeia de caracteres|A consulta de pesquisa que contém os termos de pesquisa. Obrigatório.|
|queryTemplate|String|Fornece uma maneira de enfeitar a cadeia de caracteres de consulta. Oferece suporte a KQL e variáveis de consulta. Opcional.|
|query_string (preterido)|[searchQueryString](searchquerystring.md)|Isso agora é substituído pela **propriedade queryString** . A consulta de pesquisa que contém os termos de pesquisa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String",
  "queryTemplate": "String",
  "query_string": {"@odata.type": "microsoft.graph.searchQueryString"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

