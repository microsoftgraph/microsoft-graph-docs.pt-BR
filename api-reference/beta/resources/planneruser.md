---
title: tipo de recurso plannerUser
description: 'O recurso **plannerUser** fornece acesso aos recursos do Planner para um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2229020f00331e761eceeadf0739c84995e5bbdb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008989"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="c269e-103">tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="c269e-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c269e-104">O recurso **plannerUser** fornece acesso aos recursos do Planner para um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="c269e-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="c269e-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c269e-105">Methods</span></span>

| <span data-ttu-id="c269e-106">Método</span><span class="sxs-lookup"><span data-stu-id="c269e-106">Method</span></span>           | <span data-ttu-id="c269e-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c269e-107">Return Type</span></span>    |<span data-ttu-id="c269e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c269e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c269e-109">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="c269e-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="c269e-110">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c269e-111">Obtenha o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c269e-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="c269e-112">Listar favoritePlans</span><span class="sxs-lookup"><span data-stu-id="c269e-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="c269e-113">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c269e-114">Obter o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c269e-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="c269e-115">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="c269e-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="c269e-116">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c269e-117">Obtenha o [plannerPlans](plannerplan.md) exibido recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="c269e-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="c269e-118">Atualização</span><span class="sxs-lookup"><span data-stu-id="c269e-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="c269e-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="c269e-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="c269e-120">Atualizar um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="c269e-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="c269e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c269e-121">Properties</span></span>
| <span data-ttu-id="c269e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c269e-122">Property</span></span>     | <span data-ttu-id="c269e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c269e-123">Type</span></span>   |<span data-ttu-id="c269e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c269e-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c269e-125">id</span><span class="sxs-lookup"><span data-stu-id="c269e-125">id</span></span>|<span data-ttu-id="c269e-126">String</span><span class="sxs-lookup"><span data-stu-id="c269e-126">String</span></span>| <span data-ttu-id="c269e-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c269e-127">Read-only.</span></span> <span data-ttu-id="c269e-128">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="c269e-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="c269e-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="c269e-129">favoritePlanReferences</span></span>|[<span data-ttu-id="c269e-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c269e-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="c269e-131">Uma coleção que contém as referências aos planos que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="c269e-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="c269e-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="c269e-132">recentPlanReferences</span></span>|[<span data-ttu-id="c269e-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="c269e-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="c269e-134">Uma coleção que contém referências aos planos que foram exibidos recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="c269e-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c269e-135">Relações</span><span class="sxs-lookup"><span data-stu-id="c269e-135">Relationships</span></span>
| <span data-ttu-id="c269e-136">Relação</span><span class="sxs-lookup"><span data-stu-id="c269e-136">Relationship</span></span> | <span data-ttu-id="c269e-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="c269e-137">Type</span></span>   |<span data-ttu-id="c269e-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c269e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c269e-139">tarefas</span><span class="sxs-lookup"><span data-stu-id="c269e-139">tasks</span></span>|<span data-ttu-id="c269e-140">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c269e-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c269e-141">Read-only.</span></span> <span data-ttu-id="c269e-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c269e-142">Nullable.</span></span> <span data-ttu-id="c269e-143">Retorna o [plannerTasks](plannertask.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="c269e-143">Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="c269e-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="c269e-144">favoritePlans</span></span>|<span data-ttu-id="c269e-145">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c269e-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c269e-146">Read-only.</span></span> <span data-ttu-id="c269e-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c269e-147">Nullable.</span></span> <span data-ttu-id="c269e-148">Retorna o [plannerPlans](plannerplan.md) que o usuário marcou como favoritos.</span><span class="sxs-lookup"><span data-stu-id="c269e-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="c269e-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="c269e-149">recentPlans</span></span>|<span data-ttu-id="c269e-150">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="c269e-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="c269e-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c269e-151">Read-only.</span></span> <span data-ttu-id="c269e-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c269e-152">Nullable.</span></span> <span data-ttu-id="c269e-153">Retorna o [plannerPlans](plannerplan.md) que foi exibido recentemente pelo usuário em aplicativos que dão suporte a planos recentes.</span><span class="sxs-lookup"><span data-stu-id="c269e-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c269e-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c269e-154">JSON representation</span></span>
<span data-ttu-id="c269e-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c269e-155">The following is a JSON representation of the resource.</span></span>

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
