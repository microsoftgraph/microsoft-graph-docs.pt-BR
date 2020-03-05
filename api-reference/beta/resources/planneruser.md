---
title: tipo de recurso plannerUser
description: 'O recurso **plannerUser** fornece acesso aos recursos do Planner para um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 70ca7596cfb809a16b76f684a85c97b0c3e43a50
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521633"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="949aa-103">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="949aa-103">plannerUser resource type</span></span>

<span data-ttu-id="949aa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="949aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949aa-105">O recurso **plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="949aa-105">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="949aa-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="949aa-106">Methods</span></span>

| <span data-ttu-id="949aa-107">Método</span><span class="sxs-lookup"><span data-stu-id="949aa-107">Method</span></span>           | <span data-ttu-id="949aa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="949aa-108">Return Type</span></span>    |<span data-ttu-id="949aa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="949aa-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="949aa-110">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="949aa-110">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="949aa-111">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-111">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="949aa-112">Obtenha o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="949aa-112">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="949aa-113">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="949aa-113">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="949aa-114">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-114">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="949aa-115">Obter o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="949aa-115">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="949aa-116">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="949aa-116">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="949aa-117">coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-117">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="949aa-118">Obtenha o [plannerPlans](plannerplan.md) exibido recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="949aa-118">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="949aa-119">Update</span><span class="sxs-lookup"><span data-stu-id="949aa-119">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="949aa-120">plannerUser</span><span class="sxs-lookup"><span data-stu-id="949aa-120">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="949aa-121">Atualizar um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="949aa-121">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="949aa-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="949aa-122">Properties</span></span>
| <span data-ttu-id="949aa-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="949aa-123">Property</span></span>     | <span data-ttu-id="949aa-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="949aa-124">Type</span></span>   |<span data-ttu-id="949aa-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="949aa-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="949aa-126">id</span><span class="sxs-lookup"><span data-stu-id="949aa-126">id</span></span>|<span data-ttu-id="949aa-127">String</span><span class="sxs-lookup"><span data-stu-id="949aa-127">String</span></span>| <span data-ttu-id="949aa-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="949aa-128">Read-only.</span></span> <span data-ttu-id="949aa-129">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="949aa-129">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="949aa-130">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="949aa-130">favoritePlanReferences</span></span>|[<span data-ttu-id="949aa-131">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="949aa-131">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="949aa-132">Uma coleção que contém as referências aos planos que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="949aa-132">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="949aa-133">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="949aa-133">recentPlanReferences</span></span>|[<span data-ttu-id="949aa-134">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="949aa-134">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="949aa-135">Uma coleção que contém referências aos planos que foram exibidos recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="949aa-135">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="949aa-136">Relações</span><span class="sxs-lookup"><span data-stu-id="949aa-136">Relationships</span></span>
| <span data-ttu-id="949aa-137">Relação</span><span class="sxs-lookup"><span data-stu-id="949aa-137">Relationship</span></span> | <span data-ttu-id="949aa-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="949aa-138">Type</span></span>   |<span data-ttu-id="949aa-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="949aa-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="949aa-140">tarefas</span><span class="sxs-lookup"><span data-stu-id="949aa-140">tasks</span></span>|<span data-ttu-id="949aa-141">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-141">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="949aa-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="949aa-142">Read-only.</span></span> <span data-ttu-id="949aa-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="949aa-143">Nullable.</span></span> <span data-ttu-id="949aa-144">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="949aa-144">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="949aa-145">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="949aa-145">favoritePlans</span></span>|<span data-ttu-id="949aa-146">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-146">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="949aa-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="949aa-147">Read-only.</span></span> <span data-ttu-id="949aa-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="949aa-148">Nullable.</span></span> <span data-ttu-id="949aa-149">Retorna o [plannerPlans](plannerplan.md) que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="949aa-149">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="949aa-150">recentPlans</span><span class="sxs-lookup"><span data-stu-id="949aa-150">recentPlans</span></span>|<span data-ttu-id="949aa-151">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="949aa-151">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="949aa-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="949aa-152">Read-only.</span></span> <span data-ttu-id="949aa-153">Anulável.</span><span class="sxs-lookup"><span data-stu-id="949aa-153">Nullable.</span></span> <span data-ttu-id="949aa-154">Retorna o [plannerPlans](plannerplan.md) que foi exibido recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="949aa-154">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="949aa-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="949aa-155">JSON representation</span></span>
<span data-ttu-id="949aa-156">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="949aa-156">The following is a JSON representation of the resource.</span></span>

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
