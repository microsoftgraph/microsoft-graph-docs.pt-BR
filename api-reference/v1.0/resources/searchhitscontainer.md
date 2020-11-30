---
title: tipo de recurso searchHitsContainer
description: Representa a lista de resultados de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f32fa198624c04da6eadfc828b60350164cbdddc
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377982"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="52e72-103">tipo de recurso searchHitsContainer</span><span class="sxs-lookup"><span data-stu-id="52e72-103">searchHitsContainer resource type</span></span>

<span data-ttu-id="52e72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52e72-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="52e72-105">Representa a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52e72-105">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="52e72-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52e72-106">Properties</span></span>

| <span data-ttu-id="52e72-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52e72-107">Property</span></span>     | <span data-ttu-id="52e72-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="52e72-108">Type</span></span>        | <span data-ttu-id="52e72-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52e72-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52e72-110">falta</span><span class="sxs-lookup"><span data-stu-id="52e72-110">hits</span></span>|<span data-ttu-id="52e72-111">coleção [searchHit](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="52e72-111">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="52e72-112">Uma coleção dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="52e72-112">A collection of the search results.</span></span>|
|<span data-ttu-id="52e72-113">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="52e72-113">moreResultsAvailable</span></span>|<span data-ttu-id="52e72-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e72-114">Boolean</span></span>|<span data-ttu-id="52e72-115">Fornece informações se mais resultados estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="52e72-115">Provides information if more results are available.</span></span> <span data-ttu-id="52e72-116">Com base nessas informações, você pode ajustar as propriedades **from** e **size** do [searchRequest](searchrequest.md) adequadamente.</span><span class="sxs-lookup"><span data-stu-id="52e72-116">Based on this information, you can adjust the **from** and **size** properties of the [searchRequest](searchrequest.md) accordingly.</span></span>|
|<span data-ttu-id="52e72-117">total</span><span class="sxs-lookup"><span data-stu-id="52e72-117">total</span></span>|<span data-ttu-id="52e72-118">Int32</span><span class="sxs-lookup"><span data-stu-id="52e72-118">Int32</span></span>|<span data-ttu-id="52e72-119">O número total de resultados.</span><span class="sxs-lookup"><span data-stu-id="52e72-119">The total number of results.</span></span> <span data-ttu-id="52e72-120">Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.</span><span class="sxs-lookup"><span data-stu-id="52e72-120">Note this is not the number of results on the page, but the total number of results satisfying the query.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="52e72-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52e72-121">JSON representation</span></span>

<span data-ttu-id="52e72-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52e72-122">The following is a JSON representation of the resource.</span></span>

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


