---
title: tipo de recurso plannerUser
description: O recurso **plannerUser** fornece acesso a recursos do Planner para um usuário. Ele não contém propriedades utilizáveis.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d995888b55282ac9db8aef9cc047f069a3cf20fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035137"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="9ebb9-104">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="9ebb9-104">plannerUser resource type</span></span>

<span data-ttu-id="9ebb9-105">O recurso **plannerUser** fornece acesso a recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="9ebb9-105">The **plannerUser** resource provide access to Planner resources for a [user](user.md).</span></span> <span data-ttu-id="9ebb9-106">Ele não contém propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-106">It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="9ebb9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ebb9-107">Methods</span></span>

| <span data-ttu-id="9ebb9-108">Método</span><span class="sxs-lookup"><span data-stu-id="9ebb9-108">Method</span></span>           | <span data-ttu-id="9ebb9-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ebb9-109">Return Type</span></span>    |<span data-ttu-id="9ebb9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ebb9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ebb9-111">Listar planos</span><span class="sxs-lookup"><span data-stu-id="9ebb9-111">List plans</span></span>](../api/planneruser-list-plans.md) |<span data-ttu-id="9ebb9-112">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9ebb9-112">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9ebb9-113">Obtenha uma coleção de objetos **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="9ebb9-113">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="9ebb9-114">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="9ebb9-114">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="9ebb9-115">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9ebb9-115">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9ebb9-116">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-116">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ebb9-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ebb9-117">Properties</span></span>
| <span data-ttu-id="9ebb9-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ebb9-118">Property</span></span>     | <span data-ttu-id="9ebb9-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ebb9-119">Type</span></span>   |<span data-ttu-id="9ebb9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ebb9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ebb9-121">id</span><span class="sxs-lookup"><span data-stu-id="9ebb9-121">id</span></span>|<span data-ttu-id="9ebb9-122">String</span><span class="sxs-lookup"><span data-stu-id="9ebb9-122">String</span></span>| <span data-ttu-id="9ebb9-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-123">Read-only.</span></span> <span data-ttu-id="9ebb9-124">Identificador do planenrUser</span><span class="sxs-lookup"><span data-stu-id="9ebb9-124">Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ebb9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="9ebb9-125">Relationships</span></span>
| <span data-ttu-id="9ebb9-126">Relação</span><span class="sxs-lookup"><span data-stu-id="9ebb9-126">Relationship</span></span> | <span data-ttu-id="9ebb9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ebb9-127">Type</span></span>   |<span data-ttu-id="9ebb9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ebb9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ebb9-129">Planeje</span><span class="sxs-lookup"><span data-stu-id="9ebb9-129">plans</span></span>|<span data-ttu-id="9ebb9-130">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9ebb9-130">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9ebb9-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-131">Read-only.</span></span> <span data-ttu-id="9ebb9-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-132">Nullable.</span></span> <span data-ttu-id="9ebb9-133">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-133">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="9ebb9-134">tarefas</span><span class="sxs-lookup"><span data-stu-id="9ebb9-134">tasks</span></span>|<span data-ttu-id="9ebb9-135">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9ebb9-135">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9ebb9-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-136">Read-only.</span></span> <span data-ttu-id="9ebb9-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-137">Nullable.</span></span> <span data-ttu-id="9ebb9-138">Retorna o [plannerPlans](plannerplan.md) compartilhado com o usuário.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-138">Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ebb9-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ebb9-139">JSON representation</span></span>
<span data-ttu-id="9ebb9-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ebb9-140">Here is a JSON representation of the resource.</span></span>

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
