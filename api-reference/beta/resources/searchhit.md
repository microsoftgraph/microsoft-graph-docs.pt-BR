---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210329"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="c85a4-103">Tipo de recurso searchHit</span><span class="sxs-lookup"><span data-stu-id="c85a4-103">searchHit resource type</span></span>

<span data-ttu-id="c85a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c85a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

<span data-ttu-id="c85a4-105">Representa um único resultado na lista de resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c85a4-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="c85a4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c85a4-106">Properties</span></span>

| <span data-ttu-id="c85a4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c85a4-107">Property</span></span>     | <span data-ttu-id="c85a4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c85a4-108">Type</span></span>        | <span data-ttu-id="c85a4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c85a4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c85a4-110">hitId</span><span class="sxs-lookup"><span data-stu-id="c85a4-110">hitId</span></span>|<span data-ttu-id="c85a4-111">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-111">String</span></span>|<span data-ttu-id="c85a4-112">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="c85a4-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="c85a4-113">classificação</span><span class="sxs-lookup"><span data-stu-id="c85a4-113">rank</span></span>|<span data-ttu-id="c85a4-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c85a4-114">Int32</span></span>|<span data-ttu-id="c85a4-115">A classificação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="c85a4-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="c85a4-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="c85a4-116">contentSource</span></span>|<span data-ttu-id="c85a4-117">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-117">String</span></span>|<span data-ttu-id="c85a4-118">O nome da fonte de conteúdo da **qual o externalItem** faz parte .</span><span class="sxs-lookup"><span data-stu-id="c85a4-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="c85a4-119">summary</span><span class="sxs-lookup"><span data-stu-id="c85a4-119">summary</span></span>|<span data-ttu-id="c85a4-120">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-120">String</span></span>|<span data-ttu-id="c85a4-121">Um resumo do resultado, se um resumo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="c85a4-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="c85a4-122">resultTemplateId</span><span class="sxs-lookup"><span data-stu-id="c85a4-122">resultTemplateId</span></span>|<span data-ttu-id="c85a4-123">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-123">String</span></span>|<span data-ttu-id="c85a4-124">ID do modelo de resultado para renderizar o resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c85a4-124">ID of the result template for rendering the search result.</span></span> <span data-ttu-id="c85a4-125">Essa ID deve mapear para um layout de exibição no dicionário **resultTemplates,** incluído também na [pesquisaresponse.](searchresponse.md)</span><span class="sxs-lookup"><span data-stu-id="c85a4-125">This ID must map to a display layout in the **resultTemplates** dictionary, included in the [searchresponse](searchresponse.md) as well.</span></span>|
|<span data-ttu-id="c85a4-126">recurso</span><span class="sxs-lookup"><span data-stu-id="c85a4-126">resource</span></span>|[<span data-ttu-id="c85a4-127">entity</span><span class="sxs-lookup"><span data-stu-id="c85a4-127">entity</span></span>](entity.md)|<span data-ttu-id="c85a4-128">A representação básica da Microsoft Graph do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c85a4-128">The underlying Microsoft Graph representation of the search result.</span></span>|
|<span data-ttu-id="c85a4-129">_id (preterido)</span><span class="sxs-lookup"><span data-stu-id="c85a4-129">_id (deprecated)</span></span>|<span data-ttu-id="c85a4-130">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-130">String</span></span>| <span data-ttu-id="c85a4-131">Renomeado como **hitId**.</span><span class="sxs-lookup"><span data-stu-id="c85a4-131">Renamed as **hitId**.</span></span> <span data-ttu-id="c85a4-132">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="c85a4-132">The internal identifier for the item.</span></span>|
|<span data-ttu-id="c85a4-133">_score (preterido)</span><span class="sxs-lookup"><span data-stu-id="c85a4-133">_score (deprecated)</span></span>|<span data-ttu-id="c85a4-134">Int32</span><span class="sxs-lookup"><span data-stu-id="c85a4-134">Int32</span></span>|<span data-ttu-id="c85a4-135">Renomeado como **classificação**.</span><span class="sxs-lookup"><span data-stu-id="c85a4-135">Renamed as **rank**.</span></span> <span data-ttu-id="c85a4-136">A pontuação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="c85a4-136">The score or the order of the result.</span></span>|
|<span data-ttu-id="c85a4-137">_summary (preterido)</span><span class="sxs-lookup"><span data-stu-id="c85a4-137">_summary (deprecated)</span></span>|<span data-ttu-id="c85a4-138">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-138">String</span></span>|<span data-ttu-id="c85a4-139">Renomeado como **resumo**.</span><span class="sxs-lookup"><span data-stu-id="c85a4-139">Renamed as **summary**.</span></span> <span data-ttu-id="c85a4-140">Um resumo do resultado (se o resumo estiver disponível).</span><span class="sxs-lookup"><span data-stu-id="c85a4-140">A summary of the result (if summary is available).</span></span>|
|<span data-ttu-id="c85a4-141">_sortField (preterido)</span><span class="sxs-lookup"><span data-stu-id="c85a4-141">_sortField (deprecated)</span></span>|<span data-ttu-id="c85a4-142">String</span><span class="sxs-lookup"><span data-stu-id="c85a4-142">String</span></span>|<span data-ttu-id="c85a4-143">Essa propriedade foi removida.</span><span class="sxs-lookup"><span data-stu-id="c85a4-143">This property has been removed.</span></span>|
|<span data-ttu-id="c85a4-144">_source (preterido)</span><span class="sxs-lookup"><span data-stu-id="c85a4-144">_source (deprecated)</span></span>|[<span data-ttu-id="c85a4-145">entity</span><span class="sxs-lookup"><span data-stu-id="c85a4-145">entity</span></span>](entity.md)|<span data-ttu-id="c85a4-146">Renomeado como **recurso**.</span><span class="sxs-lookup"><span data-stu-id="c85a4-146">Renamed as **resource**.</span></span> <span data-ttu-id="c85a4-147">A representação Graph base do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c85a4-147">The underlying Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c85a4-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c85a4-148">JSON representation</span></span>

<span data-ttu-id="c85a4-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c85a4-149">The following is a JSON representation of the resource.</span></span>

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
  "resultTemplateId": "String",
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

