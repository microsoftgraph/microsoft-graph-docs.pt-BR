---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto Plan tem um objeto Details que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 5da918e3ba0e8087d4572799168fa1132e0ce5e7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344458"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="78420-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="78420-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78420-108">O recurso **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="78420-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="78420-109">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de plannerTasks.</span><span class="sxs-lookup"><span data-stu-id="78420-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="78420-110">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="78420-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="78420-111">Cada objeto Plan tem um objeto [Details](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="78420-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="78420-112">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="78420-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="78420-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="78420-113">Methods</span></span>

| <span data-ttu-id="78420-114">Método</span><span class="sxs-lookup"><span data-stu-id="78420-114">Method</span></span>           | <span data-ttu-id="78420-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78420-115">Return Type</span></span>    |<span data-ttu-id="78420-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="78420-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="78420-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="78420-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="78420-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="78420-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="78420-119">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="78420-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="78420-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="78420-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="78420-121">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="78420-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="78420-122">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="78420-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="78420-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="78420-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="78420-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="78420-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="78420-125">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="78420-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="78420-126">Atualizar</span><span class="sxs-lookup"><span data-stu-id="78420-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="78420-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="78420-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="78420-128">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="78420-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="78420-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78420-129">Properties</span></span>
| <span data-ttu-id="78420-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78420-130">Property</span></span>     | <span data-ttu-id="78420-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="78420-131">Type</span></span>   |<span data-ttu-id="78420-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="78420-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78420-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78420-133">createdDateTime</span></span>|<span data-ttu-id="78420-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78420-134">DateTimeOffset</span></span>|<span data-ttu-id="78420-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-135">Read-only.</span></span> <span data-ttu-id="78420-136">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="78420-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="78420-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="78420-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="78420-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="78420-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="78420-139">id</span><span class="sxs-lookup"><span data-stu-id="78420-139">id</span></span>|<span data-ttu-id="78420-140">String</span><span class="sxs-lookup"><span data-stu-id="78420-140">String</span></span>| <span data-ttu-id="78420-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-141">Read-only.</span></span> <span data-ttu-id="78420-142">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="78420-142">ID of the plan.</span></span> <span data-ttu-id="78420-143">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="78420-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="78420-144">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="78420-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="78420-145">owner</span><span class="sxs-lookup"><span data-stu-id="78420-145">owner</span></span>|<span data-ttu-id="78420-146">String</span><span class="sxs-lookup"><span data-stu-id="78420-146">String</span></span>|<span data-ttu-id="78420-147">A ID do [Grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="78420-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="78420-148">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="78420-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="78420-149">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="78420-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="78420-150">title</span><span class="sxs-lookup"><span data-stu-id="78420-150">title</span></span>|<span data-ttu-id="78420-151">String</span><span class="sxs-lookup"><span data-stu-id="78420-151">String</span></span>|<span data-ttu-id="78420-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78420-152">Required.</span></span> <span data-ttu-id="78420-153">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="78420-153">Title of the plan.</span></span>|
|<span data-ttu-id="78420-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="78420-154">createdBy</span></span>|[<span data-ttu-id="78420-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="78420-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="78420-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-156">Read-only.</span></span> <span data-ttu-id="78420-157">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="78420-157">The user who created the plan.</span></span>|
|<span data-ttu-id="78420-158">contextos</span><span class="sxs-lookup"><span data-stu-id="78420-158">contexts</span></span>|[<span data-ttu-id="78420-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="78420-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="78420-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-160">Read-only.</span></span> <span data-ttu-id="78420-161">Experiências de usuário adicionais nas quais esse plano é usado, representado como entradas [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="78420-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78420-162">Relações</span><span class="sxs-lookup"><span data-stu-id="78420-162">Relationships</span></span>
| <span data-ttu-id="78420-163">Relação</span><span class="sxs-lookup"><span data-stu-id="78420-163">Relationship</span></span> | <span data-ttu-id="78420-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="78420-164">Type</span></span>   |<span data-ttu-id="78420-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="78420-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78420-166">buckets</span><span class="sxs-lookup"><span data-stu-id="78420-166">buckets</span></span>|<span data-ttu-id="78420-167">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="78420-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="78420-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-168">Read-only.</span></span> <span data-ttu-id="78420-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="78420-169">Nullable.</span></span> <span data-ttu-id="78420-170">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="78420-170">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="78420-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="78420-171">details</span></span>|[<span data-ttu-id="78420-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="78420-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="78420-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-173">Read-only.</span></span> <span data-ttu-id="78420-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="78420-174">Nullable.</span></span> <span data-ttu-id="78420-175">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="78420-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="78420-176">tarefas</span><span class="sxs-lookup"><span data-stu-id="78420-176">tasks</span></span>|<span data-ttu-id="78420-177">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="78420-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="78420-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78420-178">Read-only.</span></span> <span data-ttu-id="78420-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="78420-179">Nullable.</span></span> <span data-ttu-id="78420-180">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="78420-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78420-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78420-181">JSON representation</span></span>

<span data-ttu-id="78420-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78420-182">Here is a JSON representation of the resource.</span></span>

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
