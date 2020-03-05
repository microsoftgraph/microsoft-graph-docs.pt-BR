---
title: tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto Plan tem um objeto details.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: e06afabfa01e7c63f103208bb0f290bcb58e4c56
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447105"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="a97bd-104">tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a97bd-104">plannerPlanDetails resource type</span></span>

<span data-ttu-id="a97bd-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a97bd-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="a97bd-106">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano.</span><span class="sxs-lookup"><span data-stu-id="a97bd-106">The **plannerPlanDetails** resource represents the additional information about a plan.</span></span> <span data-ttu-id="a97bd-107">Cada objeto [Plan](plannerplan.md) tem um objeto details.</span><span class="sxs-lookup"><span data-stu-id="a97bd-107">Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="a97bd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="a97bd-108">Methods</span></span>

| <span data-ttu-id="a97bd-109">Método</span><span class="sxs-lookup"><span data-stu-id="a97bd-109">Method</span></span>           | <span data-ttu-id="a97bd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a97bd-110">Return Type</span></span>    |<span data-ttu-id="a97bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97bd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a97bd-112">Obter plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a97bd-112">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="a97bd-113">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a97bd-113">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="a97bd-114">Leia as propriedades e os relacionamentos do objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="a97bd-114">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="a97bd-115">Update</span><span class="sxs-lookup"><span data-stu-id="a97bd-115">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="a97bd-116">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="a97bd-116">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="a97bd-117">Atualize o objeto **plannerPlanDetails** .</span><span class="sxs-lookup"><span data-stu-id="a97bd-117">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a97bd-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a97bd-118">Properties</span></span>
| <span data-ttu-id="a97bd-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a97bd-119">Property</span></span>     | <span data-ttu-id="a97bd-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a97bd-120">Type</span></span>   |<span data-ttu-id="a97bd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a97bd-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a97bd-122">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a97bd-122">categoryDescriptions</span></span>|[<span data-ttu-id="a97bd-123">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="a97bd-123">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="a97bd-124">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="a97bd-124">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="a97bd-125">id</span><span class="sxs-lookup"><span data-stu-id="a97bd-125">id</span></span>|<span data-ttu-id="a97bd-126">String</span><span class="sxs-lookup"><span data-stu-id="a97bd-126">String</span></span>| <span data-ttu-id="a97bd-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a97bd-127">Read-only.</span></span> <span data-ttu-id="a97bd-128">ID do plano de detalhes.</span><span class="sxs-lookup"><span data-stu-id="a97bd-128">ID of the plan details.</span></span> <span data-ttu-id="a97bd-129">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a97bd-129">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a97bd-130">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="a97bd-130">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a97bd-131">sharedWith</span><span class="sxs-lookup"><span data-stu-id="a97bd-131">sharedWith</span></span>|[<span data-ttu-id="a97bd-132">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="a97bd-132">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="a97bd-133">Conjunto de IDs de usuário com as quais esse plano é compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a97bd-133">Set of user ids that this plan is shared with.</span></span> <span data-ttu-id="a97bd-134">Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) .</span><span class="sxs-lookup"><span data-stu-id="a97bd-134">If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan.</span></span> <span data-ttu-id="a97bd-135">Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.</span><span class="sxs-lookup"><span data-stu-id="a97bd-135">You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a97bd-136">Relações</span><span class="sxs-lookup"><span data-stu-id="a97bd-136">Relationships</span></span>
<span data-ttu-id="a97bd-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a97bd-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a97bd-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a97bd-138">JSON representation</span></span>
<span data-ttu-id="a97bd-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a97bd-139">Here is a JSON representation of the resource.</span></span>

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
