---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 1d2d643fed135f97f1ccf2c6346d8fdd6e22f8b5
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193362"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="52120-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="52120-103">searchQuery resource type</span></span>

<span data-ttu-id="52120-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="52120-105">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="52120-105">Represents a search query that contains search terms and optional filters.</span></span>

## <a name="properties"></a><span data-ttu-id="52120-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52120-106">Properties</span></span>

| <span data-ttu-id="52120-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52120-107">Property</span></span>     | <span data-ttu-id="52120-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="52120-108">Type</span></span>        | <span data-ttu-id="52120-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52120-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52120-110">queryString</span><span class="sxs-lookup"><span data-stu-id="52120-110">queryString</span></span>|<span data-ttu-id="52120-111">String</span><span class="sxs-lookup"><span data-stu-id="52120-111">String</span></span>|<span data-ttu-id="52120-112">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52120-112">The search query containing the search terms.</span></span> <span data-ttu-id="52120-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52120-113">Required.</span></span>|
|<span data-ttu-id="52120-114">query_string (preterido)</span><span class="sxs-lookup"><span data-stu-id="52120-114">query_string (deprecated)</span></span>|[<span data-ttu-id="52120-115">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="52120-115">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="52120-116">Agora, ele é substituído pela propriedade **QueryString** .</span><span class="sxs-lookup"><span data-stu-id="52120-116">This is now replaced by the **queryString** property.</span></span> <span data-ttu-id="52120-117">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52120-117">The search query containing the search terms.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52120-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52120-118">JSON representation</span></span>

<span data-ttu-id="52120-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52120-119">The following is a JSON representation of the resource.</span></span>

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

