---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ef94a7507558279e5295239588e2a8eda512882
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009129"
---
# <a name="planner-resource-type"></a><span data-ttu-id="eb370-105">tipo de recurso Planner</span><span class="sxs-lookup"><span data-stu-id="eb370-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb370-106">O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="eb370-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="eb370-107">Ele retorna um recurso **planejador** singleton.</span><span class="sxs-lookup"><span data-stu-id="eb370-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="eb370-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="eb370-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="eb370-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb370-109">Methods</span></span>

| <span data-ttu-id="eb370-110">Método</span><span class="sxs-lookup"><span data-stu-id="eb370-110">Method</span></span>           | <span data-ttu-id="eb370-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb370-111">Return Type</span></span>    |<span data-ttu-id="eb370-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb370-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eb370-113">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="eb370-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="eb370-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="eb370-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="eb370-115">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="eb370-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="eb370-116">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="eb370-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="eb370-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="eb370-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="eb370-118">Crie um novo **plannerPlan** postando na coleção Plans.</span><span class="sxs-lookup"><span data-stu-id="eb370-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="eb370-119">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="eb370-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="eb370-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="eb370-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="eb370-121">Crie um novo **plannerTask** postando na coleção Tasks.</span><span class="sxs-lookup"><span data-stu-id="eb370-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb370-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb370-122">Properties</span></span>
| <span data-ttu-id="eb370-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb370-123">Property</span></span>     | <span data-ttu-id="eb370-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb370-124">Type</span></span>   |<span data-ttu-id="eb370-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb370-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb370-126">id</span><span class="sxs-lookup"><span data-stu-id="eb370-126">id</span></span>|<span data-ttu-id="eb370-127">String</span><span class="sxs-lookup"><span data-stu-id="eb370-127">String</span></span>| <span data-ttu-id="eb370-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb370-128">Read-only.</span></span> <span data-ttu-id="eb370-129">Identificador do recurso **Planner** .</span><span class="sxs-lookup"><span data-stu-id="eb370-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb370-130">Relações</span><span class="sxs-lookup"><span data-stu-id="eb370-130">Relationships</span></span>
| <span data-ttu-id="eb370-131">Relação</span><span class="sxs-lookup"><span data-stu-id="eb370-131">Relationship</span></span> | <span data-ttu-id="eb370-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb370-132">Type</span></span>   |<span data-ttu-id="eb370-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb370-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb370-134">buckets</span><span class="sxs-lookup"><span data-stu-id="eb370-134">buckets</span></span>|<span data-ttu-id="eb370-135">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="eb370-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="eb370-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb370-136">Read-only.</span></span> <span data-ttu-id="eb370-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eb370-137">Nullable.</span></span> <span data-ttu-id="eb370-138">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="eb370-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="eb370-139">Planeje</span><span class="sxs-lookup"><span data-stu-id="eb370-139">plans</span></span>|<span data-ttu-id="eb370-140">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="eb370-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="eb370-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb370-141">Read-only.</span></span> <span data-ttu-id="eb370-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eb370-142">Nullable.</span></span> <span data-ttu-id="eb370-143">Retorna uma coleção de planos especificados</span><span class="sxs-lookup"><span data-stu-id="eb370-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="eb370-144">tarefas</span><span class="sxs-lookup"><span data-stu-id="eb370-144">tasks</span></span>|<span data-ttu-id="eb370-145">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="eb370-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="eb370-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb370-146">Read-only.</span></span> <span data-ttu-id="eb370-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eb370-147">Nullable.</span></span> <span data-ttu-id="eb370-148">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="eb370-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb370-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb370-149">JSON representation</span></span>
<span data-ttu-id="eb370-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb370-150">Here is a JSON representation of the resource.</span></span>

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
