---
title: Tipo de recurso plannerUser
description: 'O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um usuário. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f10810f6debf2346ed12484bac8e1f4bfd2f372
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526876"
---
# <a name="planneruser-resource-type"></a><span data-ttu-id="49663-103">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="49663-103">plannerUser resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49663-104">O recurso de **plannerUser** fornece acesso aos recursos do Planejador de um [usuário](user.md).</span><span class="sxs-lookup"><span data-stu-id="49663-104">The **plannerUser** resource provides access to Planner resources for a [user](user.md).</span></span> 


## <a name="methods"></a><span data-ttu-id="49663-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="49663-105">Methods</span></span>

| <span data-ttu-id="49663-106">Método</span><span class="sxs-lookup"><span data-stu-id="49663-106">Method</span></span>           | <span data-ttu-id="49663-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="49663-107">Return Type</span></span>    |<span data-ttu-id="49663-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="49663-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49663-109">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="49663-109">List tasks</span></span>](../api/planneruser-list-tasks.md) |<span data-ttu-id="49663-110">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="49663-110">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="49663-111">Obtenha o [plannerTasks](plannertask.md) atribuída ao usuário.</span><span class="sxs-lookup"><span data-stu-id="49663-111">Get the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|[<span data-ttu-id="49663-112">Lista favoritePlans</span><span class="sxs-lookup"><span data-stu-id="49663-112">List favoritePlans</span></span>](../api/planneruser-list-favoriteplans.md) |<span data-ttu-id="49663-113">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="49663-113">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="49663-114">Obtenha o [plannerPlans](plannerplan.md) marcado como favorito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="49663-114">Get the [plannerPlans](plannerplan.md) marked as favorite by the user.</span></span>|
|[<span data-ttu-id="49663-115">Lista recentPlans</span><span class="sxs-lookup"><span data-stu-id="49663-115">List recentPlans</span></span>](../api/planneruser-list-recentplans.md) |<span data-ttu-id="49663-116">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="49663-116">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="49663-117">Obtenha o [plannerPlans](plannerplan.md) visualizados recentemente pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="49663-117">Get the [plannerPlans](plannerplan.md) recently viewed by the user.</span></span>|
|[<span data-ttu-id="49663-118">Update</span><span class="sxs-lookup"><span data-stu-id="49663-118">Update</span></span>](../api/planneruser-update.md) | [<span data-ttu-id="49663-119">plannerUser</span><span class="sxs-lookup"><span data-stu-id="49663-119">plannerUser</span></span>](planneruser.md)| <span data-ttu-id="49663-120">Atualize um objeto **plannerUser** .</span><span class="sxs-lookup"><span data-stu-id="49663-120">Update a **plannerUser** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="49663-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49663-121">Properties</span></span>
| <span data-ttu-id="49663-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49663-122">Property</span></span>     | <span data-ttu-id="49663-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="49663-123">Type</span></span>   |<span data-ttu-id="49663-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="49663-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49663-125">id</span><span class="sxs-lookup"><span data-stu-id="49663-125">id</span></span>|<span data-ttu-id="49663-126">String</span><span class="sxs-lookup"><span data-stu-id="49663-126">String</span></span>| <span data-ttu-id="49663-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49663-127">Read-only.</span></span> <span data-ttu-id="49663-128">Identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="49663-128">Identifier of the plannerUser</span></span>|
|<span data-ttu-id="49663-129">favoritePlanReferences</span><span class="sxs-lookup"><span data-stu-id="49663-129">favoritePlanReferences</span></span>|[<span data-ttu-id="49663-130">plannerFavoritePlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="49663-130">plannerFavoritePlanReferenceCollection</span></span>](plannerfavoriteplanreferencecollection.md)| <span data-ttu-id="49663-131">Uma coleção que contém as referências para os planos de que o usuário tenha marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="49663-131">A collection containing the references to the plans that the user has marked as favorites.</span></span>|
|<span data-ttu-id="49663-132">recentPlanReferences</span><span class="sxs-lookup"><span data-stu-id="49663-132">recentPlanReferences</span></span>|[<span data-ttu-id="49663-133">plannerRecentPlanReferenceCollection</span><span class="sxs-lookup"><span data-stu-id="49663-133">plannerRecentPlanReferenceCollection</span></span>](plannerrecentplanreferencecollection.md)| <span data-ttu-id="49663-134">Uma coleção que contém referências para os planos que foram visualizados recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="49663-134">A collection containing references to the plans that were viewed recently by the user in apps that support recent plans.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49663-135">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="49663-135">Relationships</span></span>
| <span data-ttu-id="49663-136">Relação</span><span class="sxs-lookup"><span data-stu-id="49663-136">Relationship</span></span> | <span data-ttu-id="49663-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="49663-137">Type</span></span>   |<span data-ttu-id="49663-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="49663-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49663-139">tarefas</span><span class="sxs-lookup"><span data-stu-id="49663-139">tasks</span></span>|<span data-ttu-id="49663-140">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="49663-140">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="49663-p102">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="49663-p102">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="49663-144">favoritePlans</span><span class="sxs-lookup"><span data-stu-id="49663-144">favoritePlans</span></span>|<span data-ttu-id="49663-145">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="49663-145">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="49663-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49663-146">Read-only.</span></span> <span data-ttu-id="49663-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="49663-147">Nullable.</span></span> <span data-ttu-id="49663-148">Retorna o [plannerPlans](plannerplan.md) que o usuário marcado como Favoritos.</span><span class="sxs-lookup"><span data-stu-id="49663-148">Returns the [plannerPlans](plannerplan.md) that the user marked as favorites.</span></span>|
|<span data-ttu-id="49663-149">recentPlans</span><span class="sxs-lookup"><span data-stu-id="49663-149">recentPlans</span></span>|<span data-ttu-id="49663-150">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="49663-150">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="49663-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="49663-151">Read-only.</span></span> <span data-ttu-id="49663-152">Anulável.</span><span class="sxs-lookup"><span data-stu-id="49663-152">Nullable.</span></span> <span data-ttu-id="49663-153">Retorna o [plannerPlans](plannerplan.md) exibidos recentemente pelo usuário em aplicativos que suportam planos recentes.</span><span class="sxs-lookup"><span data-stu-id="49663-153">Returns the [plannerPlans](plannerplan.md) that have been recently viewed by the user in apps that support recent plans.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="49663-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49663-154">JSON representation</span></span>
<span data-ttu-id="49663-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49663-155">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/planneruser.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
