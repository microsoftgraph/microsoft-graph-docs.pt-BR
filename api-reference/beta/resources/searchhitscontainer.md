---
title: tipo de recurso searchHitsContainer
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 750bd79dad9758f3ffe883fd87713c42c29c0917
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520918"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="04000-103">tipo de recurso searchHitsContainer</span><span class="sxs-lookup"><span data-stu-id="04000-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="04000-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="04000-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04000-105">Representa a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="04000-105">Represent the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="04000-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04000-106">Properties</span></span>

| <span data-ttu-id="04000-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04000-107">Property</span></span>     | <span data-ttu-id="04000-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="04000-108">Type</span></span>        | <span data-ttu-id="04000-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="04000-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="04000-110">falta</span><span class="sxs-lookup"><span data-stu-id="04000-110">hits</span></span>|<span data-ttu-id="04000-111">coleção [searchHit](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="04000-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="04000-112">Encasulate os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="04000-112">Encasulate the Search results.</span></span>|
|<span data-ttu-id="04000-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="04000-113">moreResultsAvailable</span></span>|<span data-ttu-id="04000-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="04000-114">Boolean</span></span>|<span data-ttu-id="04000-115">Fornece informações se mais resultados estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="04000-115">Provides information if more results are available.</span></span> <span data-ttu-id="04000-116">Nesse caso, você pode aumentar o deslocamento "de" e "para".</span><span class="sxs-lookup"><span data-stu-id="04000-116">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="04000-117">total</span><span class="sxs-lookup"><span data-stu-id="04000-117">total</span></span>|<span data-ttu-id="04000-118">Int32</span><span class="sxs-lookup"><span data-stu-id="04000-118">Int32</span></span>|<span data-ttu-id="04000-119">O número total de resultados.</span><span class="sxs-lookup"><span data-stu-id="04000-119">The total number of results.</span></span> <span data-ttu-id="04000-120">Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.</span><span class="sxs-lookup"><span data-stu-id="04000-120">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04000-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04000-121">JSON representation</span></span>

<span data-ttu-id="04000-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04000-122">The following is a JSON representation of the resource.</span></span>

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