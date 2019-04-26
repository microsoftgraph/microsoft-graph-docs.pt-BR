---
title: tipo de recurso plannerUser
description: 'O recurso **plannerUser** fornece acesso aos recursos do Planner para um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: fd279e541df4b45e47d1c389d2e8a1e212b01a41
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344337"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="35664-103">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="35664-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35664-104">O recurso **plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="35664-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="35664-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="35664-105">Methods</span></span>

| <span data-ttu-id="35664-106">Método</span><span class="sxs-lookup"><span data-stu-id="35664-106">Method</span></span>           | <span data-ttu-id="35664-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="35664-107">Return Type</span></span>    |<span data-ttu-id="35664-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="35664-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35664-109">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="35664-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="35664-110">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="35664-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="35664-111">Obtenha o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="35664-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="35664-112">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="35664-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="35664-113">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35664-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="35664-114">Obter o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="35664-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="35664-115">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="35664-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="35664-116">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35664-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="35664-117">Obtenha o [plannerPlans](plannerplan.md) exibido recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="35664-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="35664-118">Atualizar</span><span class="sxs-lookup"><span data-stu-id="35664-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="35664-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="35664-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="35664-120">Atualizar um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="35664-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="35664-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35664-121">Properties</span></span>
| <span data-ttu-id="35664-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35664-122">Property</span></span>     | <span data-ttu-id="35664-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="35664-123">Type</span></span>   |<span data-ttu-id="35664-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="35664-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35664-125">id</span><span class="sxs-lookup"><span data-stu-id="35664-125">id</span></span>|<span data-ttu-id="35664-126">String</span><span class="sxs-lookup"><span data-stu-id="35664-126">String</span></span>| <span data-ttu-id="35664-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35664-127">Read-only.</span></span> <span data-ttu-id="35664-128">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="35664-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="35664-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="35664-129">favoritePlanReferences</span></span>|[<span data-ttu-id="35664-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="35664-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="35664-131">Uma coleção que contém as referências aos planos que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="35664-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="35664-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="35664-132">recentPlanReferences</span></span>|[<span data-ttu-id="35664-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="35664-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="35664-134">Uma coleção que contém referências aos planos que foram exibidos recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="35664-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35664-135">Relações</span><span class="sxs-lookup"><span data-stu-id="35664-135">Relationships</span></span>
| <span data-ttu-id="35664-136">Relação</span><span class="sxs-lookup"><span data-stu-id="35664-136">Relationship</span></span> | <span data-ttu-id="35664-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="35664-137">Type</span></span>   |<span data-ttu-id="35664-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="35664-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35664-139">tarefas</span><span class="sxs-lookup"><span data-stu-id="35664-139">tasks</span></span>|<span data-ttu-id="35664-140">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="35664-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="35664-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35664-141">Read-only.</span></span> <span data-ttu-id="35664-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="35664-142">Nullable.</span></span> <span data-ttu-id="35664-143">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="35664-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="35664-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="35664-144">favoritePlans</span></span>|<span data-ttu-id="35664-145">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35664-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="35664-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35664-146">Read-only.</span></span> <span data-ttu-id="35664-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="35664-147">Nullable.</span></span> <span data-ttu-id="35664-148">Retorna o [plannerPlans](plannerplan.md) que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="35664-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="35664-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="35664-149">recentPlans</span></span>|<span data-ttu-id="35664-150">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="35664-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="35664-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="35664-151">Read-only.</span></span> <span data-ttu-id="35664-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="35664-152">Nullable.</span></span> <span data-ttu-id="35664-153">Retorna o [plannerPlans](plannerplan.md) que foi exibido recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="35664-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35664-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35664-154">JSON representation</span></span>
<span data-ttu-id="35664-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35664-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "favoritePlanReferences": {"@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"},
  "id": "String (identifier)",
  "recentPlanReferences": {"@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
