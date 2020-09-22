---
title: tipo de recurso searchHit
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3d010f3731fa65e1ab2dc3abbf84ffdc5ebdb732
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985773"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="10ae4-103">tipo de recurso searchHit</span><span class="sxs-lookup"><span data-stu-id="10ae4-103">searchHit resource type</span></span>

<span data-ttu-id="10ae4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ae4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10ae4-105">Representa um único resultado dentro da lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="10ae4-105">Represent a single result within the list of search results.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="10ae4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10ae4-106">Properties</span></span>

| <span data-ttu-id="10ae4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10ae4-107">Property</span></span>     | <span data-ttu-id="10ae4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="10ae4-108">Type</span></span>        | <span data-ttu-id="10ae4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10ae4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10ae4-110">_id</span><span class="sxs-lookup"><span data-stu-id="10ae4-110">_id</span></span>|<span data-ttu-id="10ae4-111">String</span><span class="sxs-lookup"><span data-stu-id="10ae4-111">String</span></span>|<span data-ttu-id="10ae4-112">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="10ae4-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="10ae4-113">_score</span><span class="sxs-lookup"><span data-stu-id="10ae4-113">_score</span></span>|<span data-ttu-id="10ae4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="10ae4-114">Int32</span></span>|<span data-ttu-id="10ae4-115">A pontuação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="10ae4-115">The score or the order of the result.</span></span>|
|<span data-ttu-id="10ae4-116">_sortField</span><span class="sxs-lookup"><span data-stu-id="10ae4-116">_sortField</span></span>|<span data-ttu-id="10ae4-117">String</span><span class="sxs-lookup"><span data-stu-id="10ae4-117">String</span></span>|<span data-ttu-id="10ae4-118">A ordem de classificação usada.</span><span class="sxs-lookup"><span data-stu-id="10ae4-118">The sort order used.</span></span> <span data-ttu-id="10ae4-119">Pode ser DateTime ou relevância.</span><span class="sxs-lookup"><span data-stu-id="10ae4-119">It can be DateTime or Relevance.</span></span>|
|<span data-ttu-id="10ae4-120">_summary</span><span class="sxs-lookup"><span data-stu-id="10ae4-120">_summary</span></span>|<span data-ttu-id="10ae4-121">String</span><span class="sxs-lookup"><span data-stu-id="10ae4-121">String</span></span>|<span data-ttu-id="10ae4-122">Um resumo do resultado (se o resumo estiver disponível).</span><span class="sxs-lookup"><span data-stu-id="10ae4-122">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="10ae4-123">_source</span><span class="sxs-lookup"><span data-stu-id="10ae4-123">_source</span></span>|[<span data-ttu-id="10ae4-124">entity</span><span class="sxs-lookup"><span data-stu-id="10ae4-124">entity</span></span>](entity.md)|<span data-ttu-id="10ae4-125">A representação de gráfico subjacente do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="10ae4-125">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10ae4-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10ae4-126">JSON representation</span></span>

<span data-ttu-id="10ae4-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10ae4-127">The following is a JSON representation of the resource.</span></span>

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

