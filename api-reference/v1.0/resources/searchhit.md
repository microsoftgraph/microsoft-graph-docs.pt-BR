---
title: tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bad671657e46068263d3386eb0bb04026cfaa28e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377954"
---
# <a name="searchhit-resource-type"></a><span data-ttu-id="fc52e-103">tipo de recurso searchHit</span><span class="sxs-lookup"><span data-stu-id="fc52e-103">searchHit resource type</span></span>

<span data-ttu-id="fc52e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc52e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc52e-105">Representa um único resultado dentro da lista de resultados de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fc52e-105">Represents a single result within the list of search results.</span></span>

## <a name="properties"></a><span data-ttu-id="fc52e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc52e-106">Properties</span></span>

| <span data-ttu-id="fc52e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc52e-107">Property</span></span>     | <span data-ttu-id="fc52e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc52e-108">Type</span></span>        | <span data-ttu-id="fc52e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc52e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc52e-110">hitId</span><span class="sxs-lookup"><span data-stu-id="fc52e-110">hitId</span></span>|<span data-ttu-id="fc52e-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fc52e-111">String</span></span>|<span data-ttu-id="fc52e-112">O identificador interno do item.</span><span class="sxs-lookup"><span data-stu-id="fc52e-112">The internal identifier for the item.</span></span>|
|<span data-ttu-id="fc52e-113">classificação</span><span class="sxs-lookup"><span data-stu-id="fc52e-113">rank</span></span>|<span data-ttu-id="fc52e-114">Int32</span><span class="sxs-lookup"><span data-stu-id="fc52e-114">Int32</span></span>|<span data-ttu-id="fc52e-115">A classificação ou a ordem do resultado.</span><span class="sxs-lookup"><span data-stu-id="fc52e-115">The rank or the order of the result.</span></span>|
|<span data-ttu-id="fc52e-116">contentSource</span><span class="sxs-lookup"><span data-stu-id="fc52e-116">contentSource</span></span>|<span data-ttu-id="fc52e-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fc52e-117">String</span></span>|<span data-ttu-id="fc52e-118">O nome da fonte de conteúdo da qual o **externalItem** faz parte.</span><span class="sxs-lookup"><span data-stu-id="fc52e-118">The name of the content source which the **externalItem** is part of .</span></span>|
|<span data-ttu-id="fc52e-119">summary</span><span class="sxs-lookup"><span data-stu-id="fc52e-119">summary</span></span>|<span data-ttu-id="fc52e-120">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="fc52e-120">String</span></span>|<span data-ttu-id="fc52e-121">Um resumo do resultado, se um resumo estiver disponível.</span><span class="sxs-lookup"><span data-stu-id="fc52e-121">A summary of the result, if a summary is available.</span></span>|
|<span data-ttu-id="fc52e-122">recurso</span><span class="sxs-lookup"><span data-stu-id="fc52e-122">resource</span></span>|[<span data-ttu-id="fc52e-123">entity</span><span class="sxs-lookup"><span data-stu-id="fc52e-123">entity</span></span>](entity.md)|<span data-ttu-id="fc52e-124">A representação subjacente do Microsoft Graph do resultado da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fc52e-124">The underlying Microsoft Graph representation of the search result.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc52e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc52e-125">JSON representation</span></span>

<span data-ttu-id="fc52e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc52e-126">The following is a JSON representation of the resource.</span></span>

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
  "resource": { "@odata.type": "microsoft.graph.entity" }
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

