---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f6d25238436b79dec0397df1d005e67e6b17239a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462274"
---
# <a name="planner-resource-type"></a><span data-ttu-id="27bed-105">tipo de recurso Planner</span><span class="sxs-lookup"><span data-stu-id="27bed-105">planner resource type</span></span>

<span data-ttu-id="27bed-106">O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="27bed-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="27bed-107">Ele retorna um recurso **planejador** singleton.</span><span class="sxs-lookup"><span data-stu-id="27bed-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="27bed-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="27bed-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="27bed-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="27bed-109">Methods</span></span>

| <span data-ttu-id="27bed-110">Método</span><span class="sxs-lookup"><span data-stu-id="27bed-110">Method</span></span>           | <span data-ttu-id="27bed-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="27bed-111">Return Type</span></span>    |<span data-ttu-id="27bed-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="27bed-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="27bed-113">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="27bed-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="27bed-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="27bed-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="27bed-115">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="27bed-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="27bed-116">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="27bed-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="27bed-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="27bed-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="27bed-118">Crie um novo **plannerPlan** postando na coleção Plans.</span><span class="sxs-lookup"><span data-stu-id="27bed-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="27bed-119">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="27bed-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="27bed-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="27bed-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="27bed-121">Crie um novo **plannerTask** postando na coleção Tasks.</span><span class="sxs-lookup"><span data-stu-id="27bed-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27bed-122">Relações</span><span class="sxs-lookup"><span data-stu-id="27bed-122">Relationships</span></span>
| <span data-ttu-id="27bed-123">Relação</span><span class="sxs-lookup"><span data-stu-id="27bed-123">Relationship</span></span> | <span data-ttu-id="27bed-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="27bed-124">Type</span></span>   |<span data-ttu-id="27bed-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="27bed-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27bed-126">buckets</span><span class="sxs-lookup"><span data-stu-id="27bed-126">buckets</span></span>|<span data-ttu-id="27bed-127">coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="27bed-127">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="27bed-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27bed-128">Read-only.</span></span> <span data-ttu-id="27bed-129">Anulável.</span><span class="sxs-lookup"><span data-stu-id="27bed-129">Nullable.</span></span> <span data-ttu-id="27bed-130">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="27bed-130">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="27bed-131">Planeje</span><span class="sxs-lookup"><span data-stu-id="27bed-131">plans</span></span>|<span data-ttu-id="27bed-132">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="27bed-132">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="27bed-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27bed-133">Read-only.</span></span> <span data-ttu-id="27bed-134">Anulável.</span><span class="sxs-lookup"><span data-stu-id="27bed-134">Nullable.</span></span> <span data-ttu-id="27bed-135">Retorna uma coleção de planos especificados</span><span class="sxs-lookup"><span data-stu-id="27bed-135">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="27bed-136">tarefas</span><span class="sxs-lookup"><span data-stu-id="27bed-136">tasks</span></span>|<span data-ttu-id="27bed-137">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="27bed-137">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="27bed-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="27bed-138">Read-only.</span></span> <span data-ttu-id="27bed-139">Anulável.</span><span class="sxs-lookup"><span data-stu-id="27bed-139">Nullable.</span></span> <span data-ttu-id="27bed-140">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="27bed-140">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27bed-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="27bed-141">JSON representation</span></span>
<span data-ttu-id="27bed-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="27bed-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="27bed-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27bed-143">Example</span></span>

<span data-ttu-id="27bed-144">O recurso **Planner** está disponível na raiz do gráfico.</span><span class="sxs-lookup"><span data-stu-id="27bed-144">The **planner** resource is available at the root of the graph.</span></span>

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
