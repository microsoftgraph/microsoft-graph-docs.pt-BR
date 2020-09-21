---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: f8333596ee93a42db8eded49815059e8633bf3db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037630"
---
# <a name="planner-resource-type"></a><span data-ttu-id="17926-105">tipo de recurso Planner</span><span class="sxs-lookup"><span data-stu-id="17926-105">planner resource type</span></span>

<span data-ttu-id="17926-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17926-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17926-107">O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="17926-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="17926-108">Ele retorna um recurso **planejador** singleton.</span><span class="sxs-lookup"><span data-stu-id="17926-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="17926-109">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="17926-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="17926-110">Methods</span><span class="sxs-lookup"><span data-stu-id="17926-110">Methods</span></span>

| <span data-ttu-id="17926-111">Método</span><span class="sxs-lookup"><span data-stu-id="17926-111">Method</span></span>           | <span data-ttu-id="17926-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17926-112">Return Type</span></span>    |<span data-ttu-id="17926-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="17926-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17926-114">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="17926-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="17926-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="17926-115">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="17926-116">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="17926-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="17926-117">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="17926-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="17926-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="17926-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="17926-119">Crie um novo **plannerPlan** postando na coleção Plans.</span><span class="sxs-lookup"><span data-stu-id="17926-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="17926-120">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="17926-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="17926-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="17926-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="17926-122">Crie um novo **plannerTask** postando na coleção Tasks.</span><span class="sxs-lookup"><span data-stu-id="17926-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17926-123">Relações</span><span class="sxs-lookup"><span data-stu-id="17926-123">Relationships</span></span>
| <span data-ttu-id="17926-124">Relação</span><span class="sxs-lookup"><span data-stu-id="17926-124">Relationship</span></span> | <span data-ttu-id="17926-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="17926-125">Type</span></span>   |<span data-ttu-id="17926-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="17926-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17926-127">buckets</span><span class="sxs-lookup"><span data-stu-id="17926-127">buckets</span></span>|<span data-ttu-id="17926-128">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="17926-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="17926-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17926-129">Read-only.</span></span> <span data-ttu-id="17926-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="17926-130">Nullable.</span></span> <span data-ttu-id="17926-131">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="17926-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="17926-132">Planeje</span><span class="sxs-lookup"><span data-stu-id="17926-132">plans</span></span>|<span data-ttu-id="17926-133">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="17926-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="17926-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17926-134">Read-only.</span></span> <span data-ttu-id="17926-135">Anulável.</span><span class="sxs-lookup"><span data-stu-id="17926-135">Nullable.</span></span> <span data-ttu-id="17926-136">Retorna uma coleção de planos especificados</span><span class="sxs-lookup"><span data-stu-id="17926-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="17926-137">tarefas</span><span class="sxs-lookup"><span data-stu-id="17926-137">tasks</span></span>|<span data-ttu-id="17926-138">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="17926-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="17926-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="17926-139">Read-only.</span></span> <span data-ttu-id="17926-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="17926-140">Nullable.</span></span> <span data-ttu-id="17926-141">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="17926-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17926-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17926-142">JSON representation</span></span>
<span data-ttu-id="17926-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17926-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="17926-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17926-144">Example</span></span>

<span data-ttu-id="17926-145">O recurso **Planner** está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="17926-145">The **planner** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.planner"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

