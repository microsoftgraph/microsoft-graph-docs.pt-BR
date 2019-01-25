---
title: Tipo de recurso plannerPlan
description: O recurso de **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte planejador.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: f37f6ea08f2951256e2d7f94cf9abad7e8ac60b2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529548"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="20544-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="20544-107">plannerPlan resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20544-108">O recurso de **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="20544-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="20544-109">Um plano pode pertencer a um [grupo](group.md) e contém uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="20544-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="20544-110">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="20544-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="20544-111">Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="20544-111">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="20544-112">Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte [Planejador](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="20544-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="20544-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="20544-113">Methods</span></span>

| <span data-ttu-id="20544-114">Método</span><span class="sxs-lookup"><span data-stu-id="20544-114">Method</span></span>           | <span data-ttu-id="20544-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20544-115">Return Type</span></span>    |<span data-ttu-id="20544-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="20544-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20544-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="20544-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="20544-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="20544-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="20544-119">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="20544-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="20544-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="20544-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="20544-121">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="20544-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="20544-122">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="20544-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="20544-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="20544-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="20544-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="20544-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="20544-125">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="20544-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="20544-126">Atualizar</span><span class="sxs-lookup"><span data-stu-id="20544-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="20544-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="20544-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="20544-128">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="20544-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="20544-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20544-129">Properties</span></span>
| <span data-ttu-id="20544-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20544-130">Property</span></span>     | <span data-ttu-id="20544-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="20544-131">Type</span></span>   |<span data-ttu-id="20544-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="20544-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20544-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20544-133">createdDateTime</span></span>|<span data-ttu-id="20544-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20544-134">DateTimeOffset</span></span>|<span data-ttu-id="20544-p103">Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="20544-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="20544-139">id</span><span class="sxs-lookup"><span data-stu-id="20544-139">id</span></span>|<span data-ttu-id="20544-140">String</span><span class="sxs-lookup"><span data-stu-id="20544-140">String</span></span>| <span data-ttu-id="20544-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20544-141">Read-only.</span></span> <span data-ttu-id="20544-142">ID do plano.</span><span class="sxs-lookup"><span data-stu-id="20544-142">ID of the plan.</span></span> <span data-ttu-id="20544-143">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="20544-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="20544-144">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="20544-144">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="20544-145">owner</span><span class="sxs-lookup"><span data-stu-id="20544-145">owner</span></span>|<span data-ttu-id="20544-146">String</span><span class="sxs-lookup"><span data-stu-id="20544-146">String</span></span>|<span data-ttu-id="20544-147">ID do [grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="20544-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="20544-148">Um grupo válido deve existir antes que esse campo pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="20544-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="20544-149">Depois que ele for definido, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="20544-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="20544-150">title</span><span class="sxs-lookup"><span data-stu-id="20544-150">title</span></span>|<span data-ttu-id="20544-151">String</span><span class="sxs-lookup"><span data-stu-id="20544-151">String</span></span>|<span data-ttu-id="20544-p106">Obrigatório. Título do plano.</span><span class="sxs-lookup"><span data-stu-id="20544-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="20544-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="20544-154">createdBy</span></span>|[<span data-ttu-id="20544-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="20544-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="20544-p107">Somente leitura. O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="20544-p107">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="20544-158">contextos</span><span class="sxs-lookup"><span data-stu-id="20544-158">contexts</span></span>|[<span data-ttu-id="20544-159">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="20544-159">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="20544-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20544-160">Read-only.</span></span> <span data-ttu-id="20544-161">Experiências de usuário adicional no qual este plano for usado, representado como entradas de [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="20544-161">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20544-162">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="20544-162">Relationships</span></span>
| <span data-ttu-id="20544-163">Relação</span><span class="sxs-lookup"><span data-stu-id="20544-163">Relationship</span></span> | <span data-ttu-id="20544-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="20544-164">Type</span></span>   |<span data-ttu-id="20544-165">Descrição</span><span class="sxs-lookup"><span data-stu-id="20544-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20544-166">buckets</span><span class="sxs-lookup"><span data-stu-id="20544-166">buckets</span></span>|<span data-ttu-id="20544-167">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="20544-167">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="20544-p109">Somente leitura. Anulável. A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="20544-p109">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="20544-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="20544-171">details</span></span>|[<span data-ttu-id="20544-172">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="20544-172">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="20544-p110">Somente leitura. Anulável. Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="20544-p110">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="20544-176">tarefas</span><span class="sxs-lookup"><span data-stu-id="20544-176">tasks</span></span>|<span data-ttu-id="20544-177">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="20544-177">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="20544-p111">Somente leitura. Anulável. A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="20544-p111">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20544-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20544-181">JSON representation</span></span>

<span data-ttu-id="20544-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20544-182">Here is a JSON representation of the resource.</span></span>

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
