---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d75bbf877fcd70203b71159b198f5bad5f1bc3f0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035186"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="116fa-104">tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="116fa-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="116fa-105">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano.</span><span class="sxs-lookup"><span data-stu-id="116fa-105">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="116fa-106">Cada objeto [Plan](plannerplan.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="116fa-106">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="116fa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="116fa-107">Methods</span></span>

| <span data-ttu-id="116fa-108">Método</span><span class="sxs-lookup"><span data-stu-id="116fa-108">Method</span></span>           | <span data-ttu-id="116fa-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="116fa-109">Return Type</span></span>    |<span data-ttu-id="116fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="116fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="116fa-111">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="116fa-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="116fa-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="116fa-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="116fa-113">Leia as propriedades e os relacionamentos do objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="116fa-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="116fa-114">Atualização</span><span class="sxs-lookup"><span data-stu-id="116fa-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="116fa-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="116fa-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="116fa-116">Atualize o objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="116fa-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="116fa-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="116fa-117">Properties</span></span>
| <span data-ttu-id="116fa-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="116fa-118">Property</span></span>     | <span data-ttu-id="116fa-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="116fa-119">Type</span></span>   |<span data-ttu-id="116fa-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="116fa-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="116fa-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="116fa-121">categoryDescriptions</span></span>|[<span data-ttu-id="116fa-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="116fa-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="116fa-123">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="116fa-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="116fa-124">id</span><span class="sxs-lookup"><span data-stu-id="116fa-124">id</span></span>|<span data-ttu-id="116fa-125">String</span><span class="sxs-lookup"><span data-stu-id="116fa-125">String</span></span>| <span data-ttu-id="116fa-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="116fa-126">Read-only.</span></span> <span data-ttu-id="116fa-127">ID do plano de detalhes.</span><span class="sxs-lookup"><span data-stu-id="116fa-127">ID of the plan details.</span></span> <span data-ttu-id="116fa-128">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="116fa-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="116fa-129">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="116fa-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="116fa-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="116fa-130">sharedWith</span></span>|[<span data-ttu-id="116fa-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="116fa-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="116fa-132">Conjunto de IDs de usuário com as quais esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="116fa-132">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="116fa-133">Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="116fa-133">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="116fa-134">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="116fa-134">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="116fa-135">Relações</span><span class="sxs-lookup"><span data-stu-id="116fa-135">Relationships</span></span>
<span data-ttu-id="116fa-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="116fa-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="116fa-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="116fa-137">JSON representation</span></span>
<span data-ttu-id="116fa-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="116fa-138">Here is a JSON representation of the resource.</span></span>

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
