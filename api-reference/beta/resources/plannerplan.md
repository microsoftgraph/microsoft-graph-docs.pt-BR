---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Microsoft 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto plan tem um objeto de detalhes que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4763f268628a4609ac91d0597aeb4f55a2d406ce
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720988"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="b0135-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b0135-107">plannerPlan resource type</span></span>

<span data-ttu-id="b0135-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0135-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0135-109">O recurso **plannerPlan** representa um plano no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b0135-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="b0135-110">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="b0135-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="b0135-111">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="b0135-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="b0135-112">Cada objeto plan tem um [objeto de](plannerplandetails.md) detalhes que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="b0135-113">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="b0135-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="b0135-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0135-114">Methods</span></span>

| <span data-ttu-id="b0135-115">Método</span><span class="sxs-lookup"><span data-stu-id="b0135-115">Method</span></span>           | <span data-ttu-id="b0135-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0135-116">Return Type</span></span>    |<span data-ttu-id="b0135-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0135-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0135-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b0135-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="b0135-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b0135-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b0135-120">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="b0135-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="b0135-121">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="b0135-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="b0135-122">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="b0135-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b0135-123">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="b0135-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="b0135-124">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="b0135-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="b0135-125">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="b0135-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b0135-126">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="b0135-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="b0135-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="b0135-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="b0135-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="b0135-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="b0135-129">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="b0135-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0135-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0135-130">Properties</span></span>
| <span data-ttu-id="b0135-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0135-131">Property</span></span>     | <span data-ttu-id="b0135-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0135-132">Type</span></span>   |<span data-ttu-id="b0135-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0135-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0135-134">contêiner</span><span class="sxs-lookup"><span data-stu-id="b0135-134">container</span></span>|[<span data-ttu-id="b0135-135">plannerPlanContainer</span><span class="sxs-lookup"><span data-stu-id="b0135-135">plannerPlanContainer</span></span>](../resources/plannerplancontainer.md)|<span data-ttu-id="b0135-136">Identifica o contêiner do plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-136">Identifies the container of the plan.</span></span> <span data-ttu-id="b0135-137">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b0135-137">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="b0135-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0135-138">Required.</span></span>|
|<span data-ttu-id="b0135-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0135-139">createdDateTime</span></span>|<span data-ttu-id="b0135-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0135-140">DateTimeOffset</span></span>|<span data-ttu-id="b0135-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-141">Read-only.</span></span> <span data-ttu-id="b0135-142">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="b0135-142">Date and time at which the plan is created.</span></span> <span data-ttu-id="b0135-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b0135-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b0135-144">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="b0135-144">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="b0135-145">id</span><span class="sxs-lookup"><span data-stu-id="b0135-145">id</span></span>|<span data-ttu-id="b0135-146">String</span><span class="sxs-lookup"><span data-stu-id="b0135-146">String</span></span>| <span data-ttu-id="b0135-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-147">Read-only.</span></span> <span data-ttu-id="b0135-148">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-148">ID of the plan.</span></span> <span data-ttu-id="b0135-149">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="b0135-149">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b0135-150">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="b0135-150">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b0135-151">title</span><span class="sxs-lookup"><span data-stu-id="b0135-151">title</span></span>|<span data-ttu-id="b0135-152">String</span><span class="sxs-lookup"><span data-stu-id="b0135-152">String</span></span>|<span data-ttu-id="b0135-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0135-153">Required.</span></span> <span data-ttu-id="b0135-154">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-154">Title of the plan.</span></span>|
|<span data-ttu-id="b0135-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="b0135-155">createdBy</span></span>|[<span data-ttu-id="b0135-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="b0135-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="b0135-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-157">Read-only.</span></span> <span data-ttu-id="b0135-158">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-158">The user who created the plan.</span></span>|
|<span data-ttu-id="b0135-159">contexts</span><span class="sxs-lookup"><span data-stu-id="b0135-159">contexts</span></span>|[<span data-ttu-id="b0135-160">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="b0135-160">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="b0135-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-161">Read-only.</span></span> <span data-ttu-id="b0135-162">Experiências adicionais de usuário nas quais esse plano é usado, representadas como entradas [plannerPlanContext.](plannerplancontext.md)</span><span class="sxs-lookup"><span data-stu-id="b0135-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|
|<span data-ttu-id="b0135-163">owner (preterido)</span><span class="sxs-lookup"><span data-stu-id="b0135-163">owner (deprecated)</span></span> |<span data-ttu-id="b0135-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0135-164">String</span></span>| <span data-ttu-id="b0135-165">Use a **propriedade container** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="b0135-165">Use the **container** property instead.</span></span> <span data-ttu-id="b0135-166">ID do [grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-166">ID of the [group](group.md) that owns the plan.</span></span> <span data-ttu-id="b0135-167">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b0135-167">After it is set, this property can’t be updated.</span></span> <span data-ttu-id="b0135-168">Essa propriedade não retornará uma ID de grupo válida se o contêiner do plano não for um grupo.</span><span class="sxs-lookup"><span data-stu-id="b0135-168">This property will not return a valid group ID if the container of the plan is not a group.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0135-169">Relações</span><span class="sxs-lookup"><span data-stu-id="b0135-169">Relationships</span></span>
| <span data-ttu-id="b0135-170">Relação</span><span class="sxs-lookup"><span data-stu-id="b0135-170">Relationship</span></span> | <span data-ttu-id="b0135-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0135-171">Type</span></span>   |<span data-ttu-id="b0135-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0135-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0135-173">buckets</span><span class="sxs-lookup"><span data-stu-id="b0135-173">buckets</span></span>|<span data-ttu-id="b0135-174">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="b0135-174">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="b0135-175">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-175">Collection of buckets in the plan.</span></span> <span data-ttu-id="b0135-176">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-176">Read-only.</span></span> <span data-ttu-id="b0135-177">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b0135-177">Nullable.</span></span>|
|<span data-ttu-id="b0135-178">detalhes</span><span class="sxs-lookup"><span data-stu-id="b0135-178">details</span></span>|[<span data-ttu-id="b0135-179">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="b0135-179">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="b0135-180">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-180">Additional details about the plan.</span></span> <span data-ttu-id="b0135-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-181">Read-only.</span></span> <span data-ttu-id="b0135-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b0135-182">Nullable.</span></span> |
|<span data-ttu-id="b0135-183">tarefas</span><span class="sxs-lookup"><span data-stu-id="b0135-183">tasks</span></span>|<span data-ttu-id="b0135-184">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="b0135-184">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="b0135-185">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="b0135-185">Collection of tasks in the plan.</span></span> <span data-ttu-id="b0135-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0135-186">Read-only.</span></span> <span data-ttu-id="b0135-187">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b0135-187">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0135-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0135-188">JSON representation</span></span>

<span data-ttu-id="b0135-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0135-189">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "contexts": {
    "48#19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype19%3Ad128c63941b24733951ea7defd81e550%40thread%2Eskype": {
        "@odata.type": "#microsoft.graph.plannerPlanContext",
        "associationType": "Board",
        "createdDateTime": "2015-10-14T00:57:28.4698344Z",
        "displayNameSegments": [
            "Finance Team",
            "Budget Plans"
        ],
        "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
    }
  },
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "container": {
    "@odata.type": "microsoft.graph.plannerPlanContainer",
    "url": "String",
    "containerId": "String",
    "type": "String"
  },
  "title": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


