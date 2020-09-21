---
title: tipo de recurso plannerUser
description: 'O recurso **plannerUser** fornece acesso aos recursos do Planner para um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 309f464afe33f09366f7905af7698660dd161094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063966"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="706d0-103">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="706d0-103">plannerUser resource type</span></span>

<span data-ttu-id="706d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="706d0-105">O recurso **plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="706d0-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="706d0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="706d0-106">Methods</span></span>

| <span data-ttu-id="706d0-107">Método</span><span class="sxs-lookup"><span data-stu-id="706d0-107">Method</span></span>           | <span data-ttu-id="706d0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="706d0-108">Return Type</span></span>    |<span data-ttu-id="706d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="706d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="706d0-110">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="706d0-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="706d0-111">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="706d0-112">Obtenha o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="706d0-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="706d0-113">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="706d0-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="706d0-114">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="706d0-115">Obter o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="706d0-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="706d0-116">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="706d0-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="706d0-117">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="706d0-118">Obtenha o [plannerPlans](plannerplan.md) exibido recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="706d0-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="706d0-119">Update</span><span class="sxs-lookup"><span data-stu-id="706d0-119">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="706d0-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="706d0-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="706d0-121">Atualizar um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="706d0-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="706d0-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="706d0-122">Properties</span></span>
| <span data-ttu-id="706d0-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="706d0-123">Property</span></span>     | <span data-ttu-id="706d0-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="706d0-124">Type</span></span>   |<span data-ttu-id="706d0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="706d0-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="706d0-126">id</span><span class="sxs-lookup"><span data-stu-id="706d0-126">id</span></span>|<span data-ttu-id="706d0-127">String</span><span class="sxs-lookup"><span data-stu-id="706d0-127">String</span></span>| <span data-ttu-id="706d0-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706d0-128">Read-only.</span></span> <span data-ttu-id="706d0-129">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="706d0-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="706d0-130">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="706d0-130">favoritePlanReferences</span></span>|[<span data-ttu-id="706d0-131">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="706d0-131">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="706d0-132">Uma coleção que contém as referências aos planos que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="706d0-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="706d0-133">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="706d0-133">recentPlanReferences</span></span>|[<span data-ttu-id="706d0-134">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="706d0-134">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="706d0-135">Uma coleção que contém referências aos planos que foram exibidos recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="706d0-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="706d0-136">Relações</span><span class="sxs-lookup"><span data-stu-id="706d0-136">Relationships</span></span>
| <span data-ttu-id="706d0-137">Relação</span><span class="sxs-lookup"><span data-stu-id="706d0-137">Relationship</span></span> | <span data-ttu-id="706d0-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="706d0-138">Type</span></span>   |<span data-ttu-id="706d0-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="706d0-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="706d0-140">tarefas</span><span class="sxs-lookup"><span data-stu-id="706d0-140">tasks</span></span>|<span data-ttu-id="706d0-141">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="706d0-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706d0-142">Read-only.</span></span> <span data-ttu-id="706d0-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="706d0-143">Nullable.</span></span> <span data-ttu-id="706d0-144">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="706d0-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="706d0-145">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="706d0-145">favoritePlans</span></span>|<span data-ttu-id="706d0-146">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="706d0-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706d0-147">Read-only.</span></span> <span data-ttu-id="706d0-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="706d0-148">Nullable.</span></span> <span data-ttu-id="706d0-149">Retorna o [plannerPlans](plannerplan.md) que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="706d0-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="706d0-150">recentPlans</span><span class="sxs-lookup"><span data-stu-id="706d0-150">recentPlans</span></span>|<span data-ttu-id="706d0-151">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="706d0-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="706d0-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="706d0-152">Read-only.</span></span> <span data-ttu-id="706d0-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="706d0-153">Nullable.</span></span> <span data-ttu-id="706d0-154">Retorna o [plannerPlans](plannerplan.md) que foi exibido recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="706d0-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="706d0-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="706d0-155">JSON representation</span></span>
<span data-ttu-id="706d0-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="706d0-156">The following is a JSON representation of the resource.</span></span>

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


