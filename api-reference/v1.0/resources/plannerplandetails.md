---
title: Tipo de recurso plannerPlanDetails
description: O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto plan tem um objeto de detalhes.
localization_priority: Normal
ms.openlocfilehash: 59064093b485b6c82bd5b2e0b59ca1868e8517e4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867736"
---
# <a name="plannerplandetails-resource-type"></a><span data-ttu-id="7b55e-104">Tipo de recurso plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7b55e-104">plannerPlanDetails resource type</span></span>


<span data-ttu-id="7b55e-p102">O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="7b55e-p102">The **plannerPlanDetails** resource represents the additional information about a plan. Each [plan](plannerplan.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="7b55e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b55e-107">Methods</span></span>

| <span data-ttu-id="7b55e-108">Método</span><span class="sxs-lookup"><span data-stu-id="7b55e-108">Method</span></span>           | <span data-ttu-id="7b55e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b55e-109">Return Type</span></span>    |<span data-ttu-id="7b55e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b55e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b55e-111">Get plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7b55e-111">Get plannerPlanDetails</span></span>](../api/plannerplandetails-get.md) | [<span data-ttu-id="7b55e-112">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7b55e-112">plannerPlanDetails</span></span>](plannerplandetails.md) |<span data-ttu-id="7b55e-113">Leia as propriedades e as relações do objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="7b55e-113">Read properties and relationships of **plannerPlanDetails** object.</span></span>|
|[<span data-ttu-id="7b55e-114">Update</span><span class="sxs-lookup"><span data-stu-id="7b55e-114">Update</span></span>](../api/plannerplandetails-update.md) | [<span data-ttu-id="7b55e-115">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="7b55e-115">plannerPlanDetails</span></span>](plannerplandetails.md)    |<span data-ttu-id="7b55e-116">Atualize o objeto **plannerPlanDetails**.</span><span class="sxs-lookup"><span data-stu-id="7b55e-116">Update **plannerPlanDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7b55e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b55e-117">Properties</span></span>
| <span data-ttu-id="7b55e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b55e-118">Property</span></span>     | <span data-ttu-id="7b55e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b55e-119">Type</span></span>   |<span data-ttu-id="7b55e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b55e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b55e-121">categoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7b55e-121">categoryDescriptions</span></span>|[<span data-ttu-id="7b55e-122">plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="7b55e-122">plannerCategoryDescriptions</span></span>](plannercategorydescriptions.md)|<span data-ttu-id="7b55e-123">Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano</span><span class="sxs-lookup"><span data-stu-id="7b55e-123">An object that specifies the descriptions of the six categories that can be associated with tasks in the plan</span></span>|
|<span data-ttu-id="7b55e-124">id</span><span class="sxs-lookup"><span data-stu-id="7b55e-124">id</span></span>|<span data-ttu-id="7b55e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7b55e-125">String</span></span>| <span data-ttu-id="7b55e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b55e-126">Read-only.</span></span> <span data-ttu-id="7b55e-127">ID dos detalhes do plano.</span><span class="sxs-lookup"><span data-stu-id="7b55e-127">ID of the plan details.</span></span> <span data-ttu-id="7b55e-128">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="7b55e-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7b55e-129">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="7b55e-129">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7b55e-130">sharedWith</span><span class="sxs-lookup"><span data-stu-id="7b55e-130">sharedWith</span></span>|[<span data-ttu-id="7b55e-131">plannerUserIds</span><span class="sxs-lookup"><span data-stu-id="7b55e-131">plannerUserIds</span></span>](planneruserids.md)|<span data-ttu-id="7b55e-p104">Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo.</span><span class="sxs-lookup"><span data-stu-id="7b55e-p104">Set of user ids that this plan is shared with. If you are leveraging Office 365 Groups, use the Groups API to manage group membership to share the [group's](group.md) plan. You can also add existing members of the group to this collection though it is not required for them to access the plan owned by the group.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7b55e-135">Relações</span><span class="sxs-lookup"><span data-stu-id="7b55e-135">Relationships</span></span>
<span data-ttu-id="7b55e-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b55e-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b55e-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b55e-137">JSON representation</span></span>
<span data-ttu-id="7b55e-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b55e-138">Here is a JSON representation of the resource.</span></span>

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
