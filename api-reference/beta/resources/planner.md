---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: cf2877d5f413f3e54e1e0e750da1f22d6f9ffd95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925179"
---
# <a name="planner-resource-type"></a><span data-ttu-id="6f20c-105">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="6f20c-105">planner resource type</span></span>

> <span data-ttu-id="6f20c-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f20c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f20c-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f20c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6f20c-p103">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="6f20c-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="6f20c-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f20c-111">Methods</span></span>

| <span data-ttu-id="6f20c-112">Método</span><span class="sxs-lookup"><span data-stu-id="6f20c-112">Method</span></span>           | <span data-ttu-id="6f20c-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f20c-113">Return Type</span></span>    |<span data-ttu-id="6f20c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f20c-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f20c-115">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="6f20c-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="6f20c-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="6f20c-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="6f20c-117">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="6f20c-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="6f20c-118">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6f20c-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="6f20c-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6f20c-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="6f20c-120">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="6f20c-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="6f20c-121">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="6f20c-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="6f20c-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="6f20c-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="6f20c-123">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="6f20c-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f20c-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f20c-124">Properties</span></span>
| <span data-ttu-id="6f20c-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6f20c-125">Property</span></span>     | <span data-ttu-id="6f20c-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f20c-126">Type</span></span>   |<span data-ttu-id="6f20c-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f20c-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f20c-128">id</span><span class="sxs-lookup"><span data-stu-id="6f20c-128">id</span></span>|<span data-ttu-id="6f20c-129">String</span><span class="sxs-lookup"><span data-stu-id="6f20c-129">String</span></span>| <span data-ttu-id="6f20c-p104">Somente leitura. O identificador do recurso **planner**</span><span class="sxs-lookup"><span data-stu-id="6f20c-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f20c-132">Relações</span><span class="sxs-lookup"><span data-stu-id="6f20c-132">Relationships</span></span>
| <span data-ttu-id="6f20c-133">Relação</span><span class="sxs-lookup"><span data-stu-id="6f20c-133">Relationship</span></span> | <span data-ttu-id="6f20c-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f20c-134">Type</span></span>   |<span data-ttu-id="6f20c-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f20c-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f20c-136">buckets</span><span class="sxs-lookup"><span data-stu-id="6f20c-136">buckets</span></span>|<span data-ttu-id="6f20c-137">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="6f20c-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6f20c-p105">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="6f20c-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="6f20c-141">plans</span><span class="sxs-lookup"><span data-stu-id="6f20c-141">plans</span></span>|<span data-ttu-id="6f20c-142">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="6f20c-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="6f20c-p106">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="6f20c-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="6f20c-146">tarefas</span><span class="sxs-lookup"><span data-stu-id="6f20c-146">tasks</span></span>|<span data-ttu-id="6f20c-147">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="6f20c-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6f20c-p107">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="6f20c-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f20c-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f20c-151">JSON representation</span></span>
<span data-ttu-id="6f20c-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6f20c-152">Here is a JSON representation of the resource.</span></span>

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
