---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e9501831ef2e83d23aa4a5587b9afd8eaa7f5ee8
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703902"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="6460b-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="6460b-103">searchQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6460b-104">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="6460b-104">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="6460b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6460b-105">Properties</span></span>

| <span data-ttu-id="6460b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6460b-106">Property</span></span>     | <span data-ttu-id="6460b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6460b-107">Type</span></span>        | <span data-ttu-id="6460b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6460b-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6460b-109">query_string</span><span class="sxs-lookup"><span data-stu-id="6460b-109">query_string</span></span>|[<span data-ttu-id="6460b-110">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="6460b-110">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="6460b-111">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6460b-111">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6460b-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6460b-112">JSON representation</span></span>

<span data-ttu-id="6460b-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6460b-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
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