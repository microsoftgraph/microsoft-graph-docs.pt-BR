---
title: Tipo de recurso plannerUser
description: 'O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um usuário. '
localization_priority: Normal
ms.openlocfilehash: 709b259c88d8fe0f02defaa57e77727a7b967cfd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820801"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="eeb1f-103">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="eeb1f-103">plannerUser resource type</span></span>

> <span data-ttu-id="eeb1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eeb1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eeb1f-106">O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="eeb1f-106">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="eeb1f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eeb1f-107">Methods</span></span>

| <span data-ttu-id="eeb1f-108">Método</span><span class="sxs-lookup"><span data-stu-id="eeb1f-108">Method</span></span>           | <span data-ttu-id="eeb1f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eeb1f-109">Return Type</span></span>    |<span data-ttu-id="eeb1f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb1f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eeb1f-111">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="eeb1f-111">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="eeb1f-112">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="eeb1f-113">Obtenha o [plannerTasks](plannertask.md) atribuída ao usuário.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-113">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="eeb1f-114">Lista favoritePlans</span><span class="sxs-lookup"><span data-stu-id="eeb1f-114">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="eeb1f-115">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-115">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="eeb1f-116">Obtenha o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-116">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="eeb1f-117">Lista recentPlans</span><span class="sxs-lookup"><span data-stu-id="eeb1f-117">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="eeb1f-118">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-118">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="eeb1f-119">Obtenha o [plannerPlans](plannerplan.md) visualizados recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-119">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="eeb1f-120">Update</span><span class="sxs-lookup"><span data-stu-id="eeb1f-120">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="eeb1f-121">plannerUser</span><span class="sxs-lookup"><span data-stu-id="eeb1f-121">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="eeb1f-122">Atualize um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="eeb1f-122">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="eeb1f-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eeb1f-123">Properties</span></span>
| <span data-ttu-id="eeb1f-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eeb1f-124">Property</span></span>     | <span data-ttu-id="eeb1f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb1f-125">Type</span></span>   |<span data-ttu-id="eeb1f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb1f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb1f-127">id</span><span class="sxs-lookup"><span data-stu-id="eeb1f-127">id</span></span>|<span data-ttu-id="eeb1f-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eeb1f-128">String</span></span>| <span data-ttu-id="eeb1f-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-129">Read-only.</span></span> <span data-ttu-id="eeb1f-130">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="eeb1f-130">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="eeb1f-131">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="eeb1f-131">favoritePlanReferences</span></span>|[<span data-ttu-id="eeb1f-132">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="eeb1f-132">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="eeb1f-133">Uma coleção que contém as referências para os planos de que o usuário tenha marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-133">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="eeb1f-134">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="eeb1f-134">recentPlanReferences</span></span>|[<span data-ttu-id="eeb1f-135">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="eeb1f-135">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="eeb1f-136">Uma coleção que contém referências para os planos que foram visualizados recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-136">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeb1f-137">Relações</span><span class="sxs-lookup"><span data-stu-id="eeb1f-137">Relationships</span></span>
| <span data-ttu-id="eeb1f-138">Relação</span><span class="sxs-lookup"><span data-stu-id="eeb1f-138">Relationship</span></span> | <span data-ttu-id="eeb1f-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="eeb1f-139">Type</span></span>   |<span data-ttu-id="eeb1f-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="eeb1f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eeb1f-141">tarefas</span><span class="sxs-lookup"><span data-stu-id="eeb1f-141">tasks</span></span>|<span data-ttu-id="eeb1f-142">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-142">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="eeb1f-p103">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="eeb1f-146">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="eeb1f-146">favoritePlans</span></span>|<span data-ttu-id="eeb1f-147">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-147">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="eeb1f-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-148">Read-only.</span></span> <span data-ttu-id="eeb1f-149">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-149">Nullable.</span></span> <span data-ttu-id="eeb1f-150">Retorna o [plannerPlans](plannerplan.md) que o usuário marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-150">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="eeb1f-151">recentPlans</span><span class="sxs-lookup"><span data-stu-id="eeb1f-151">recentPlans</span></span>|<span data-ttu-id="eeb1f-152">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="eeb1f-152">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="eeb1f-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-153">Read-only.</span></span> <span data-ttu-id="eeb1f-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-154">Nullable.</span></span> <span data-ttu-id="eeb1f-155">Retorna o [plannerPlans](plannerplan.md) exibidos recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-155">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eeb1f-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eeb1f-156">JSON representation</span></span>
<span data-ttu-id="eeb1f-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eeb1f-157">The following is a JSON representation of the resource.</span></span>

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
