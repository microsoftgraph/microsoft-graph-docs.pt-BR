---
title: Tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto plan tem um objeto de detalhes.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9d10f5b04bc3b98a5e32eac7b577cbf4c582bab4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529877"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="40b09-104">Tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="40b09-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40b09-p102">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="40b09-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="40b09-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="40b09-107">Methods</span></span>

| <span data-ttu-id="40b09-108">Método</span><span class="sxs-lookup"><span data-stu-id="40b09-108">Method</span></span>           | <span data-ttu-id="40b09-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40b09-109">Return Type</span></span>    |<span data-ttu-id="40b09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b09-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40b09-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="40b09-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="40b09-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="40b09-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="40b09-113">Leia as propriedades e relacionamentos de um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="40b09-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="40b09-114">Update</span><span class="sxs-lookup"><span data-stu-id="40b09-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="40b09-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="40b09-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="40b09-116">Atualize um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="40b09-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="40b09-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b09-117">Properties</span></span>
| <span data-ttu-id="40b09-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b09-118">Property</span></span>     | <span data-ttu-id="40b09-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b09-119">Type</span></span>   |<span data-ttu-id="40b09-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b09-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b09-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="40b09-121">categoryDescriptions</span></span>|[<span data-ttu-id="40b09-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="40b09-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="40b09-123">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="40b09-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="40b09-124">id</span><span class="sxs-lookup"><span data-stu-id="40b09-124">id</span></span>|<span data-ttu-id="40b09-125">String</span><span class="sxs-lookup"><span data-stu-id="40b09-125">String</span></span>| <span data-ttu-id="40b09-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b09-126">Read-only.</span></span> <span data-ttu-id="40b09-127">A identificação dos detalhes do plano.</span><span class="sxs-lookup"><span data-stu-id="40b09-127">The ID of the plan details.</span></span> <span data-ttu-id="40b09-128">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="40b09-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="40b09-129">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="40b09-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="40b09-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="40b09-130">sharedWith</span></span>|[<span data-ttu-id="40b09-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="40b09-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="40b09-132">O conjunto deste plano compartilhada com IDs de usuário.</span><span class="sxs-lookup"><span data-stu-id="40b09-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="40b09-133">Se você estiver usando o Office 365 grupos, use os API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="40b09-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="40b09-134">Você também pode adicionar membros existentes do grupo para este conjunto, embora não seja obrigatório na ordem para que eles possam acessar o plano pertencente ao grupo.</span><span class="sxs-lookup"><span data-stu-id="40b09-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="40b09-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="40b09-135">contextDetails</span></span>|[<span data-ttu-id="40b09-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="40b09-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="40b09-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b09-137">Read-only.</span></span> <span data-ttu-id="40b09-138">Uma coleção de informações adicionais associadas entradas [plannerPlanContext](plannerplancontext.md) definidas para o contêiner de [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="40b09-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="40b09-139">Relações</span><span class="sxs-lookup"><span data-stu-id="40b09-139">Relationships</span></span>
<span data-ttu-id="40b09-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b09-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="40b09-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b09-141">JSON representation</span></span>
<span data-ttu-id="40b09-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40b09-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "contextDetails": {"@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplandetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
