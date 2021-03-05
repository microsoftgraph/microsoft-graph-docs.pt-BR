---
title: Tipo de recurso do planner
description: O **recurso** planner é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso de **planejador de singleton.**  Ele não contém propriedades usáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8fc5f91dd8da85b259dd792a0926311d57098ee9
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470673"
---
# <a name="planner-resource-type"></a><span data-ttu-id="25625-105">Tipo de recurso do planner</span><span class="sxs-lookup"><span data-stu-id="25625-105">planner resource type</span></span>

<span data-ttu-id="25625-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25625-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="25625-107">O **recurso** planner é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="25625-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="25625-108">Ele retorna um recurso de **planejador de singleton.**</span><span class="sxs-lookup"><span data-stu-id="25625-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="25625-109">Ele não contém propriedades usáveis.</span><span class="sxs-lookup"><span data-stu-id="25625-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="25625-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="25625-110">Methods</span></span>

| <span data-ttu-id="25625-111">Método</span><span class="sxs-lookup"><span data-stu-id="25625-111">Method</span></span>           | <span data-ttu-id="25625-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25625-112">Return Type</span></span>    |<span data-ttu-id="25625-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="25625-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25625-114">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="25625-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="25625-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="25625-115">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="25625-116">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="25625-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="25625-117">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="25625-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="25625-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="25625-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="25625-119">Crie um novo **plannerPlan** postando na coleção plans.</span><span class="sxs-lookup"><span data-stu-id="25625-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="25625-120">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="25625-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="25625-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="25625-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="25625-122">Crie um novo **plannerTask** postando na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="25625-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25625-123">Relações</span><span class="sxs-lookup"><span data-stu-id="25625-123">Relationships</span></span>
| <span data-ttu-id="25625-124">Relação</span><span class="sxs-lookup"><span data-stu-id="25625-124">Relationship</span></span> | <span data-ttu-id="25625-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="25625-125">Type</span></span>   |<span data-ttu-id="25625-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="25625-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25625-127">buckets</span><span class="sxs-lookup"><span data-stu-id="25625-127">buckets</span></span>|<span data-ttu-id="25625-128">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="25625-128">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="25625-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25625-129">Read-only.</span></span> <span data-ttu-id="25625-130">Anulável.</span><span class="sxs-lookup"><span data-stu-id="25625-130">Nullable.</span></span> <span data-ttu-id="25625-131">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="25625-131">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="25625-132">plans</span><span class="sxs-lookup"><span data-stu-id="25625-132">plans</span></span>|<span data-ttu-id="25625-133">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="25625-133">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="25625-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25625-134">Read-only.</span></span> <span data-ttu-id="25625-135">Anulável.</span><span class="sxs-lookup"><span data-stu-id="25625-135">Nullable.</span></span> <span data-ttu-id="25625-136">Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="25625-136">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="25625-137">tarefas</span><span class="sxs-lookup"><span data-stu-id="25625-137">tasks</span></span>|<span data-ttu-id="25625-138">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="25625-138">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="25625-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25625-139">Read-only.</span></span> <span data-ttu-id="25625-140">Anulável.</span><span class="sxs-lookup"><span data-stu-id="25625-140">Nullable.</span></span> <span data-ttu-id="25625-141">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="25625-141">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25625-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25625-142">JSON representation</span></span>
<span data-ttu-id="25625-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25625-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="25625-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25625-144">Example</span></span>

<span data-ttu-id="25625-145">O **recurso** planner está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="25625-145">The **planner** resource is available at the root of the graph.</span></span>

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
```http
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

