---
title: tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c140a30d4e77840b1fd7c7ccceec16e0554cd855
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193607"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="a87af-103">tipo de recurso searchHit</span><span class="sxs-lookup"><span data-stu-id="a87af-103">searchHit resource type</span></span>

<span data-ttu-id="a87af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a87af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="a87af-105">Representa um único resultado dentro da lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a87af-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="a87af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a87af-106">Properties</span></span>

| <span data-ttu-id="a87af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a87af-107">Property</span></span>     | <span data-ttu-id="a87af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a87af-108">Type</span></span>        | <span data-ttu-id="a87af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a87af-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a87af-110">hitId</span><span class="sxs-lookup"><span data-stu-id="a87af-110">hitId</span></span>|<span data-ttu-id="a87af-111">String</span><span class="sxs-lookup"><span data-stu-id="a87af-111">String</span></span>|<span data-ttu-id="a87af-112">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="a87af-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="a87af-113">classificação</span><span class="sxs-lookup"><span data-stu-id="a87af-113">rank</span></span>|<span data-ttu-id="a87af-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a87af-114">Int32</span></span>|<span data-ttu-id="a87af-115">A classificação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="a87af-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="a87af-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="a87af-116">contentSource</span></span>|<span data-ttu-id="a87af-117">String</span><span class="sxs-lookup"><span data-stu-id="a87af-117">String</span></span>|<span data-ttu-id="a87af-118">O nome da fonte de conteúdo da qual o **externalItem** faz parte.</span><span class="sxs-lookup"><span data-stu-id="a87af-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="a87af-119">summary</span><span class="sxs-lookup"><span data-stu-id="a87af-119">summary</span></span>|<span data-ttu-id="a87af-120">String</span><span class="sxs-lookup"><span data-stu-id="a87af-120">String</span></span>|<span data-ttu-id="a87af-121">Um resumo do resultado, se um resumo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="a87af-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="a87af-122">recurso</span><span class="sxs-lookup"><span data-stu-id="a87af-122">resource</span></span>|[<span data-ttu-id="a87af-123">entity</span><span class="sxs-lookup"><span data-stu-id="a87af-123">entity</span></span>](entity.md)|<span data-ttu-id="a87af-124">A representação subjacente do Microsoft Graph do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a87af-124">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="a87af-125">_id (preterido)</span><span class="sxs-lookup"><span data-stu-id="a87af-125">_id (deprecated)</span></span>|<span data-ttu-id="a87af-126">String</span><span class="sxs-lookup"><span data-stu-id="a87af-126">String</span></span>| <span data-ttu-id="a87af-127">Renomeado como **hitId**.</span><span class="sxs-lookup"><span data-stu-id="a87af-127">Renamed as **hitId**.</span></span> <span data-ttu-id="a87af-128">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="a87af-128">The internal identifier for the item.</span></span>|
|<span data-ttu-id="a87af-129">_score (preterido)</span><span class="sxs-lookup"><span data-stu-id="a87af-129">_score (deprecated)</span></span>|<span data-ttu-id="a87af-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a87af-130">Int32</span></span>|<span data-ttu-id="a87af-131">Renomeado como **classificação**.</span><span class="sxs-lookup"><span data-stu-id="a87af-131">Renamed as **rank**.</span></span> <span data-ttu-id="a87af-132">A pontuação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="a87af-132">The score or the order of the result.</span></span>|
|<span data-ttu-id="a87af-133">_summary (preterido)</span><span class="sxs-lookup"><span data-stu-id="a87af-133">_summary (deprecated)</span></span>|<span data-ttu-id="a87af-134">String</span><span class="sxs-lookup"><span data-stu-id="a87af-134">String</span></span>|<span data-ttu-id="a87af-135">Renomeado como **Resumo**.</span><span class="sxs-lookup"><span data-stu-id="a87af-135">Renamed as **summary**.</span></span> <span data-ttu-id="a87af-136">Um resumo do resultado (se o resumo estiver disponível).</span><span class="sxs-lookup"><span data-stu-id="a87af-136">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="a87af-137">_sortField (preterido)</span><span class="sxs-lookup"><span data-stu-id="a87af-137">_sortField (deprecated)</span></span>|<span data-ttu-id="a87af-138">String</span><span class="sxs-lookup"><span data-stu-id="a87af-138">String</span></span>|<span data-ttu-id="a87af-139">Essa propriedade foi removida.</span><span class="sxs-lookup"><span data-stu-id="a87af-139">This property has been removed.</span></span>|
|<span data-ttu-id="a87af-140">_source (preterido)</span><span class="sxs-lookup"><span data-stu-id="a87af-140">_source (deprecated)</span></span>|[<span data-ttu-id="a87af-141">entity</span><span class="sxs-lookup"><span data-stu-id="a87af-141">entity</span></span>](entity.md)|<span data-ttu-id="a87af-142">Renomeado como **recurso**.</span><span class="sxs-lookup"><span data-stu-id="a87af-142">Renamed as **resource**.</span></span> <span data-ttu-id="a87af-143">A representação de gráfico subjacente do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a87af-143">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a87af-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a87af-144">JSON representation</span></span>

<span data-ttu-id="a87af-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a87af-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
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

