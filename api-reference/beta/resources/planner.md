---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 8acc6d4d7ce6e91912f9fe5cb940967def8e1078
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094950"
---
# <a name="planner-resource-type"></a><span data-ttu-id="cc33d-105">tipo de recurso Planner</span><span class="sxs-lookup"><span data-stu-id="cc33d-105">planner resource type</span></span>

<span data-ttu-id="cc33d-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc33d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc33d-107">O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="cc33d-107">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="cc33d-108">Ele retorna um recurso **planejador** singleton.</span><span class="sxs-lookup"><span data-stu-id="cc33d-108">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="cc33d-109">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="cc33d-109">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="cc33d-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="cc33d-110">Methods</span></span>

| <span data-ttu-id="cc33d-111">Método</span><span class="sxs-lookup"><span data-stu-id="cc33d-111">Method</span></span>           | <span data-ttu-id="cc33d-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cc33d-112">Return Type</span></span>    |<span data-ttu-id="cc33d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc33d-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc33d-114">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="cc33d-114">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="cc33d-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="cc33d-115">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="cc33d-116">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="cc33d-116">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="cc33d-117">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cc33d-117">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="cc33d-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="cc33d-118">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="cc33d-119">Crie um novo **plannerPlan** postando na coleção Plans.</span><span class="sxs-lookup"><span data-stu-id="cc33d-119">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="cc33d-120">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="cc33d-120">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="cc33d-121">plannerTask</span><span class="sxs-lookup"><span data-stu-id="cc33d-121">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="cc33d-122">Crie um novo **plannerTask** postando na coleção Tasks.</span><span class="sxs-lookup"><span data-stu-id="cc33d-122">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc33d-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc33d-123">Properties</span></span>
| <span data-ttu-id="cc33d-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc33d-124">Property</span></span>     | <span data-ttu-id="cc33d-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc33d-125">Type</span></span>   |<span data-ttu-id="cc33d-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc33d-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc33d-127">id</span><span class="sxs-lookup"><span data-stu-id="cc33d-127">id</span></span>|<span data-ttu-id="cc33d-128">String</span><span class="sxs-lookup"><span data-stu-id="cc33d-128">String</span></span>| <span data-ttu-id="cc33d-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc33d-129">Read-only.</span></span> <span data-ttu-id="cc33d-130">Identificador do recurso **Planner** .</span><span class="sxs-lookup"><span data-stu-id="cc33d-130">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc33d-131">Relações</span><span class="sxs-lookup"><span data-stu-id="cc33d-131">Relationships</span></span>
| <span data-ttu-id="cc33d-132">Relação</span><span class="sxs-lookup"><span data-stu-id="cc33d-132">Relationship</span></span> | <span data-ttu-id="cc33d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc33d-133">Type</span></span>   |<span data-ttu-id="cc33d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc33d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc33d-135">buckets</span><span class="sxs-lookup"><span data-stu-id="cc33d-135">buckets</span></span>|<span data-ttu-id="cc33d-136">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="cc33d-136">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="cc33d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc33d-137">Read-only.</span></span> <span data-ttu-id="cc33d-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc33d-138">Nullable.</span></span> <span data-ttu-id="cc33d-139">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="cc33d-139">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="cc33d-140">Planeje</span><span class="sxs-lookup"><span data-stu-id="cc33d-140">plans</span></span>|<span data-ttu-id="cc33d-141">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="cc33d-141">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="cc33d-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc33d-142">Read-only.</span></span> <span data-ttu-id="cc33d-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc33d-143">Nullable.</span></span> <span data-ttu-id="cc33d-144">Retorna uma coleção de planos especificados</span><span class="sxs-lookup"><span data-stu-id="cc33d-144">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="cc33d-145">tarefas</span><span class="sxs-lookup"><span data-stu-id="cc33d-145">tasks</span></span>|<span data-ttu-id="cc33d-146">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="cc33d-146">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="cc33d-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc33d-147">Read-only.</span></span> <span data-ttu-id="cc33d-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cc33d-148">Nullable.</span></span> <span data-ttu-id="cc33d-149">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="cc33d-149">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc33d-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc33d-150">JSON representation</span></span>
<span data-ttu-id="cc33d-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc33d-151">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


