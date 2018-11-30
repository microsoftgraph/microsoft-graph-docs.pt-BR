---
title: Tipo de recurso planner
description: O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.
ms.openlocfilehash: c076eda1660cef9e31f584e5fe439f916eba81d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040994"
---
# <a name="planner-resource-type"></a><span data-ttu-id="d0202-105">Tipo de recurso planner</span><span class="sxs-lookup"><span data-stu-id="d0202-105">planner resource type</span></span>

> <span data-ttu-id="d0202-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d0202-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0202-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d0202-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0202-p103">O recurso **planner** é o ponto de entrada do modelo de objeto do Planner. Ele retorna um único recurso **planner**.  Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="d0202-p103">The **planner** resource is the entry point for the Planner object model. It returns a singleton **planner** resource.  It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="d0202-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="d0202-111">Methods</span></span>

| <span data-ttu-id="d0202-112">Método</span><span class="sxs-lookup"><span data-stu-id="d0202-112">Method</span></span>           | <span data-ttu-id="d0202-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0202-113">Return Type</span></span>    |<span data-ttu-id="d0202-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0202-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0202-115">Criar plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d0202-115">Create plannerBucket</span></span>](../api/planner-post-buckets.md) |[<span data-ttu-id="d0202-116">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="d0202-116">plannerBucket</span></span>](plannerbucket.md)| <span data-ttu-id="d0202-117">Crie um novo **plannerBucket** ao postar na coleção de buckets.</span><span class="sxs-lookup"><span data-stu-id="d0202-117">Create a new **plannerBucket** by posting to the buckets collection.</span></span>|
|[<span data-ttu-id="d0202-118">Criar plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0202-118">Create plannerPlan</span></span>](../api/planner-post-plans.md) |[<span data-ttu-id="d0202-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0202-119">plannerPlan</span></span>](plannerplan.md)| <span data-ttu-id="d0202-120">Crie um novo **plannerPlan** ao postar na coleção de planos.</span><span class="sxs-lookup"><span data-stu-id="d0202-120">Create a new **plannerPlan** by posting to the plans collection.</span></span>|
|[<span data-ttu-id="d0202-121">Criar plannerTask</span><span class="sxs-lookup"><span data-stu-id="d0202-121">Create plannerTask</span></span>](../api/planner-post-tasks.md) |[<span data-ttu-id="d0202-122">plannerTask</span><span class="sxs-lookup"><span data-stu-id="d0202-122">plannerTask</span></span>](plannertask.md)| <span data-ttu-id="d0202-123">Crie um novo **plannerTask** ao postar na coleção de tarefas.</span><span class="sxs-lookup"><span data-stu-id="d0202-123">Create a new **plannerTask** by posting to the tasks collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0202-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0202-124">Properties</span></span>
| <span data-ttu-id="d0202-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0202-125">Property</span></span>     | <span data-ttu-id="d0202-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0202-126">Type</span></span>   |<span data-ttu-id="d0202-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0202-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0202-128">id</span><span class="sxs-lookup"><span data-stu-id="d0202-128">id</span></span>|<span data-ttu-id="d0202-129">String</span><span class="sxs-lookup"><span data-stu-id="d0202-129">String</span></span>| <span data-ttu-id="d0202-p104">Somente leitura. O identificador do recurso **planner**</span><span class="sxs-lookup"><span data-stu-id="d0202-p104">Read-only. Identifier of the **planner** resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0202-132">Relações</span><span class="sxs-lookup"><span data-stu-id="d0202-132">Relationships</span></span>
| <span data-ttu-id="d0202-133">Relação</span><span class="sxs-lookup"><span data-stu-id="d0202-133">Relationship</span></span> | <span data-ttu-id="d0202-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0202-134">Type</span></span>   |<span data-ttu-id="d0202-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0202-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0202-136">buckets</span><span class="sxs-lookup"><span data-stu-id="d0202-136">buckets</span></span>|<span data-ttu-id="d0202-137">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d0202-137">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d0202-p105">Somente leitura. Anulável. Retorna uma coleção dos buckets especificados</span><span class="sxs-lookup"><span data-stu-id="d0202-p105">Read-only. Nullable. Returns a collection of the specified buckets</span></span>|
|<span data-ttu-id="d0202-141">plans</span><span class="sxs-lookup"><span data-stu-id="d0202-141">plans</span></span>|<span data-ttu-id="d0202-142">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="d0202-142">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="d0202-p106">Somente leitura. Anulável. Retorna uma coleção dos planos especificados</span><span class="sxs-lookup"><span data-stu-id="d0202-p106">Read-only. Nullable. Returns a collection of the specified plans</span></span>|
|<span data-ttu-id="d0202-146">tarefas</span><span class="sxs-lookup"><span data-stu-id="d0202-146">tasks</span></span>|<span data-ttu-id="d0202-147">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d0202-147">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d0202-p107">Somente leitura. Anulável. Retorna uma coleção das tarefas especificadas</span><span class="sxs-lookup"><span data-stu-id="d0202-p107">Read-only. Nullable. Returns a collection of the specified tasks</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0202-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0202-151">JSON representation</span></span>
<span data-ttu-id="d0202-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0202-152">Here is a JSON representation of the resource.</span></span>

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