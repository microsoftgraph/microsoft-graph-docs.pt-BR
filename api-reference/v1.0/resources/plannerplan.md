---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Microsoft 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d8824ddde9cfa54bcf31cf7e2421d16fd749e3ca
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444347"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="2ddf5-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2ddf5-107">plannerPlan resource type</span></span>

<span data-ttu-id="2ddf5-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ddf5-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ddf5-109">O recurso **plannerPlan** representa um plano no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-109">The **plannerPlan** resource represents a plan in Microsoft 365.</span></span> <span data-ttu-id="2ddf5-110">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="2ddf5-110">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="2ddf5-111">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="2ddf5-111">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="2ddf5-112">Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-112">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="2ddf5-113">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="2ddf5-113">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2ddf5-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ddf5-114">Methods</span></span>

| <span data-ttu-id="2ddf5-115">Método</span><span class="sxs-lookup"><span data-stu-id="2ddf5-115">Method</span></span>           | <span data-ttu-id="2ddf5-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ddf5-116">Return Type</span></span>    |<span data-ttu-id="2ddf5-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ddf5-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ddf5-118">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2ddf5-118">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="2ddf5-119">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2ddf5-119">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="2ddf5-120">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-120">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="2ddf5-121">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="2ddf5-121">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="2ddf5-122">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2ddf5-122">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2ddf5-123">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-123">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="2ddf5-124">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="2ddf5-124">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="2ddf5-125">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2ddf5-125">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2ddf5-126">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-126">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="2ddf5-127">Atualizar</span><span class="sxs-lookup"><span data-stu-id="2ddf5-127">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="2ddf5-128">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="2ddf5-128">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="2ddf5-129">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-129">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2ddf5-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ddf5-130">Properties</span></span>
| <span data-ttu-id="2ddf5-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ddf5-131">Property</span></span>     | <span data-ttu-id="2ddf5-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ddf5-132">Type</span></span>   |<span data-ttu-id="2ddf5-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ddf5-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ddf5-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ddf5-134">createdDateTime</span></span>|<span data-ttu-id="2ddf5-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ddf5-135">DateTimeOffset</span></span>|<span data-ttu-id="2ddf5-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-136">Read-only.</span></span> <span data-ttu-id="2ddf5-137">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-137">Date and time at which the plan is created.</span></span> <span data-ttu-id="2ddf5-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ddf5-139">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2ddf5-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2ddf5-140">id</span><span class="sxs-lookup"><span data-stu-id="2ddf5-140">id</span></span>|<span data-ttu-id="2ddf5-141">String</span><span class="sxs-lookup"><span data-stu-id="2ddf5-141">String</span></span>| <span data-ttu-id="2ddf5-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-142">Read-only.</span></span> <span data-ttu-id="2ddf5-143">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-143">ID of the plan.</span></span> <span data-ttu-id="2ddf5-144">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-144">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="2ddf5-145">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-145">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="2ddf5-146">owner</span><span class="sxs-lookup"><span data-stu-id="2ddf5-146">owner</span></span>|<span data-ttu-id="2ddf5-147">String</span><span class="sxs-lookup"><span data-stu-id="2ddf5-147">String</span></span>|<span data-ttu-id="2ddf5-148">A ID do [Grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-148">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="2ddf5-149">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-149">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="2ddf5-150">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-150">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="2ddf5-151">title</span><span class="sxs-lookup"><span data-stu-id="2ddf5-151">title</span></span>|<span data-ttu-id="2ddf5-152">String</span><span class="sxs-lookup"><span data-stu-id="2ddf5-152">String</span></span>|<span data-ttu-id="2ddf5-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-153">Required.</span></span> <span data-ttu-id="2ddf5-154">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-154">Title of the plan.</span></span>|
|<span data-ttu-id="2ddf5-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="2ddf5-155">createdBy</span></span>|[<span data-ttu-id="2ddf5-156">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ddf5-156">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ddf5-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-157">Read-only.</span></span> <span data-ttu-id="2ddf5-158">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-158">The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ddf5-159">Relações</span><span class="sxs-lookup"><span data-stu-id="2ddf5-159">Relationships</span></span>
| <span data-ttu-id="2ddf5-160">Relação</span><span class="sxs-lookup"><span data-stu-id="2ddf5-160">Relationship</span></span> | <span data-ttu-id="2ddf5-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ddf5-161">Type</span></span>   |<span data-ttu-id="2ddf5-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ddf5-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ddf5-163">buckets</span><span class="sxs-lookup"><span data-stu-id="2ddf5-163">buckets</span></span>|<span data-ttu-id="2ddf5-164">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="2ddf5-164">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="2ddf5-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-165">Read-only.</span></span> <span data-ttu-id="2ddf5-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-166">Nullable.</span></span> <span data-ttu-id="2ddf5-167">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-167">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="2ddf5-168">detalhes</span><span class="sxs-lookup"><span data-stu-id="2ddf5-168">details</span></span>|[<span data-ttu-id="2ddf5-169">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="2ddf5-169">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="2ddf5-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-170">Read-only.</span></span> <span data-ttu-id="2ddf5-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-171">Nullable.</span></span> <span data-ttu-id="2ddf5-172">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-172">Additional details about the plan.</span></span>|
|<span data-ttu-id="2ddf5-173">tarefas</span><span class="sxs-lookup"><span data-stu-id="2ddf5-173">tasks</span></span>|<span data-ttu-id="2ddf5-174">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="2ddf5-174">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="2ddf5-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-175">Read-only.</span></span> <span data-ttu-id="2ddf5-176">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-176">Nullable.</span></span> <span data-ttu-id="2ddf5-177">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-177">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ddf5-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ddf5-178">JSON representation</span></span>

<span data-ttu-id="2ddf5-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ddf5-179">Here is a JSON representation of the resource.</span></span>

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

