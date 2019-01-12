---
title: Tipo de recurso plannerUser
description: 'O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1b240092e7476884399f88fad61551763f33fe69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928276"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="36552-103">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="36552-103">plannerUser resource type</span></span>

> <span data-ttu-id="36552-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="36552-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36552-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36552-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36552-106">O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="36552-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="36552-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="36552-107">Methods</span></span>

| <span data-ttu-id="36552-108">Método</span><span class="sxs-lookup"><span data-stu-id="36552-108">Method</span></span>           | <span data-ttu-id="36552-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36552-109">Return Type</span></span>    |<span data-ttu-id="36552-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="36552-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="36552-111">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="36552-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="36552-112">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="36552-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="36552-113">Obtenha o [plannerTasks](plannertask.md) atribuída ao usuário.</span><span class="sxs-lookup"><span data-stu-id="36552-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="36552-114">Lista favoritePlans</span><span class="sxs-lookup"><span data-stu-id="36552-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="36552-115">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="36552-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="36552-116">Obtenha o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="36552-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="36552-117">Lista recentPlans</span><span class="sxs-lookup"><span data-stu-id="36552-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="36552-118">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="36552-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="36552-119">Obtenha o [plannerPlans](plannerplan.md) visualizados recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="36552-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="36552-120">Update</span><span class="sxs-lookup"><span data-stu-id="36552-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="36552-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="36552-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="36552-122">Atualize um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="36552-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="36552-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36552-123">Properties</span></span>
| <span data-ttu-id="36552-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36552-124">Property</span></span>     | <span data-ttu-id="36552-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="36552-125">Type</span></span>   |<span data-ttu-id="36552-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="36552-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36552-127">id</span><span class="sxs-lookup"><span data-stu-id="36552-127">id</span></span>|<span data-ttu-id="36552-128">String</span><span class="sxs-lookup"><span data-stu-id="36552-128">String</span></span>| <span data-ttu-id="36552-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36552-129">Read-only.</span></span> <span data-ttu-id="36552-130">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="36552-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="36552-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="36552-131">favoritePlanReferences</span></span>|[<span data-ttu-id="36552-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="36552-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="36552-133">Uma coleção que contém as referências para os planos de que o usuário tenha marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="36552-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="36552-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="36552-134">recentPlanReferences</span></span>|[<span data-ttu-id="36552-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="36552-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="36552-136">Uma coleção que contém referências para os planos que foram visualizados recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="36552-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36552-137">Relações</span><span class="sxs-lookup"><span data-stu-id="36552-137">Relationships</span></span>
| <span data-ttu-id="36552-138">Relação</span><span class="sxs-lookup"><span data-stu-id="36552-138">Relationship</span></span> | <span data-ttu-id="36552-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="36552-139">Type</span></span>   |<span data-ttu-id="36552-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="36552-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36552-141">tarefas</span><span class="sxs-lookup"><span data-stu-id="36552-141">tasks</span></span>|<span data-ttu-id="36552-142">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="36552-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="36552-p103">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="36552-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="36552-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="36552-146">favoritePlans</span></span>|<span data-ttu-id="36552-147">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="36552-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="36552-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36552-148">Read-only.</span></span> <span data-ttu-id="36552-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="36552-149">Nullable.</span></span> <span data-ttu-id="36552-150">Retorna o [plannerPlans](plannerplan.md) que o usuário marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="36552-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="36552-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="36552-151">recentPlans</span></span>|<span data-ttu-id="36552-152">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="36552-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="36552-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36552-153">Read-only.</span></span> <span data-ttu-id="36552-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="36552-154">Nullable.</span></span> <span data-ttu-id="36552-155">Retorna o [plannerPlans](plannerplan.md) exibidos recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="36552-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="36552-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36552-156">JSON representation</span></span>
<span data-ttu-id="36552-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36552-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
