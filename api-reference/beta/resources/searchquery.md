---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: db647c47c528428820acc2ded9b079546b991be6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985738"
---
# <a name="searchquery-resource-type"></a><span data-ttu-id="dc1be-103">tipo de recurso searchQuery</span><span class="sxs-lookup"><span data-stu-id="dc1be-103">searchQuery resource type</span></span>

<span data-ttu-id="dc1be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc1be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc1be-105">Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.</span><span class="sxs-lookup"><span data-stu-id="dc1be-105">Represents a search query that contains search terms and optional filters.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="dc1be-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc1be-106">Properties</span></span>

| <span data-ttu-id="dc1be-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc1be-107">Property</span></span>     | <span data-ttu-id="dc1be-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc1be-108">Type</span></span>        | <span data-ttu-id="dc1be-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc1be-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dc1be-110">query_string</span><span class="sxs-lookup"><span data-stu-id="dc1be-110">query_string</span></span>|[<span data-ttu-id="dc1be-111">searchQueryString</span><span class="sxs-lookup"><span data-stu-id="dc1be-111">searchQueryString</span></span>](searchquerystring.md)|<span data-ttu-id="dc1be-112">A consulta de pesquisa que contém os termos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dc1be-112">The search query containing the search terms.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc1be-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc1be-113">JSON representation</span></span>

<span data-ttu-id="dc1be-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc1be-114">The following is a JSON representation of the resource.</span></span>

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

