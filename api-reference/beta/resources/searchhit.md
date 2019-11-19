---
title: tipo de recurso searchHit
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 787ecfeaefc7e5b140dc6338195af7d58e1a8ccd
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703916"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="8d049-103">tipo de recurso searchHit</span><span class="sxs-lookup"><span data-stu-id="8d049-103">searchHit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d049-104">Representa um único resultado dentro da lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8d049-104">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="8d049-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d049-105">Properties</span></span>

| <span data-ttu-id="8d049-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d049-106">Property</span></span>     | <span data-ttu-id="8d049-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d049-107">Type</span></span>        | <span data-ttu-id="8d049-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d049-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d049-109">_id</span><span class="sxs-lookup"><span data-stu-id="8d049-109">_id</span></span>|<span data-ttu-id="8d049-110">String</span><span class="sxs-lookup"><span data-stu-id="8d049-110">String</span></span>|<span data-ttu-id="8d049-111">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="8d049-111">The internal identifier for the item.</span></span>|
|<span data-ttu-id="8d049-112">_score</span><span class="sxs-lookup"><span data-stu-id="8d049-112">_score</span></span>|<span data-ttu-id="8d049-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8d049-113">Int32</span></span>|<span data-ttu-id="8d049-114">A pontuação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="8d049-114">The score or the order of the result.</span></span>|
|<span data-ttu-id="8d049-115">_sortField</span><span class="sxs-lookup"><span data-stu-id="8d049-115">_sortField</span></span>|<span data-ttu-id="8d049-116">String</span><span class="sxs-lookup"><span data-stu-id="8d049-116">String</span></span>|<span data-ttu-id="8d049-117">A ordem de classificação usada.</span><span class="sxs-lookup"><span data-stu-id="8d049-117">The sort order used.</span></span> <span data-ttu-id="8d049-118">Pode ser DateTime ou relevância.</span><span class="sxs-lookup"><span data-stu-id="8d049-118">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="8d049-119">_summary</span><span class="sxs-lookup"><span data-stu-id="8d049-119">_summary</span></span>|<span data-ttu-id="8d049-120">String</span><span class="sxs-lookup"><span data-stu-id="8d049-120">String</span></span>|<span data-ttu-id="8d049-121">Um resumo do resultado (se o resumo estiver disponível).</span><span class="sxs-lookup"><span data-stu-id="8d049-121">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="8d049-122">_source</span><span class="sxs-lookup"><span data-stu-id="8d049-122">_source</span></span>|[<span data-ttu-id="8d049-123">entity</span><span class="sxs-lookup"><span data-stu-id="8d049-123">entity</span></span>](entity.md)|<span data-ttu-id="8d049-124">A representação de gráfico subjacente do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8d049-124">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d049-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d049-125">JSON representation</span></span>

<span data-ttu-id="8d049-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d049-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->