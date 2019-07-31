---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61296138f1477219e85ae7fd372102b8c7fd3a47
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965884"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="d8e62-104">tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d8e62-104">plannerPlanDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8e62-105">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano.</span><span class="sxs-lookup"><span data-stu-id="d8e62-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="d8e62-106">Cada objeto [Plan](plannerplan.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="d8e62-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d8e62-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d8e62-107">Methods</span></span>

| <span data-ttu-id="d8e62-108">Método</span><span class="sxs-lookup"><span data-stu-id="d8e62-108">Method</span></span>           | <span data-ttu-id="d8e62-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d8e62-109">Return Type</span></span>    |<span data-ttu-id="d8e62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e62-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8e62-111">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d8e62-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="d8e62-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d8e62-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="d8e62-113">Leia as propriedades e os relacionamentos de um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="d8e62-113">Read the properties and relationships of a **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="d8e62-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="d8e62-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="d8e62-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d8e62-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="d8e62-116">Atualizar um objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="d8e62-116">Update a **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d8e62-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8e62-117">Properties</span></span>
| <span data-ttu-id="d8e62-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8e62-118">Property</span></span>     | <span data-ttu-id="d8e62-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8e62-119">Type</span></span>   |<span data-ttu-id="d8e62-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e62-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8e62-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d8e62-121">categoryDescriptions</span></span>|[<span data-ttu-id="d8e62-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="d8e62-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="d8e62-123">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="d8e62-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="d8e62-124">id</span><span class="sxs-lookup"><span data-stu-id="d8e62-124">id</span></span>|<span data-ttu-id="d8e62-125">String</span><span class="sxs-lookup"><span data-stu-id="d8e62-125">String</span></span>| <span data-ttu-id="d8e62-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8e62-126">Read-only.</span></span> <span data-ttu-id="d8e62-127">A identificação do plano de detalhes.</span><span class="sxs-lookup"><span data-stu-id="d8e62-127">The ID of the plan details.</span></span> <span data-ttu-id="d8e62-128">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d8e62-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d8e62-129">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="d8e62-129">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d8e62-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="d8e62-130">sharedWith</span></span>|[<span data-ttu-id="d8e62-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="d8e62-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="d8e62-132">O conjunto de IDs de usuário com o qual esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d8e62-132">The set of user IDs that this plan is shared with.</span></span> <span data-ttu-id="d8e62-133">Se você estiver usando grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="d8e62-133">If you are using Office 365 Groups, use the groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="d8e62-134">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário para que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="d8e62-134">You can also add existing members of the group to this collection, although it is not required in order for them to access the plan owned by the group.</span></span> |
|<span data-ttu-id="d8e62-135">contextDetails</span><span class="sxs-lookup"><span data-stu-id="d8e62-135">contextDetails</span></span>|[<span data-ttu-id="d8e62-136">plannerPlanContextDetailsCollection</span><span class="sxs-lookup"><span data-stu-id="d8e62-136">plannerPlanContextDetailsCollection</span></span>](plannerplancontextdetailscollection.md)|<span data-ttu-id="d8e62-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8e62-137">Read-only.</span></span> <span data-ttu-id="d8e62-138">Uma coleção de informações adicionais associadas às entradas [plannerPlanContext](plannerplancontext.md) definidas para o contêiner [plannerPlan](plannerplan.md) .</span><span class="sxs-lookup"><span data-stu-id="d8e62-138">A collection of additional information associated with [plannerPlanContext](plannerplancontext.md) entries that are defined for the [plannerPlan](plannerplan.md) container.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d8e62-139">Relações</span><span class="sxs-lookup"><span data-stu-id="d8e62-139">Relationships</span></span>
<span data-ttu-id="d8e62-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8e62-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d8e62-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8e62-141">JSON representation</span></span>
<span data-ttu-id="d8e62-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8e62-142">The following is a JSON representation of the resource.</span></span>

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
