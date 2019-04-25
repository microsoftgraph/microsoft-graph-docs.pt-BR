---
title: tipo de recurso Planner
description: O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner. Ele retorna um recurso **planejador** singleton.  Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579244"
---
# <a name="planner-resource-type"></a><span data-ttu-id="d98d7-105">tipo de recurso Planner</span><span class="sxs-lookup"><span data-stu-id="d98d7-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d98d7-106">O recurso **Planner** é o ponto de entrada para o modelo de objeto do Planner.</span><span class="sxs-lookup"><span data-stu-id="d98d7-106">The **planner** resource is the entry point for the Planner object model.</span></span> <span data-ttu-id="d98d7-107">Ele retorna um recurso **planejador** singleton.</span><span class="sxs-lookup"><span data-stu-id="d98d7-107">It returns a singleton **planner** resource.</span></span>  <span data-ttu-id="d98d7-108">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="d98d7-108">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d98d7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="d98d7-109">Methods</span></span>

| <span data-ttu-id="d98d7-110">Método</span><span class="sxs-lookup"><span data-stu-id="d98d7-110">Method</span></span>           | <span data-ttu-id="d98d7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d98d7-111">Return Type</span></span>    |<span data-ttu-id="d98d7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d98d7-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d98d7-113">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d98d7-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="d98d7-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d98d7-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="d98d7-115">Crie um novo **plannerBucket** postando na coleção buckets.</span><span class="sxs-lookup"><span data-stu-id="d98d7-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="d98d7-116">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d98d7-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="d98d7-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d98d7-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="d98d7-118">Crie um novo **plannerPlan** postando na coleção Plans.</span><span class="sxs-lookup"><span data-stu-id="d98d7-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="d98d7-119">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="d98d7-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="d98d7-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="d98d7-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="d98d7-121">Crie um novo **plannerTask** postando na coleção Tasks.</span><span class="sxs-lookup"><span data-stu-id="d98d7-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d98d7-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d98d7-122">Properties</span></span>
| <span data-ttu-id="d98d7-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d98d7-123">Property</span></span>     | <span data-ttu-id="d98d7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="d98d7-124">Type</span></span>   |<span data-ttu-id="d98d7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d98d7-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d98d7-126">id</span><span class="sxs-lookup"><span data-stu-id="d98d7-126">id</span></span>|<span data-ttu-id="d98d7-127">String</span><span class="sxs-lookup"><span data-stu-id="d98d7-127">String</span></span>| <span data-ttu-id="d98d7-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d98d7-128">Read-only.</span></span> <span data-ttu-id="d98d7-129">Identificador do recurso **Planner** .</span><span class="sxs-lookup"><span data-stu-id="d98d7-129">Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d98d7-130">Relações</span><span class="sxs-lookup"><span data-stu-id="d98d7-130">Relationships</span></span>
| <span data-ttu-id="d98d7-131">Relação</span><span class="sxs-lookup"><span data-stu-id="d98d7-131">Relationship</span></span> | <span data-ttu-id="d98d7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="d98d7-132">Type</span></span>   |<span data-ttu-id="d98d7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="d98d7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d98d7-134">buckets</span><span class="sxs-lookup"><span data-stu-id="d98d7-134">buckets</span></span>|<span data-ttu-id="d98d7-135">coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d98d7-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d98d7-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d98d7-136">Read-only.</span></span> <span data-ttu-id="d98d7-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d98d7-137">Nullable.</span></span> <span data-ttu-id="d98d7-138">Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="d98d7-138">Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="d98d7-139">Planeje</span><span class="sxs-lookup"><span data-stu-id="d98d7-139">plans</span></span>|<span data-ttu-id="d98d7-140">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d98d7-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d98d7-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d98d7-141">Read-only.</span></span> <span data-ttu-id="d98d7-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d98d7-142">Nullable.</span></span> <span data-ttu-id="d98d7-143">Retorna uma coleção de planos especificados</span><span class="sxs-lookup"><span data-stu-id="d98d7-143">Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="d98d7-144">tarefas</span><span class="sxs-lookup"><span data-stu-id="d98d7-144">tasks</span></span>|<span data-ttu-id="d98d7-145">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d98d7-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d98d7-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d98d7-146">Read-only.</span></span> <span data-ttu-id="d98d7-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d98d7-147">Nullable.</span></span> <span data-ttu-id="d98d7-148">Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="d98d7-148">Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d98d7-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d98d7-149">JSON representation</span></span>
<span data-ttu-id="d98d7-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d98d7-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/planner.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
