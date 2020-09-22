---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 727da0983ddcaffb158be14a578a5a81eacecab3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037385"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="378b7-104">tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="378b7-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="378b7-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="378b7-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="378b7-106">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano.</span><span class="sxs-lookup"><span data-stu-id="378b7-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="378b7-107">Cada objeto [Plan](plannerplan.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="378b7-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="378b7-108">Methods</span><span class="sxs-lookup"><span data-stu-id="378b7-108">Methods</span></span>

| <span data-ttu-id="378b7-109">Método</span><span class="sxs-lookup"><span data-stu-id="378b7-109">Method</span></span>           | <span data-ttu-id="378b7-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="378b7-110">Return Type</span></span>    |<span data-ttu-id="378b7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="378b7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="378b7-112">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="378b7-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="378b7-113">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="378b7-113">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="378b7-114">Leia as propriedades e os relacionamentos do objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="378b7-114">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="378b7-115">Atualização</span><span class="sxs-lookup"><span data-stu-id="378b7-115">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="378b7-116">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="378b7-116">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="378b7-117">Atualize o objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="378b7-117">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="378b7-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="378b7-118">Properties</span></span>
| <span data-ttu-id="378b7-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="378b7-119">Property</span></span>     | <span data-ttu-id="378b7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="378b7-120">Type</span></span>   |<span data-ttu-id="378b7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="378b7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="378b7-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="378b7-122">categoryDescriptions</span></span>|[<span data-ttu-id="378b7-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="378b7-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="378b7-124">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="378b7-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="378b7-125">id</span><span class="sxs-lookup"><span data-stu-id="378b7-125">id</span></span>|<span data-ttu-id="378b7-126">String</span><span class="sxs-lookup"><span data-stu-id="378b7-126">String</span></span>| <span data-ttu-id="378b7-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="378b7-127">Read-only.</span></span> <span data-ttu-id="378b7-128">ID do plano de detalhes.</span><span class="sxs-lookup"><span data-stu-id="378b7-128">ID of the plan details.</span></span> <span data-ttu-id="378b7-129">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="378b7-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="378b7-130">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="378b7-130">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="378b7-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="378b7-131">sharedWith</span></span>|[<span data-ttu-id="378b7-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="378b7-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="378b7-133">Conjunto de IDs de usuário com as quais esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="378b7-133">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="378b7-134">Se você estiver aproveitando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="378b7-134">If you are leveraging Microsoft 365 groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="378b7-135">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="378b7-135">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="378b7-136">Relações</span><span class="sxs-lookup"><span data-stu-id="378b7-136">Relationships</span></span>
<span data-ttu-id="378b7-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="378b7-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="378b7-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="378b7-138">JSON representation</span></span>
<span data-ttu-id="378b7-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="378b7-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
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

