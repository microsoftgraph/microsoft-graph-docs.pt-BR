---
title: Tipo de recurso plannerPlan
description: O recurso de **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte planejador.
ms.openlocfilehash: cd2990bc42929c4c501e676d05d7d643dd6f7d3d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007254"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="00295-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="00295-107">plannerPlan resource type</span></span>

<span data-ttu-id="00295-p102">O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md). Cada objeto de plano tem um objeto [details](plannerplandetails.md) que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="00295-p102">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md). It can also have a collection of [plannerBuckets](plannerbucket.md). Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="00295-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="00295-113">Methods</span></span>

| <span data-ttu-id="00295-114">Método</span><span class="sxs-lookup"><span data-stu-id="00295-114">Method</span></span>           | <span data-ttu-id="00295-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00295-115">Return Type</span></span>    |<span data-ttu-id="00295-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="00295-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00295-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="00295-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="00295-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="00295-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="00295-119">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="00295-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="00295-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="00295-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="00295-121">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="00295-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="00295-122">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="00295-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="00295-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="00295-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="00295-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="00295-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="00295-125">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="00295-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="00295-126">Atualizar</span><span class="sxs-lookup"><span data-stu-id="00295-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="00295-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="00295-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="00295-128">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="00295-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="00295-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00295-129">Properties</span></span>
| <span data-ttu-id="00295-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00295-130">Property</span></span>     | <span data-ttu-id="00295-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="00295-131">Type</span></span>   |<span data-ttu-id="00295-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="00295-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00295-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00295-133">createdDateTime</span></span>|<span data-ttu-id="00295-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00295-134">DateTimeOffset</span></span>|<span data-ttu-id="00295-p103">Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="00295-p103">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="00295-139">id</span><span class="sxs-lookup"><span data-stu-id="00295-139">id</span></span>|<span data-ttu-id="00295-140">String</span><span class="sxs-lookup"><span data-stu-id="00295-140">String</span></span>| <span data-ttu-id="00295-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00295-141">Read-only.</span></span> <span data-ttu-id="00295-142">ID do plano.</span><span class="sxs-lookup"><span data-stu-id="00295-142">ID of the plan.</span></span> <span data-ttu-id="00295-143">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="00295-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="00295-144">[Validação de formato](planner-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="00295-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="00295-145">owner</span><span class="sxs-lookup"><span data-stu-id="00295-145">owner</span></span>|<span data-ttu-id="00295-146">String</span><span class="sxs-lookup"><span data-stu-id="00295-146">String</span></span>|<span data-ttu-id="00295-147">ID do [grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="00295-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="00295-148">Um grupo válido deve existir antes que esse campo pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="00295-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="00295-149">Depois que ele for definido, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="00295-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="00295-150">title</span><span class="sxs-lookup"><span data-stu-id="00295-150">title</span></span>|<span data-ttu-id="00295-151">String</span><span class="sxs-lookup"><span data-stu-id="00295-151">String</span></span>|<span data-ttu-id="00295-p106">Obrigatório. Título do plano.</span><span class="sxs-lookup"><span data-stu-id="00295-p106">Required. Title of the plan.</span></span>|
|<span data-ttu-id="00295-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="00295-154">createdBy</span></span>|[<span data-ttu-id="00295-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="00295-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="00295-p107">Somente leitura. O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="00295-p107">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00295-158">Relações</span><span class="sxs-lookup"><span data-stu-id="00295-158">Relationships</span></span>
| <span data-ttu-id="00295-159">Relação</span><span class="sxs-lookup"><span data-stu-id="00295-159">Relationship</span></span> | <span data-ttu-id="00295-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="00295-160">Type</span></span>   |<span data-ttu-id="00295-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="00295-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00295-162">buckets</span><span class="sxs-lookup"><span data-stu-id="00295-162">buckets</span></span>|<span data-ttu-id="00295-163">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="00295-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="00295-p108">Somente leitura. Anulável. A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="00295-p108">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="00295-167">detalhes</span><span class="sxs-lookup"><span data-stu-id="00295-167">details</span></span>|[<span data-ttu-id="00295-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="00295-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="00295-p109">Somente leitura. Anulável. Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="00295-p109">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="00295-172">tarefas</span><span class="sxs-lookup"><span data-stu-id="00295-172">tasks</span></span>|<span data-ttu-id="00295-173">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="00295-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="00295-p110">Somente leitura. Anulável. A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="00295-p110">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00295-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00295-177">JSON representation</span></span>

<span data-ttu-id="00295-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00295-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->