---
title: tipo de recurso searchHitsContainer
description: Representa a lista de resultados de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a2d120722179cb0fd771a84f867948a7fbfffdd4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192781"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="2ee79-103">tipo de recurso searchHitsContainer</span><span class="sxs-lookup"><span data-stu-id="2ee79-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="2ee79-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ee79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ee79-105">Representa a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2ee79-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="2ee79-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ee79-106">Properties</span></span>

| <span data-ttu-id="2ee79-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ee79-107">Property</span></span>     | <span data-ttu-id="2ee79-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ee79-108">Type</span></span>        | <span data-ttu-id="2ee79-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ee79-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ee79-110">falta</span><span class="sxs-lookup"><span data-stu-id="2ee79-110">hits</span></span>|<span data-ttu-id="2ee79-111">coleção [searchHit](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="2ee79-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="2ee79-112">Uma coleção dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2ee79-112">A collection of the search results.</span></span>|
|<span data-ttu-id="2ee79-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="2ee79-113">moreResultsAvailable</span></span>|<span data-ttu-id="2ee79-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ee79-114">Boolean</span></span>|<span data-ttu-id="2ee79-115">Fornece informações se mais resultados estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="2ee79-115">Provides information if more results are available.</span></span> <span data-ttu-id="2ee79-116">Com base nessas informações, você pode ajustar as propriedades **from** e **size** do [searchRequest](searchrequest.md) adequadamente.</span><span class="sxs-lookup"><span data-stu-id="2ee79-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="2ee79-117">total</span><span class="sxs-lookup"><span data-stu-id="2ee79-117">total</span></span>|<span data-ttu-id="2ee79-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2ee79-118">Int32</span></span>|<span data-ttu-id="2ee79-119">O número total de resultados.</span><span class="sxs-lookup"><span data-stu-id="2ee79-119">The total number of results.</span></span> <span data-ttu-id="2ee79-120">Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.</span><span class="sxs-lookup"><span data-stu-id="2ee79-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|
|<span data-ttu-id="2ee79-121">Aggregations</span><span class="sxs-lookup"><span data-stu-id="2ee79-121">aggregations</span></span>|<span data-ttu-id="2ee79-122">coleção [searchAggregation](searchaggregation.md)</span><span class="sxs-lookup"><span data-stu-id="2ee79-122">[searchAggregation](searchaggregation.md) collection</span></span>|<span data-ttu-id="2ee79-123">Contém a coleção de agregações computadas com base no [aggregationOption](aggregationoption.md) fornecido especificado na solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ee79-123">Contains the collection of aggregations computed based on the provided [aggregationOption](aggregationoption.md) specified in the request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ee79-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ee79-124">JSON representation</span></span>

<span data-ttu-id="2ee79-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ee79-125">The following is a JSON representation of the resource.</span></span>

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
  "total": 1024,
  "aggregations": [{"@odata.type": "microsoft.graph.searchAggregation"}]
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


