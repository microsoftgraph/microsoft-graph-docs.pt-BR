---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1f928252963c7796a396e1e342b413d135fb1764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035179"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="9b454-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9b454-107">plannerPlan resource type</span></span>

<span data-ttu-id="9b454-108">O recurso **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="9b454-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="9b454-109">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="9b454-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="9b454-110">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="9b454-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="9b454-111">Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="9b454-112">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9b454-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9b454-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b454-113">Methods</span></span>

| <span data-ttu-id="9b454-114">Método</span><span class="sxs-lookup"><span data-stu-id="9b454-114">Method</span></span>           | <span data-ttu-id="9b454-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b454-115">Return Type</span></span>    |<span data-ttu-id="9b454-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b454-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b454-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9b454-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="9b454-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9b454-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="9b454-119">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="9b454-119">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="9b454-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="9b454-120">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="9b454-121">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="9b454-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="9b454-122">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="9b454-122">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="9b454-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="9b454-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="9b454-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9b454-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9b454-125">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="9b454-125">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="9b454-126">Atualizar</span><span class="sxs-lookup"><span data-stu-id="9b454-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="9b454-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9b454-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="9b454-128">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="9b454-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9b454-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b454-129">Properties</span></span>
| <span data-ttu-id="9b454-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b454-130">Property</span></span>     | <span data-ttu-id="9b454-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b454-131">Type</span></span>   |<span data-ttu-id="9b454-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b454-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b454-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b454-133">createdDateTime</span></span>|<span data-ttu-id="9b454-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b454-134">DateTimeOffset</span></span>|<span data-ttu-id="9b454-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-135">Read-only.</span></span> <span data-ttu-id="9b454-136">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="9b454-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="9b454-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9b454-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9b454-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9b454-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9b454-139">id</span><span class="sxs-lookup"><span data-stu-id="9b454-139">id</span></span>|<span data-ttu-id="9b454-140">String</span><span class="sxs-lookup"><span data-stu-id="9b454-140">String</span></span>| <span data-ttu-id="9b454-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-141">Read-only.</span></span> <span data-ttu-id="9b454-142">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-142">ID of the plan.</span></span> <span data-ttu-id="9b454-143">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9b454-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9b454-144">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="9b454-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9b454-145">owner</span><span class="sxs-lookup"><span data-stu-id="9b454-145">owner</span></span>|<span data-ttu-id="9b454-146">String</span><span class="sxs-lookup"><span data-stu-id="9b454-146">String</span></span>|<span data-ttu-id="9b454-147">A ID do [Grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-147">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="9b454-148">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="9b454-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="9b454-149">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9b454-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="9b454-150">title</span><span class="sxs-lookup"><span data-stu-id="9b454-150">title</span></span>|<span data-ttu-id="9b454-151">String</span><span class="sxs-lookup"><span data-stu-id="9b454-151">String</span></span>|<span data-ttu-id="9b454-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b454-152">Required.</span></span> <span data-ttu-id="9b454-153">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-153">Title of the plan.</span></span>|
|<span data-ttu-id="9b454-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="9b454-154">createdBy</span></span>|[<span data-ttu-id="9b454-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="9b454-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="9b454-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-156">Read-only.</span></span> <span data-ttu-id="9b454-157">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-157">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b454-158">Relações</span><span class="sxs-lookup"><span data-stu-id="9b454-158">Relationships</span></span>
| <span data-ttu-id="9b454-159">Relação</span><span class="sxs-lookup"><span data-stu-id="9b454-159">Relationship</span></span> | <span data-ttu-id="9b454-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b454-160">Type</span></span>   |<span data-ttu-id="9b454-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b454-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b454-162">buckets</span><span class="sxs-lookup"><span data-stu-id="9b454-162">buckets</span></span>|<span data-ttu-id="9b454-163">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="9b454-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="9b454-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-164">Read-only.</span></span> <span data-ttu-id="9b454-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9b454-165">Nullable.</span></span> <span data-ttu-id="9b454-166">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-166">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="9b454-167">detalhes</span><span class="sxs-lookup"><span data-stu-id="9b454-167">details</span></span>|[<span data-ttu-id="9b454-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="9b454-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="9b454-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-169">Read-only.</span></span> <span data-ttu-id="9b454-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9b454-170">Nullable.</span></span> <span data-ttu-id="9b454-171">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="9b454-172">tarefas</span><span class="sxs-lookup"><span data-stu-id="9b454-172">tasks</span></span>|<span data-ttu-id="9b454-173">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9b454-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9b454-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9b454-174">Read-only.</span></span> <span data-ttu-id="9b454-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9b454-175">Nullable.</span></span> <span data-ttu-id="9b454-176">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="9b454-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b454-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b454-177">JSON representation</span></span>

<span data-ttu-id="9b454-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b454-178">Here is a JSON representation of the resource.</span></span>

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
