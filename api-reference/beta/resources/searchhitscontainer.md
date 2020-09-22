---
title: tipo de recurso searchHitsContainer
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d314fcdd2a62be5aea05bed3b2a9e1881f95c3d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985782"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="22a26-103">tipo de recurso searchHitsContainer</span><span class="sxs-lookup"><span data-stu-id="22a26-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="22a26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22a26-105">Representa a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="22a26-105">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="22a26-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22a26-106">Properties</span></span>

| <span data-ttu-id="22a26-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22a26-107">Property</span></span>     | <span data-ttu-id="22a26-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a26-108">Type</span></span>        | <span data-ttu-id="22a26-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a26-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22a26-110">falta</span><span class="sxs-lookup"><span data-stu-id="22a26-110">hits</span></span>|<span data-ttu-id="22a26-111">coleção [searchHit](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="22a26-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="22a26-112">Encasulate os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="22a26-112">Encasulate the Search results.</span></span>|
|<span data-ttu-id="22a26-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="22a26-113">moreResultsAvailable</span></span>|<span data-ttu-id="22a26-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a26-114">Boolean</span></span>|<span data-ttu-id="22a26-115">Fornece informações se mais resultados estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="22a26-115">Provides information if more results are available.</span></span> <span data-ttu-id="22a26-116">Nesse caso, você pode aumentar o deslocamento "de" e "para".</span><span class="sxs-lookup"><span data-stu-id="22a26-116">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="22a26-117">total</span><span class="sxs-lookup"><span data-stu-id="22a26-117">total</span></span>|<span data-ttu-id="22a26-118">Int32</span><span class="sxs-lookup"><span data-stu-id="22a26-118">Int32</span></span>|<span data-ttu-id="22a26-119">O número total de resultados.</span><span class="sxs-lookup"><span data-stu-id="22a26-119">The total number of results.</span></span> <span data-ttu-id="22a26-120">Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.</span><span class="sxs-lookup"><span data-stu-id="22a26-120">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22a26-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22a26-121">JSON representation</span></span>

<span data-ttu-id="22a26-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22a26-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHitsContainer",
  "baseType": null
}-->

```json
{
  "hits": [{"@odata.type": "microsoft.graph.searchHit"}],
  "moreResultsAvailable": true,
  "total": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHitsContainer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

