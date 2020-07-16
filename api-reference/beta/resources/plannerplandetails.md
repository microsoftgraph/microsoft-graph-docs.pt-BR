---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: bb9c4d013594edbf1f0b722115bb4a0740726ebe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895598"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="cf1b2-104">tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="cf1b2-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="cf1b2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf1b2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf1b2-106">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="cf1b2-107">Cada objeto [Plan](plannerplan.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="cf1b2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cf1b2-108">Methods</span></span>

| <span data-ttu-id="cf1b2-109">Método</span><span class="sxs-lookup"><span data-stu-id="cf1b2-109">Method</span></span>           | <span data-ttu-id="cf1b2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cf1b2-110">Return Type</span></span>    |<span data-ttu-id="cf1b2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf1b2-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf1b2-112">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="cf1b2-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="cf1b2-113">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="cf1b2-113">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="cf1b2-114">Leia as propriedades e os relacionamentos de um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="cf1b2-114">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="cf1b2-115">Update</span><span class="sxs-lookup"><span data-stu-id="cf1b2-115">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="cf1b2-116">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="cf1b2-116">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="cf1b2-117">Atualizar um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="cf1b2-117">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf1b2-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf1b2-118">Properties</span></span>
| <span data-ttu-id="cf1b2-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf1b2-119">Property</span></span>     | <span data-ttu-id="cf1b2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf1b2-120">Type</span></span>   |<span data-ttu-id="cf1b2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf1b2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf1b2-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="cf1b2-122">categoryDescriptions</span></span>|[<span data-ttu-id="cf1b2-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="cf1b2-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="cf1b2-124">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="cf1b2-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="cf1b2-125">id</span><span class="sxs-lookup"><span data-stu-id="cf1b2-125">id</span></span>|<span data-ttu-id="cf1b2-126">String</span><span class="sxs-lookup"><span data-stu-id="cf1b2-126">String</span></span>| <span data-ttu-id="cf1b2-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-127">Read-only.</span></span> <span data-ttu-id="cf1b2-128">A identificação do plano de detalhes.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-128">The ID of the plan details.</span></span> <span data-ttu-id="cf1b2-129">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="cf1b2-130">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-130">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="cf1b2-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="cf1b2-131">sharedWith</span></span>|[<span data-ttu-id="cf1b2-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="cf1b2-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="cf1b2-133">O conjunto de IDs de usuário com o qual esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-133">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="cf1b2-134">Se você estiver usando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="cf1b2-134">If you are using Microsoft 365 groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="cf1b2-135">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário para que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-135">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="cf1b2-136">contextDetails</span><span class="sxs-lookup"><span data-stu-id="cf1b2-136">contextDetails</span></span>|[<span data-ttu-id="cf1b2-137">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="cf1b2-137">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="cf1b2-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-138">Read-only.</span></span> <span data-ttu-id="cf1b2-139">Uma coleção de informações adicionais associadas às entradas [plannerPlanContext](plannerplancontext.md) definidas para o contêiner [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="cf1b2-139">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf1b2-140">Relações</span><span class="sxs-lookup"><span data-stu-id="cf1b2-140">Relationships</span></span>
<span data-ttu-id="cf1b2-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf1b2-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cf1b2-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf1b2-142">JSON representation</span></span>
<span data-ttu-id="cf1b2-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf1b2-143">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
