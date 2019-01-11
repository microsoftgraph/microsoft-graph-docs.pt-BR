---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
ms.openlocfilehash: 9dc6904da25d7612b94649264001dcae98859925
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889093"
---
# <a name="planner-resource-type"></a><span data-ttu-id="71fc3-105">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="71fc3-105">planner resource type</span></span>

> <span data-ttu-id="71fc3-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="71fc3-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71fc3-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="71fc3-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71fc3-p103">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="71fc3-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="71fc3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="71fc3-111">Methods</span></span>

| <span data-ttu-id="71fc3-112">Método</span><span class="sxs-lookup"><span data-stu-id="71fc3-112">Method</span></span>           | <span data-ttu-id="71fc3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71fc3-113">Return Type</span></span>    |<span data-ttu-id="71fc3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fc3-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71fc3-115">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="71fc3-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="71fc3-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="71fc3-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="71fc3-117">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="71fc3-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="71fc3-118">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="71fc3-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="71fc3-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="71fc3-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="71fc3-120">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="71fc3-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="71fc3-121">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="71fc3-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="71fc3-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="71fc3-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="71fc3-123">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="71fc3-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="71fc3-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71fc3-124">Properties</span></span>
| <span data-ttu-id="71fc3-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71fc3-125">Property</span></span>     | <span data-ttu-id="71fc3-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fc3-126">Type</span></span>   |<span data-ttu-id="71fc3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fc3-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71fc3-128">id</span><span class="sxs-lookup"><span data-stu-id="71fc3-128">id</span></span>|<span data-ttu-id="71fc3-129">String</span><span class="sxs-lookup"><span data-stu-id="71fc3-129">String</span></span>| <span data-ttu-id="71fc3-p104">Somente leitura. O identificador do recurso **planner**</span><span class="sxs-lookup"><span data-stu-id="71fc3-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71fc3-132">Relações</span><span class="sxs-lookup"><span data-stu-id="71fc3-132">Relationships</span></span>
| <span data-ttu-id="71fc3-133">Relação</span><span class="sxs-lookup"><span data-stu-id="71fc3-133">Relationship</span></span> | <span data-ttu-id="71fc3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fc3-134">Type</span></span>   |<span data-ttu-id="71fc3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fc3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71fc3-136">buckets</span><span class="sxs-lookup"><span data-stu-id="71fc3-136">buckets</span></span>|<span data-ttu-id="71fc3-137">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="71fc3-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="71fc3-p105">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="71fc3-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="71fc3-141">plans</span><span class="sxs-lookup"><span data-stu-id="71fc3-141">plans</span></span>|<span data-ttu-id="71fc3-142">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="71fc3-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="71fc3-p106">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="71fc3-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="71fc3-146">tarefas</span><span class="sxs-lookup"><span data-stu-id="71fc3-146">tasks</span></span>|<span data-ttu-id="71fc3-147">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="71fc3-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="71fc3-p107">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="71fc3-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71fc3-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71fc3-151">JSON representation</span></span>
<span data-ttu-id="71fc3-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71fc3-152">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
