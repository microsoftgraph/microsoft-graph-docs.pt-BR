---
title: tipo de recurso searchResponse
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 011b027cfcf357dfe80b47067618219cb0067044
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520889"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="07a24-103">tipo de recurso searchResponse</span><span class="sxs-lookup"><span data-stu-id="07a24-103">searchResponse resource type</span></span>

<span data-ttu-id="07a24-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07a24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07a24-105">O searchResponse contém os resultados da consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="07a24-105">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="07a24-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07a24-106">Properties</span></span>

| <span data-ttu-id="07a24-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07a24-107">Property</span></span>     | <span data-ttu-id="07a24-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="07a24-108">Type</span></span>        | <span data-ttu-id="07a24-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="07a24-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="07a24-110">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="07a24-110">hitsContainers</span></span>|<span data-ttu-id="07a24-111">coleção [searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="07a24-111">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="07a24-112">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="07a24-112">A collection of search results.</span></span>|
|<span data-ttu-id="07a24-113">searchTerms</span><span class="sxs-lookup"><span data-stu-id="07a24-113">searchTerms</span></span>|<span data-ttu-id="07a24-114">String collection</span><span class="sxs-lookup"><span data-stu-id="07a24-114">String collection</span></span>|<span data-ttu-id="07a24-115">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="07a24-115">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07a24-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07a24-116">JSON representation</span></span>

<span data-ttu-id="07a24-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07a24-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->