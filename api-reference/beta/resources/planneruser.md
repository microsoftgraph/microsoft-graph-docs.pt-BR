---
title: Tipo de recurso plannerUser
description: 'O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um usuário. '
ms.openlocfilehash: 592a26daacd1bd6d0a780ca0180d3ec5a57b6eb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037232"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="9f397-103">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="9f397-103">plannerUser resource type</span></span>

> <span data-ttu-id="9f397-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f397-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f397-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f397-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f397-106">O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="9f397-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="9f397-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f397-107">Methods</span></span>

| <span data-ttu-id="9f397-108">Método</span><span class="sxs-lookup"><span data-stu-id="9f397-108">Method</span></span>           | <span data-ttu-id="9f397-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f397-109">Return Type</span></span>    |<span data-ttu-id="9f397-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f397-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9f397-111">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="9f397-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="9f397-112">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9f397-113">Obtenha o [plannerTasks](plannertask.md) atribuída ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9f397-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="9f397-114">Lista favoritePlans</span><span class="sxs-lookup"><span data-stu-id="9f397-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="9f397-115">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9f397-116">Obtenha o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9f397-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="9f397-117">Lista recentPlans</span><span class="sxs-lookup"><span data-stu-id="9f397-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="9f397-118">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9f397-119">Obtenha o [plannerPlans](plannerplan.md) visualizados recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9f397-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="9f397-120">Update</span><span class="sxs-lookup"><span data-stu-id="9f397-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="9f397-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="9f397-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="9f397-122">Atualize um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="9f397-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="9f397-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f397-123">Properties</span></span>
| <span data-ttu-id="9f397-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f397-124">Property</span></span>     | <span data-ttu-id="9f397-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f397-125">Type</span></span>   |<span data-ttu-id="9f397-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f397-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f397-127">id</span><span class="sxs-lookup"><span data-stu-id="9f397-127">id</span></span>|<span data-ttu-id="9f397-128">String</span><span class="sxs-lookup"><span data-stu-id="9f397-128">String</span></span>| <span data-ttu-id="9f397-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f397-129">Read-only.</span></span> <span data-ttu-id="9f397-130">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="9f397-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="9f397-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="9f397-131">favoritePlanReferences</span></span>|[<span data-ttu-id="9f397-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9f397-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="9f397-133">Uma coleção que contém as referências para os planos de que o usuário tenha marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="9f397-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="9f397-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="9f397-134">recentPlanReferences</span></span>|[<span data-ttu-id="9f397-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="9f397-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="9f397-136">Uma coleção que contém referências para os planos que foram visualizados recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="9f397-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f397-137">Relações</span><span class="sxs-lookup"><span data-stu-id="9f397-137">Relationships</span></span>
| <span data-ttu-id="9f397-138">Relação</span><span class="sxs-lookup"><span data-stu-id="9f397-138">Relationship</span></span> | <span data-ttu-id="9f397-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f397-139">Type</span></span>   |<span data-ttu-id="9f397-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f397-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f397-141">tarefas</span><span class="sxs-lookup"><span data-stu-id="9f397-141">tasks</span></span>|<span data-ttu-id="9f397-142">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9f397-p103">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="9f397-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="9f397-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="9f397-146">favoritePlans</span></span>|<span data-ttu-id="9f397-147">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9f397-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f397-148">Read-only.</span></span> <span data-ttu-id="9f397-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9f397-149">Nullable.</span></span> <span data-ttu-id="9f397-150">Retorna o [plannerPlans](plannerplan.md) que o usuário marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="9f397-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="9f397-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="9f397-151">recentPlans</span></span>|<span data-ttu-id="9f397-152">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="9f397-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="9f397-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9f397-153">Read-only.</span></span> <span data-ttu-id="9f397-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9f397-154">Nullable.</span></span> <span data-ttu-id="9f397-155">Retorna o [plannerPlans](plannerplan.md) exibidos recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="9f397-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f397-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f397-156">JSON representation</span></span>
<span data-ttu-id="9f397-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f397-157">The following is a JSON representation of the resource.</span></span>

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
