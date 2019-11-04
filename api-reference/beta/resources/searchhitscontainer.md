---
title: tipo de recurso searchHitsContainer
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7bc36dc49a944de4a12decbf3b0b77a3c203eb21
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938713"
---
# <a name="searchhitscontainer-resource-type"></a><span data-ttu-id="08e5f-103">tipo de recurso searchHitsContainer</span><span class="sxs-lookup"><span data-stu-id="08e5f-103">searchHitsContainer resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08e5f-104">Representa a lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="08e5f-104">Represent the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="08e5f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08e5f-105">Properties</span></span>

| <span data-ttu-id="08e5f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08e5f-106">Property</span></span>     | <span data-ttu-id="08e5f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="08e5f-107">Type</span></span>        | <span data-ttu-id="08e5f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="08e5f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08e5f-109">falta</span><span class="sxs-lookup"><span data-stu-id="08e5f-109">hits</span></span>|<span data-ttu-id="08e5f-110">coleção [searchHit](searchhit.md)</span><span class="sxs-lookup"><span data-stu-id="08e5f-110">[searchHit](searchhit.md) collection</span></span>|<span data-ttu-id="08e5f-111">Encasulate os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="08e5f-111">Encasulate the Search results.</span></span>|
|<span data-ttu-id="08e5f-112">moreResultsAvailable</span><span class="sxs-lookup"><span data-stu-id="08e5f-112">moreResultsAvailable</span></span>|<span data-ttu-id="08e5f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="08e5f-113">Boolean</span></span>|<span data-ttu-id="08e5f-114">Fornece informações se mais resultados estiverem disponíveis.</span><span class="sxs-lookup"><span data-stu-id="08e5f-114">Provides information if more results are available.</span></span> <span data-ttu-id="08e5f-115">Nesse caso, você pode aumentar o deslocamento "de" e "para".</span><span class="sxs-lookup"><span data-stu-id="08e5f-115">In that case you can increase the "from" and "to" offset.</span></span>|
|<span data-ttu-id="08e5f-116">total</span><span class="sxs-lookup"><span data-stu-id="08e5f-116">total</span></span>|<span data-ttu-id="08e5f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="08e5f-117">Int32</span></span>|<span data-ttu-id="08e5f-118">O número total de resultados.</span><span class="sxs-lookup"><span data-stu-id="08e5f-118">The total number of results.</span></span> <span data-ttu-id="08e5f-119">Observação Este não é o número de resultados na página, mas o número total de resultados que atendem à consulta.</span><span class="sxs-lookup"><span data-stu-id="08e5f-119">Note this is not the number on results in the page, but the total number of results satisfying the query.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08e5f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08e5f-120">JSON representation</span></span>

<span data-ttu-id="08e5f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08e5f-121">The following is a JSON representation of the resource.</span></span>

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