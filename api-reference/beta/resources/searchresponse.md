---
title: tipo de recurso searchResponse
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6b433e5aba652a9f68d017975e0651edac4e2ffb
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703992"
---
# <a name="searchresponse-resource-type"></a><span data-ttu-id="7f118-103">tipo de recurso searchResponse</span><span class="sxs-lookup"><span data-stu-id="7f118-103">searchResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f118-104">O searchResponse contém os resultados da consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7f118-104">The searchResponse contains the results from the search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="7f118-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f118-105">Properties</span></span>

| <span data-ttu-id="7f118-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f118-106">Property</span></span>     | <span data-ttu-id="7f118-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f118-107">Type</span></span>        | <span data-ttu-id="7f118-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f118-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7f118-109">hitsContainers</span><span class="sxs-lookup"><span data-stu-id="7f118-109">hitsContainers</span></span>|<span data-ttu-id="7f118-110">coleção [searchHitsContainer](searchhitscontainer.md)</span><span class="sxs-lookup"><span data-stu-id="7f118-110">[searchHitsContainer](searchhitscontainer.md) collection</span></span>|<span data-ttu-id="7f118-111">Uma coleção de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7f118-111">A collection of search results.</span></span>|
|<span data-ttu-id="7f118-112">searchTerms</span><span class="sxs-lookup"><span data-stu-id="7f118-112">searchTerms</span></span>|<span data-ttu-id="7f118-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7f118-113">String collection</span></span>|<span data-ttu-id="7f118-114">Contém os termos de pesquisa enviados na consulta de pesquisa inicial.</span><span class="sxs-lookup"><span data-stu-id="7f118-114">Contains the search terms sent in the initial search query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f118-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f118-115">JSON representation</span></span>

<span data-ttu-id="7f118-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f118-116">The following is a JSON representation of the resource.</span></span>

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