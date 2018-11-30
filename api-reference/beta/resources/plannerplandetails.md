---
title: Tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto plan tem um objeto de detalhes.
ms.openlocfilehash: 1cce5727666bca705da67fccd1a3edf370c68127
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039754"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="74e4e-104">Tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="74e4e-104">plannerPlanDetails resource type</span></span>

> <span data-ttu-id="74e4e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="74e4e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74e4e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="74e4e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74e4e-p103">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="74e4e-p103">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="74e4e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="74e4e-109">Methods</span></span>

| <span data-ttu-id="74e4e-110">Método</span><span class="sxs-lookup"><span data-stu-id="74e4e-110">Method</span></span>           | <span data-ttu-id="74e4e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74e4e-111">Return Type</span></span>    |<span data-ttu-id="74e4e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="74e4e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74e4e-113">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="74e4e-113">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="74e4e-114">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="74e4e-114">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="74e4e-115">Leia as propriedades e relacionamentos de um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="74e4e-115">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="74e4e-116">Update</span><span class="sxs-lookup"><span data-stu-id="74e4e-116">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="74e4e-117">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="74e4e-117">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="74e4e-118">Atualize um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="74e4e-118">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="74e4e-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74e4e-119">Properties</span></span>
| <span data-ttu-id="74e4e-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74e4e-120">Property</span></span>     | <span data-ttu-id="74e4e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="74e4e-121">Type</span></span>   |<span data-ttu-id="74e4e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="74e4e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74e4e-123">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="74e4e-123">categoryDescriptions</span></span>|[<span data-ttu-id="74e4e-124">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="74e4e-124">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="74e4e-125">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="74e4e-125">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="74e4e-126">id</span><span class="sxs-lookup"><span data-stu-id="74e4e-126">id</span></span>|<span data-ttu-id="74e4e-127">String</span><span class="sxs-lookup"><span data-stu-id="74e4e-127">String</span></span>| <span data-ttu-id="74e4e-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74e4e-128">Read-only.</span></span> <span data-ttu-id="74e4e-129">A identificação dos detalhes do plano.</span><span class="sxs-lookup"><span data-stu-id="74e4e-129">The ID of the plan details.</span></span> <span data-ttu-id="74e4e-130">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="74e4e-130">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="74e4e-131">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="74e4e-131">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="74e4e-132">sharedWith</span><span class="sxs-lookup"><span data-stu-id="74e4e-132">sharedWith</span></span>|[<span data-ttu-id="74e4e-133">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="74e4e-133">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="74e4e-134">O conjunto deste plano compartilhada com IDs de usuário.</span><span class="sxs-lookup"><span data-stu-id="74e4e-134">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="74e4e-135">Se você estiver usando o Office 365 grupos, use os API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="74e4e-135">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="74e4e-136">Você também pode adicionar membros existentes do grupo para este conjunto, embora não seja obrigatório na ordem para que eles possam acessar o plano pertencente ao grupo.</span><span class="sxs-lookup"><span data-stu-id="74e4e-136">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="74e4e-137">contextDetails</span><span class="sxs-lookup"><span data-stu-id="74e4e-137">contextDetails</span></span>|[<span data-ttu-id="74e4e-138">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="74e4e-138">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="74e4e-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74e4e-139">Read-only.</span></span> <span data-ttu-id="74e4e-140">Uma coleção de informações adicionais associadas entradas [plannerPlanContext](plannerplancontext.md) definidas para o contêiner de [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="74e4e-140">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="74e4e-141">Relações</span><span class="sxs-lookup"><span data-stu-id="74e4e-141">Relationships</span></span>
<span data-ttu-id="74e4e-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74e4e-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="74e4e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74e4e-143">JSON representation</span></span>
<span data-ttu-id="74e4e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74e4e-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
