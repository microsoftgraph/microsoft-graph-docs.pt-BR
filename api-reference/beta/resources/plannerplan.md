---
title: Tipo de recurso plannerPlan
description: O recurso de **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um grupo e contém uma coleção de plannerTasks. Ele também pode ter uma coleção de plannerBuckets. Cada objeto de plano tem um objeto de detalhes que pode conter mais informações sobre o plano. Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte planejador.
ms.openlocfilehash: 236b6cb5d35e11a30bcb4371e0563b56ac93de8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035344"
---
# <a name="plannerplan-resource-type"></a><span data-ttu-id="6cda8-107">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6cda8-107">plannerPlan resource type</span></span>

> <span data-ttu-id="6cda8-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6cda8-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cda8-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6cda8-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cda8-110">O recurso de **plannerPlan** representa um plano no Office 365.</span><span class="sxs-lookup"><span data-stu-id="6cda8-110">The **plannerPlan** resource represents a plan in Office 365.</span></span> <span data-ttu-id="6cda8-111">Um plano pode pertencer a um [grupo](group.md) e contém uma coleção de [plannerTasks](plannertask.md).</span><span class="sxs-lookup"><span data-stu-id="6cda8-111">A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannertask.md).</span></span> <span data-ttu-id="6cda8-112">Ele também pode ter uma coleção de [plannerBuckets](plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="6cda8-112">It can also have a collection of [plannerBuckets](plannerbucket.md).</span></span> <span data-ttu-id="6cda8-113">Cada objeto de plano tem um objeto de [detalhes](plannerplandetails.md) que pode conter mais informações sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-113">Each plan object has a [details](plannerplandetails.md) object which can contain more information about the plan.</span></span> <span data-ttu-id="6cda8-114">Para obter mais informações sobre os relacionamentos entre grupos, planos e tarefas, consulte [Planejador](planner-overview.md).</span><span class="sxs-lookup"><span data-stu-id="6cda8-114">For more information about the relationships between groups, plans, and tasks, see [Planner](planner-overview.md).</span></span>



## <a name="methods"></a><span data-ttu-id="6cda8-115">Métodos</span><span class="sxs-lookup"><span data-stu-id="6cda8-115">Methods</span></span>

| <span data-ttu-id="6cda8-116">Método</span><span class="sxs-lookup"><span data-stu-id="6cda8-116">Method</span></span>           | <span data-ttu-id="6cda8-117">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6cda8-117">Return Type</span></span>    |<span data-ttu-id="6cda8-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cda8-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cda8-119">Get plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6cda8-119">Get plannerPlan</span></span>](../api/plannerplan-get.md) | [<span data-ttu-id="6cda8-120">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6cda8-120">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="6cda8-121">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="6cda8-121">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="6cda8-122">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="6cda8-122">List buckets</span></span>](../api/plannerplan-list-buckets.md) |<span data-ttu-id="6cda8-123">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="6cda8-123">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6cda8-124">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="6cda8-124">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="6cda8-125">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="6cda8-125">List tasks</span></span>](../api/plannerplan-list-tasks.md) |<span data-ttu-id="6cda8-126">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="6cda8-126">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6cda8-127">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="6cda8-127">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="6cda8-128">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6cda8-128">Update</span></span>](../api/plannerplan-update.md) | [<span data-ttu-id="6cda8-129">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="6cda8-129">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="6cda8-130">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="6cda8-130">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6cda8-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cda8-131">Properties</span></span>
| <span data-ttu-id="6cda8-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cda8-132">Property</span></span>     | <span data-ttu-id="6cda8-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cda8-133">Type</span></span>   |<span data-ttu-id="6cda8-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cda8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cda8-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cda8-135">createdDateTime</span></span>|<span data-ttu-id="6cda8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cda8-136">DateTimeOffset</span></span>|<span data-ttu-id="6cda8-p104">Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6cda8-p104">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6cda8-141">id</span><span class="sxs-lookup"><span data-stu-id="6cda8-141">id</span></span>|<span data-ttu-id="6cda8-142">String</span><span class="sxs-lookup"><span data-stu-id="6cda8-142">String</span></span>| <span data-ttu-id="6cda8-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6cda8-143">Read-only.</span></span> <span data-ttu-id="6cda8-144">ID do plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-144">ID of the plan.</span></span> <span data-ttu-id="6cda8-145">É 28 caracteres longos e diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6cda8-145">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6cda8-146">[Validação de formato](tasks-identifiers-disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="6cda8-146">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6cda8-147">owner</span><span class="sxs-lookup"><span data-stu-id="6cda8-147">owner</span></span>|<span data-ttu-id="6cda8-148">String</span><span class="sxs-lookup"><span data-stu-id="6cda8-148">String</span></span>|<span data-ttu-id="6cda8-149">ID do [grupo](group.md) que possui o plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-149">ID of the [Group](group.md) that owns the plan.</span></span> <span data-ttu-id="6cda8-150">Um grupo válido deve existir antes que esse campo pode ser definido.</span><span class="sxs-lookup"><span data-stu-id="6cda8-150">A valid group must exist before this field can be set.</span></span> <span data-ttu-id="6cda8-151">Depois que ele for definido, essa propriedade não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="6cda8-151">After it is set, this property can’t be updated.</span></span>|
|<span data-ttu-id="6cda8-152">title</span><span class="sxs-lookup"><span data-stu-id="6cda8-152">title</span></span>|<span data-ttu-id="6cda8-153">String</span><span class="sxs-lookup"><span data-stu-id="6cda8-153">String</span></span>|<span data-ttu-id="6cda8-p107">Obrigatório. Título do plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-p107">Required. Title of the plan.</span></span>|
|<span data-ttu-id="6cda8-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="6cda8-156">createdBy</span></span>|[<span data-ttu-id="6cda8-157">identitySet</span><span class="sxs-lookup"><span data-stu-id="6cda8-157">identitySet</span></span>](identityset.md)|<span data-ttu-id="6cda8-p108">Somente leitura. O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-p108">Read-only. The user who created the plan.</span></span>|
|<span data-ttu-id="6cda8-160">contextos</span><span class="sxs-lookup"><span data-stu-id="6cda8-160">contexts</span></span>|[<span data-ttu-id="6cda8-161">plannerPlanContextCollection</span><span class="sxs-lookup"><span data-stu-id="6cda8-161">plannerPlanContextCollection</span></span>](plannerplancontextcollection.md)| <span data-ttu-id="6cda8-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6cda8-162">Read-only.</span></span> <span data-ttu-id="6cda8-163">Experiências de usuário adicional no qual este plano for usado, representado como entradas de [plannerPlanContext](plannerplancontext.md) .</span><span class="sxs-lookup"><span data-stu-id="6cda8-163">Additional user experiences in which this plan is used, represented as [plannerPlanContext](plannerplancontext.md) entries.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cda8-164">Relações</span><span class="sxs-lookup"><span data-stu-id="6cda8-164">Relationships</span></span>
| <span data-ttu-id="6cda8-165">Relação</span><span class="sxs-lookup"><span data-stu-id="6cda8-165">Relationship</span></span> | <span data-ttu-id="6cda8-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cda8-166">Type</span></span>   |<span data-ttu-id="6cda8-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cda8-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cda8-168">buckets</span><span class="sxs-lookup"><span data-stu-id="6cda8-168">buckets</span></span>|<span data-ttu-id="6cda8-169">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="6cda8-169">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="6cda8-p110">Somente leitura. Anulável. A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-p110">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="6cda8-173">detalhes</span><span class="sxs-lookup"><span data-stu-id="6cda8-173">details</span></span>|[<span data-ttu-id="6cda8-174">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="6cda8-174">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="6cda8-p111">Somente leitura. Anulável. Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-p111">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="6cda8-178">tarefas</span><span class="sxs-lookup"><span data-stu-id="6cda8-178">tasks</span></span>|<span data-ttu-id="6cda8-179">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="6cda8-179">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="6cda8-p112">Somente leitura. Anulável. A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="6cda8-p112">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cda8-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cda8-183">JSON representation</span></span>

<span data-ttu-id="6cda8-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6cda8-184">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->