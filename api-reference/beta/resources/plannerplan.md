---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Microsoft 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto Plan tem um objeto Details que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 386eff2e771967231a5c37d73ea913252e5d3324
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979333"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="2f3f1-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2f3f1-107">plannerPlan resource type</span></span>

<span data-ttu-id="2f3f1-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f3f1-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f3f1-109">O recurso **plannerPlan** representa um plano no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="2f3f1-110">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="2f3f1-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="2f3f1-111">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="2f3f1-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="2f3f1-112">Cada objeto Plan tem um objeto [Details](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-112">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="2f3f1-113">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2f3f1-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="2f3f1-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f3f1-114">Methods</span></span>

| <span data-ttu-id="2f3f1-115">Método</span><span class="sxs-lookup"><span data-stu-id="2f3f1-115">Method</span></span>           | <span data-ttu-id="2f3f1-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2f3f1-116">Return Type</span></span>    |<span data-ttu-id="2f3f1-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f3f1-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f3f1-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2f3f1-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="2f3f1-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2f3f1-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="2f3f1-120">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="2f3f1-121">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="2f3f1-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="2f3f1-122">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2f3f1-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2f3f1-123">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="2f3f1-124">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="2f3f1-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="2f3f1-125">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2f3f1-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2f3f1-126">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="2f3f1-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2f3f1-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="2f3f1-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2f3f1-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="2f3f1-129">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2f3f1-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f3f1-130">Properties</span></span>
| <span data-ttu-id="2f3f1-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f3f1-131">Property</span></span>     | <span data-ttu-id="2f3f1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f3f1-132">Type</span></span>   |<span data-ttu-id="2f3f1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f3f1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f3f1-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f3f1-134">createdDateTime</span></span>|<span data-ttu-id="2f3f1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f3f1-135">DateTimeOffset</span></span>|<span data-ttu-id="2f3f1-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-136">Read-only.</span></span> <span data-ttu-id="2f3f1-137">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="2f3f1-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2f3f1-139">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2f3f1-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2f3f1-140">id</span><span class="sxs-lookup"><span data-stu-id="2f3f1-140">id</span></span>|<span data-ttu-id="2f3f1-141">String</span><span class="sxs-lookup"><span data-stu-id="2f3f1-141">String</span></span>| <span data-ttu-id="2f3f1-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-142">Read-only.</span></span> <span data-ttu-id="2f3f1-143">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-143">ID of the plan.</span></span> <span data-ttu-id="2f3f1-144">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2f3f1-145">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-145">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2f3f1-146">owner</span><span class="sxs-lookup"><span data-stu-id="2f3f1-146">owner</span></span>|<span data-ttu-id="2f3f1-147">String</span><span class="sxs-lookup"><span data-stu-id="2f3f1-147">String</span></span>|<span data-ttu-id="2f3f1-148">A ID do [Grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="2f3f1-149">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="2f3f1-150">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="2f3f1-151">title</span><span class="sxs-lookup"><span data-stu-id="2f3f1-151">title</span></span>|<span data-ttu-id="2f3f1-152">String</span><span class="sxs-lookup"><span data-stu-id="2f3f1-152">String</span></span>|<span data-ttu-id="2f3f1-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-153">Required.</span></span> <span data-ttu-id="2f3f1-154">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-154">Title of the plan.</span></span>|
|<span data-ttu-id="2f3f1-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="2f3f1-155">createdBy</span></span>|[<span data-ttu-id="2f3f1-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="2f3f1-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="2f3f1-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-157">Read-only.</span></span> <span data-ttu-id="2f3f1-158">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-158">The user who created the plan.</span></span>|
|<span data-ttu-id="2f3f1-159">contextos</span><span class="sxs-lookup"><span data-stu-id="2f3f1-159">contexts</span></span>|[<span data-ttu-id="2f3f1-160">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="2f3f1-160">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="2f3f1-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-161">Read-only.</span></span> <span data-ttu-id="2f3f1-162">Experiências de usuário adicionais nas quais esse plano é usado, representado como entradas [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="2f3f1-162">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f3f1-163">Relações</span><span class="sxs-lookup"><span data-stu-id="2f3f1-163">Relationships</span></span>
| <span data-ttu-id="2f3f1-164">Relação</span><span class="sxs-lookup"><span data-stu-id="2f3f1-164">Relationship</span></span> | <span data-ttu-id="2f3f1-165">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f3f1-165">Type</span></span>   |<span data-ttu-id="2f3f1-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f3f1-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f3f1-167">buckets</span><span class="sxs-lookup"><span data-stu-id="2f3f1-167">buckets</span></span>|<span data-ttu-id="2f3f1-168">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2f3f1-168">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2f3f1-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-169">Read-only.</span></span> <span data-ttu-id="2f3f1-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-170">Nullable.</span></span> <span data-ttu-id="2f3f1-171">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-171">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="2f3f1-172">detalhes</span><span class="sxs-lookup"><span data-stu-id="2f3f1-172">details</span></span>|[<span data-ttu-id="2f3f1-173">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="2f3f1-173">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="2f3f1-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-174">Read-only.</span></span> <span data-ttu-id="2f3f1-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-175">Nullable.</span></span> <span data-ttu-id="2f3f1-176">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-176">Additional details about the plan.</span></span>|
|<span data-ttu-id="2f3f1-177">tarefas</span><span class="sxs-lookup"><span data-stu-id="2f3f1-177">tasks</span></span>|<span data-ttu-id="2f3f1-178">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2f3f1-178">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2f3f1-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-179">Read-only.</span></span> <span data-ttu-id="2f3f1-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-180">Nullable.</span></span> <span data-ttu-id="2f3f1-181">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-181">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f3f1-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f3f1-182">JSON representation</span></span>

<span data-ttu-id="2f3f1-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f3f1-183">Here is a JSON representation of the resource.</span></span>

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
  "owner": "String",
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


