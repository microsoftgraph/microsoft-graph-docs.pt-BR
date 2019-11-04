---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cb46a41b0c46fe5f70d94a64a91489c9c2e7d43
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936584"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="96ccb-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="96ccb-103">searchQuery resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96ccb-104">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="96ccb-104">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="96ccb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96ccb-105">Properties</span></span>

| <span data-ttu-id="96ccb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96ccb-106">Property</span></span>     | <span data-ttu-id="96ccb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="96ccb-107">Type</span></span>        | <span data-ttu-id="96ccb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="96ccb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96ccb-109">query_string</span><span class="sxs-lookup"><span data-stu-id="96ccb-109">query_string</span></span>|[<span data-ttu-id="96ccb-110">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="96ccb-110">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="96ccb-111">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="96ccb-111">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96ccb-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96ccb-112">JSON representation</span></span>

<span data-ttu-id="96ccb-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96ccb-113">The following is a JSON representation of the resource.</span></span>

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