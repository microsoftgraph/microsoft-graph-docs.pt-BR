---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 50ceb8b76b398bd5898e48f31df9a6443569781e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523397"
---
# <a name="planner-resource-type"></a><span data-ttu-id="2119f-105">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="2119f-105">planner resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2119f-p102">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="2119f-p102">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="2119f-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="2119f-109">Methods</span></span>

| <span data-ttu-id="2119f-110">Método</span><span class="sxs-lookup"><span data-stu-id="2119f-110">Method</span></span>           | <span data-ttu-id="2119f-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2119f-111">Return Type</span></span>    |<span data-ttu-id="2119f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2119f-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2119f-113">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2119f-113">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="2119f-114">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="2119f-114">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="2119f-115">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="2119f-115">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="2119f-116">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2119f-116">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="2119f-117">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2119f-117">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="2119f-118">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="2119f-118">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="2119f-119">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="2119f-119">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="2119f-120">plannerTask</span><span class="sxs-lookup"><span data-stu-id="2119f-120">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="2119f-121">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="2119f-121">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="2119f-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2119f-122">Properties</span></span>
| <span data-ttu-id="2119f-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2119f-123">Property</span></span>     | <span data-ttu-id="2119f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="2119f-124">Type</span></span>   |<span data-ttu-id="2119f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="2119f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2119f-126">id</span><span class="sxs-lookup"><span data-stu-id="2119f-126">id</span></span>|<span data-ttu-id="2119f-127">String</span><span class="sxs-lookup"><span data-stu-id="2119f-127">String</span></span>| <span data-ttu-id="2119f-p103">Somente leitura. O identificador do recurso **planner**</span><span class="sxs-lookup"><span data-stu-id="2119f-p103">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2119f-130">Relações</span><span class="sxs-lookup"><span data-stu-id="2119f-130">Relationships</span></span>
| <span data-ttu-id="2119f-131">Relação</span><span class="sxs-lookup"><span data-stu-id="2119f-131">Relationship</span></span> | <span data-ttu-id="2119f-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2119f-132">Type</span></span>   |<span data-ttu-id="2119f-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2119f-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2119f-134">buckets</span><span class="sxs-lookup"><span data-stu-id="2119f-134">buckets</span></span>|<span data-ttu-id="2119f-135">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2119f-135">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2119f-p104">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="2119f-p104">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="2119f-139">plans</span><span class="sxs-lookup"><span data-stu-id="2119f-139">plans</span></span>|<span data-ttu-id="2119f-140">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="2119f-140">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="2119f-p105">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="2119f-p105">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="2119f-144">tarefas</span><span class="sxs-lookup"><span data-stu-id="2119f-144">tasks</span></span>|<span data-ttu-id="2119f-145">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2119f-145">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2119f-p106">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="2119f-p106">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2119f-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2119f-149">JSON representation</span></span>
<span data-ttu-id="2119f-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2119f-150">Here is a JSON representation of the resource.</span></span>

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
