---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b5c46353d0533fb2c032765527ed5ccf7107e1b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520911"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="f5603-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="f5603-103">searchQuery resource type</span></span>

<span data-ttu-id="f5603-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5603-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5603-105">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="f5603-105">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="f5603-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5603-106">Properties</span></span>

| <span data-ttu-id="f5603-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5603-107">Property</span></span>     | <span data-ttu-id="f5603-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5603-108">Type</span></span>        | <span data-ttu-id="f5603-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5603-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5603-110">query_string</span><span class="sxs-lookup"><span data-stu-id="f5603-110">query_string</span></span>|[<span data-ttu-id="f5603-111">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="f5603-111">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="f5603-112">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f5603-112">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5603-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5603-113">JSON representation</span></span>

<span data-ttu-id="f5603-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5603-114">The following is a JSON representation of the resource.</span></span>

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