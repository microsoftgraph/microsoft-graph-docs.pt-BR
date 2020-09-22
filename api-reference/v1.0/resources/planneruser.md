---
title: tipo de recurso plannerUser
description: O recurso **plannerUser** fornece acesso a recursos do Planner para um usuário. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1bdf811e68e6a856d50621d063fe66daecf57748
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037358"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="424fd-104">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="424fd-104">plannerUser resource type</span></span>

<span data-ttu-id="424fd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="424fd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="424fd-106">O recurso **plannerUser** fornece acesso a recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="424fd-106">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="424fd-107">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="424fd-107">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="424fd-108">Methods</span><span class="sxs-lookup"><span data-stu-id="424fd-108">Methods</span></span>

| <span data-ttu-id="424fd-109">Método</span><span class="sxs-lookup"><span data-stu-id="424fd-109">Method</span></span>           | <span data-ttu-id="424fd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="424fd-110">Return Type</span></span>    |<span data-ttu-id="424fd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="424fd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="424fd-112">Listar planos</span><span class="sxs-lookup"><span data-stu-id="424fd-112">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="424fd-113">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="424fd-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="424fd-114">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="424fd-114">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="424fd-115">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="424fd-115">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="424fd-116">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="424fd-116">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="424fd-117">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="424fd-117">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="424fd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="424fd-118">Properties</span></span>
| <span data-ttu-id="424fd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="424fd-119">Property</span></span>     | <span data-ttu-id="424fd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="424fd-120">Type</span></span>   |<span data-ttu-id="424fd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="424fd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="424fd-122">id</span><span class="sxs-lookup"><span data-stu-id="424fd-122">id</span></span>|<span data-ttu-id="424fd-123">String</span><span class="sxs-lookup"><span data-stu-id="424fd-123">String</span></span>| <span data-ttu-id="424fd-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="424fd-124">Read-only.</span></span> <span data-ttu-id="424fd-125">Identificador do planenrUser</span><span class="sxs-lookup"><span data-stu-id="424fd-125">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="424fd-126">Relações</span><span class="sxs-lookup"><span data-stu-id="424fd-126">Relationships</span></span>
| <span data-ttu-id="424fd-127">Relação</span><span class="sxs-lookup"><span data-stu-id="424fd-127">Relationship</span></span> | <span data-ttu-id="424fd-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="424fd-128">Type</span></span>   |<span data-ttu-id="424fd-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="424fd-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="424fd-130">Planeje</span><span class="sxs-lookup"><span data-stu-id="424fd-130">plans</span></span>|<span data-ttu-id="424fd-131">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="424fd-131">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="424fd-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="424fd-132">Read-only.</span></span> <span data-ttu-id="424fd-133">Anulável.</span><span class="sxs-lookup"><span data-stu-id="424fd-133">Nullable.</span></span> <span data-ttu-id="424fd-134">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="424fd-134">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="424fd-135">tarefas</span><span class="sxs-lookup"><span data-stu-id="424fd-135">tasks</span></span>|<span data-ttu-id="424fd-136">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="424fd-136">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="424fd-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="424fd-137">Read-only.</span></span> <span data-ttu-id="424fd-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="424fd-138">Nullable.</span></span> <span data-ttu-id="424fd-139">Retorna o [plannerPlans](plannerplan.md) compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="424fd-139">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="424fd-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="424fd-140">JSON representation</span></span>
<span data-ttu-id="424fd-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="424fd-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

