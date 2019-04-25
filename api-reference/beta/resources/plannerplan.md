---
title: tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Também pode ter uma coleção de plannerBuckets. Cada objeto Plan tem um objeto Details que pode conter mais informações sobre o plano. Para obter mais informações sobre as relações entre grupos, planos e tarefas, consulte Planner.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578864"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="d0a55-107">tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0a55-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0a55-108">O recurso **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="d0a55-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="d0a55-109">Um plano pode pertencer a um [grupo](group.md) e contém uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="d0a55-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="d0a55-110">Também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="d0a55-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="d0a55-111">Cada objeto Plan tem um objeto [Details](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="d0a55-112">Para obter mais informações sobre as relações entre grupos, planos e tarefas, consulte [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="d0a55-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="d0a55-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="d0a55-113">Methods</span></span>

| <span data-ttu-id="d0a55-114">Método</span><span class="sxs-lookup"><span data-stu-id="d0a55-114">Method</span></span>           | <span data-ttu-id="d0a55-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d0a55-115">Return Type</span></span>    |<span data-ttu-id="d0a55-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a55-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d0a55-117">Obter plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0a55-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="d0a55-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0a55-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="d0a55-119">Leia as propriedades e os relacionamentos do objeto **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="d0a55-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="d0a55-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="d0a55-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="d0a55-121">coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d0a55-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d0a55-122">Obtenha uma coleção de objetos **plannerBucket** .</span><span class="sxs-lookup"><span data-stu-id="d0a55-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="d0a55-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="d0a55-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="d0a55-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d0a55-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d0a55-125">Obtenha uma coleção de objetos **plannerTask** .</span><span class="sxs-lookup"><span data-stu-id="d0a55-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="d0a55-126">Update</span><span class="sxs-lookup"><span data-stu-id="d0a55-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="d0a55-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="d0a55-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="d0a55-128">Atualize o objeto **plannerPlan** .</span><span class="sxs-lookup"><span data-stu-id="d0a55-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0a55-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0a55-129">Properties</span></span>
| <span data-ttu-id="d0a55-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0a55-130">Property</span></span>     | <span data-ttu-id="d0a55-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0a55-131">Type</span></span>   |<span data-ttu-id="d0a55-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a55-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0a55-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0a55-133">createdDateTime</span></span>|<span data-ttu-id="d0a55-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0a55-134">DateTimeOffset</span></span>|<span data-ttu-id="d0a55-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-135">Read-only.</span></span> <span data-ttu-id="d0a55-136">Data e hora em que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="d0a55-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="d0a55-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d0a55-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d0a55-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d0a55-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d0a55-139">id</span><span class="sxs-lookup"><span data-stu-id="d0a55-139">id</span></span>|<span data-ttu-id="d0a55-140">String</span><span class="sxs-lookup"><span data-stu-id="d0a55-140">String</span></span>| <span data-ttu-id="d0a55-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-141">Read-only.</span></span> <span data-ttu-id="d0a55-142">ID do plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-142">ID of the plan.</span></span> <span data-ttu-id="d0a55-143">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d0a55-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d0a55-144">[Formatar validação](tasks-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="d0a55-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d0a55-145">owner</span><span class="sxs-lookup"><span data-stu-id="d0a55-145">owner</span></span>|<span data-ttu-id="d0a55-146">String</span><span class="sxs-lookup"><span data-stu-id="d0a55-146">String</span></span>|<span data-ttu-id="d0a55-147">ID do [grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="d0a55-148">Um grupo válido deve existir antes que este campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="d0a55-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="d0a55-149">Após a definição, esta propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="d0a55-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="d0a55-150">title</span><span class="sxs-lookup"><span data-stu-id="d0a55-150">title</span></span>|<span data-ttu-id="d0a55-151">String</span><span class="sxs-lookup"><span data-stu-id="d0a55-151">String</span></span>|<span data-ttu-id="d0a55-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d0a55-152">Required.</span></span> <span data-ttu-id="d0a55-153">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-153">Title of the plan.</span></span>|
|<span data-ttu-id="d0a55-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="d0a55-154">createdBy</span></span>|[<span data-ttu-id="d0a55-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="d0a55-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="d0a55-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-156">Read-only.</span></span> <span data-ttu-id="d0a55-157">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-157">The user who created the plan.</span></span>|
|<span data-ttu-id="d0a55-158">contextos</span><span class="sxs-lookup"><span data-stu-id="d0a55-158">contexts</span></span>|[<span data-ttu-id="d0a55-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="d0a55-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="d0a55-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-160">Read-only.</span></span> <span data-ttu-id="d0a55-161">Experiências de usuário adicionais nas quais esse plano é usado, representado como entradas [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="d0a55-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0a55-162">Relações</span><span class="sxs-lookup"><span data-stu-id="d0a55-162">Relationships</span></span>
| <span data-ttu-id="d0a55-163">Relação</span><span class="sxs-lookup"><span data-stu-id="d0a55-163">Relationship</span></span> | <span data-ttu-id="d0a55-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0a55-164">Type</span></span>   |<span data-ttu-id="d0a55-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0a55-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0a55-166">buckets</span><span class="sxs-lookup"><span data-stu-id="d0a55-166">buckets</span></span>|<span data-ttu-id="d0a55-167">coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="d0a55-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="d0a55-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-168">Read-only.</span></span> <span data-ttu-id="d0a55-169">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d0a55-169">Nullable.</span></span> <span data-ttu-id="d0a55-170">Conjunto de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-170">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="d0a55-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="d0a55-171">details</span></span>|[<span data-ttu-id="d0a55-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="d0a55-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="d0a55-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-173">Read-only.</span></span> <span data-ttu-id="d0a55-174">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d0a55-174">Nullable.</span></span> <span data-ttu-id="d0a55-175">Detalhes adicionais sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-175">Additional details about the plan.</span></span>|
|<span data-ttu-id="d0a55-176">tarefas</span><span class="sxs-lookup"><span data-stu-id="d0a55-176">tasks</span></span>|<span data-ttu-id="d0a55-177">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="d0a55-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="d0a55-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d0a55-178">Read-only.</span></span> <span data-ttu-id="d0a55-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d0a55-179">Nullable.</span></span> <span data-ttu-id="d0a55-180">Conjunto de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="d0a55-180">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0a55-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0a55-181">JSON representation</span></span>

<span data-ttu-id="d0a55-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0a55-182">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplan.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
