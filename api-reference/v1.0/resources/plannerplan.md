---
title: Tipo de recurso plannerPlan
description: O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e conter um conjunto de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o Planner.
localization_priority: Priority
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 9e77f2c0163f9093d931c46098498caa8c43f42c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462288"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="9a68c-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9a68c-107">plannerPlan resource type</span></span>

<span data-ttu-id="9a68c-108">O recurso **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="9a68c-108">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="9a68c-109">Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de plannerTasks.</span><span class="sxs-lookup"><span data-stu-id="9a68c-109">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="9a68c-110">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="9a68c-110">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="9a68c-111">Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-111">Each plan object has a [details](plannerplandetails.md) object that can contain more information about the plan.</span></span> <span data-ttu-id="9a68c-112">Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="9a68c-112">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9a68c-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a68c-113">Methods</span></span>

| <span data-ttu-id="9a68c-114">Método</span><span class="sxs-lookup"><span data-stu-id="9a68c-114">Method</span></span>           | <span data-ttu-id="9a68c-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a68c-115">Return Type</span></span>    |<span data-ttu-id="9a68c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a68c-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a68c-117">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9a68c-117">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="9a68c-118">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9a68c-118">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="9a68c-119">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="9a68c-119">Read properties and relationships of user object.</span></span>|
|[<span data-ttu-id="9a68c-120">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="9a68c-120">List plan buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="9a68c-121">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="9a68c-121">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="9a68c-122">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="9a68c-122">Get a CalendarGroup object collection.</span></span>|
|[<span data-ttu-id="9a68c-123">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="9a68c-123">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="9a68c-124">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9a68c-124">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9a68c-125">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="9a68c-125">Get a Calendar object collection.</span></span>|
|[<span data-ttu-id="9a68c-126">Atualizar</span><span class="sxs-lookup"><span data-stu-id="9a68c-126">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="9a68c-127">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="9a68c-127">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="9a68c-128">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="9a68c-128">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a68c-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a68c-129">Properties</span></span>
| <span data-ttu-id="9a68c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a68c-130">Property</span></span>     | <span data-ttu-id="9a68c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a68c-131">Type</span></span>   |<span data-ttu-id="9a68c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a68c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a68c-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a68c-133">createdDateTime</span></span>|<span data-ttu-id="9a68c-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a68c-134">DateTimeOffset</span></span>|<span data-ttu-id="9a68c-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-135">Read-only.</span></span> <span data-ttu-id="9a68c-136">A data e a hora que o plano foi criado.</span><span class="sxs-lookup"><span data-stu-id="9a68c-136">Date and time at which the plan is created.</span></span> <span data-ttu-id="9a68c-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9a68c-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a68c-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9a68c-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9a68c-139">id</span><span class="sxs-lookup"><span data-stu-id="9a68c-139">id</span></span>|<span data-ttu-id="9a68c-140">String</span><span class="sxs-lookup"><span data-stu-id="9a68c-140">String</span></span>| <span data-ttu-id="9a68c-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-141">Read-only.</span></span> <span data-ttu-id="9a68c-142">A ID do plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-142">ID of the translator.</span></span> <span data-ttu-id="9a68c-143">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9a68c-143">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="9a68c-144">[Formatar validação](planner-identifiers-disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="9a68c-144">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="9a68c-145">owner</span><span class="sxs-lookup"><span data-stu-id="9a68c-145">owner</span></span>|<span data-ttu-id="9a68c-146">String</span><span class="sxs-lookup"><span data-stu-id="9a68c-146">String</span></span>|<span data-ttu-id="9a68c-147">A ID do [Grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-147">ID of the principal that owns the lock.</span></span> <span data-ttu-id="9a68c-148">Deve haver um grupo válido para que esse campo possa ser definido.</span><span class="sxs-lookup"><span data-stu-id="9a68c-148">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="9a68c-149">Depois de definida, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9a68c-149">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="9a68c-150">title</span><span class="sxs-lookup"><span data-stu-id="9a68c-150">title</span></span>|<span data-ttu-id="9a68c-151">String</span><span class="sxs-lookup"><span data-stu-id="9a68c-151">String</span></span>|<span data-ttu-id="9a68c-152">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a68c-152">Required.</span></span> <span data-ttu-id="9a68c-153">Título do plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-153">Title of the add-in.</span></span>|
|<span data-ttu-id="9a68c-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="9a68c-154">createdBy</span></span>|[<span data-ttu-id="9a68c-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a68c-155">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a68c-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-156">Read-only.</span></span> <span data-ttu-id="9a68c-157">O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-157">The user who created the Timesheet is listed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a68c-158">Relações</span><span class="sxs-lookup"><span data-stu-id="9a68c-158">Relationships</span></span>
| <span data-ttu-id="9a68c-159">Relação</span><span class="sxs-lookup"><span data-stu-id="9a68c-159">Relationship</span></span> | <span data-ttu-id="9a68c-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a68c-160">Type</span></span>   |<span data-ttu-id="9a68c-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a68c-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a68c-162">buckets</span><span class="sxs-lookup"><span data-stu-id="9a68c-162">Buckets</span></span>|<span data-ttu-id="9a68c-163">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="9a68c-163">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="9a68c-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-164">Read-only.</span></span> <span data-ttu-id="9a68c-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9a68c-165">Nullable.</span></span> <span data-ttu-id="9a68c-166">A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-166">Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="9a68c-167">detalhes</span><span class="sxs-lookup"><span data-stu-id="9a68c-167">details</span></span>|[<span data-ttu-id="9a68c-168">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="9a68c-168">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="9a68c-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-169">Read-only.</span></span> <span data-ttu-id="9a68c-170">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9a68c-170">Nullable.</span></span> <span data-ttu-id="9a68c-171">Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-171">Additional details about the plan.</span></span>|
|<span data-ttu-id="9a68c-172">tarefas</span><span class="sxs-lookup"><span data-stu-id="9a68c-172">Tasks</span></span>|<span data-ttu-id="9a68c-173">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="9a68c-173">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="9a68c-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a68c-174">Read-only.</span></span> <span data-ttu-id="9a68c-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9a68c-175">Nullable.</span></span> <span data-ttu-id="9a68c-176">A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="9a68c-176">Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a68c-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a68c-177">JSON representation</span></span>

<span data-ttu-id="9a68c-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a68c-178">Here is a JSON representation of the resource.</span></span>

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
