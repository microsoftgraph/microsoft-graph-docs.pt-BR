# <a name="plannerplan-resource-type"></a><span data-ttu-id="c5394-101">Tipo de recurso plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c5394-101">plannerPlan resource type</span></span>

<span data-ttu-id="c5394-p101">O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannerTask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerBucket.md). Cada objeto de plano tem um objeto [details](plannerPlanDetails.md) que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner_overview.md).</span><span class="sxs-lookup"><span data-stu-id="c5394-p101">The **plannerPlan** resource represents a plan in Office 365. A plan can be owned by a [group](group.md) and contains a collection of [plannerTasks](plannerTask.md). It can also have a collection of [plannerBuckets](plannerBucket.md). Each plan object has a [details](plannerPlanDetails.md) object that can contain more information about the plan. For more information about the relationships between groups, plans, and tasks, see [Planner](planner_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c5394-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5394-107">Methods</span></span>

| <span data-ttu-id="c5394-108">Método</span><span class="sxs-lookup"><span data-stu-id="c5394-108">Method</span></span>           | <span data-ttu-id="c5394-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5394-109">Return Type</span></span>    |<span data-ttu-id="c5394-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5394-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5394-111">Obter plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c5394-111">Get plannerPlan</span></span>](../api/plannerplan_get.md) | [<span data-ttu-id="c5394-112">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c5394-112">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c5394-113">Leia as propriedades e as relações do objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="c5394-113">Read properties and relationships of **plannerPlan** object.</span></span>|
|[<span data-ttu-id="c5394-114">Listar buckets</span><span class="sxs-lookup"><span data-stu-id="c5394-114">List buckets</span></span>](../api/plannerplan_list_buckets.md) |<span data-ttu-id="c5394-115">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="c5394-115">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c5394-116">Obter uma coleção de objetos **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="c5394-116">Get a **plannerBucket** object collection.</span></span>|
|[<span data-ttu-id="c5394-117">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="c5394-117">List tasks</span></span>](../api/plannerplan_list_tasks.md) |<span data-ttu-id="c5394-118">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c5394-118">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c5394-119">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="c5394-119">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="c5394-120">Atualizar</span><span class="sxs-lookup"><span data-stu-id="c5394-120">Update</span></span>](../api/plannerplan_update.md) | [<span data-ttu-id="c5394-121">plannerPlan</span><span class="sxs-lookup"><span data-stu-id="c5394-121">plannerPlan</span></span>](plannerplan.md) |<span data-ttu-id="c5394-122">Atualize o objeto **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="c5394-122">Update **plannerPlan** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5394-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5394-123">Properties</span></span>
| <span data-ttu-id="c5394-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5394-124">Property</span></span>     | <span data-ttu-id="c5394-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5394-125">Type</span></span>   |<span data-ttu-id="c5394-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5394-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5394-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5394-127">createdDateTime</span></span>|<span data-ttu-id="c5394-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5394-128">DateTimeOffset</span></span>|<span data-ttu-id="c5394-p102">Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c5394-p102">Read-only. Date and time at which the plan is created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c5394-133">id</span><span class="sxs-lookup"><span data-stu-id="c5394-133">id</span></span>|<span data-ttu-id="c5394-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5394-134">String</span></span>| <span data-ttu-id="c5394-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5394-135">Read-only.</span></span> <span data-ttu-id="c5394-136">ID do plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-136">Title of the plan.</span></span> <span data-ttu-id="c5394-137">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c5394-137">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c5394-138">A[validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="c5394-138">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c5394-139">proprietário</span><span class="sxs-lookup"><span data-stu-id="c5394-139">owner</span></span>|<span data-ttu-id="c5394-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5394-140">String</span></span>|<span data-ttu-id="c5394-p104">A ID do [Grupo](group.md) que possui o plano. Deve haver um grupo válido para que esse campo possa ser definido. Após definido, ele só poderá ser atualizado pelo proprietário.</span><span class="sxs-lookup"><span data-stu-id="c5394-p104">ID of the [Group](group.md) that owns the plan. A valid group must exist before this field can be set. Once set, this can only be updated by the owner.</span></span>|
|<span data-ttu-id="c5394-144">título</span><span class="sxs-lookup"><span data-stu-id="c5394-144">title</span></span>|<span data-ttu-id="c5394-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5394-145">String</span></span>|<span data-ttu-id="c5394-p105">Obrigatório. Título do plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-p105">Required. Title of the plan.</span></span>|
|<span data-ttu-id="c5394-148">createdBy</span><span class="sxs-lookup"><span data-stu-id="c5394-148">createdBy</span></span>|[<span data-ttu-id="c5394-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="c5394-149">identitySet</span></span>](identityset.md)|<span data-ttu-id="c5394-p106">Somente leitura. O usuário que criou o plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-p106">Read-only. The user who created the plan.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5394-152">Relações</span><span class="sxs-lookup"><span data-stu-id="c5394-152">Relationships</span></span>
| <span data-ttu-id="c5394-153">Relação</span><span class="sxs-lookup"><span data-stu-id="c5394-153">Relationship</span></span> | <span data-ttu-id="c5394-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5394-154">Type</span></span>   |<span data-ttu-id="c5394-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5394-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5394-156">buckets</span><span class="sxs-lookup"><span data-stu-id="c5394-156">buckets</span></span>|<span data-ttu-id="c5394-157">Coleção [plannerBucket](plannerbucket.md)</span><span class="sxs-lookup"><span data-stu-id="c5394-157">[plannerBucket](plannerbucket.md) collection</span></span>| <span data-ttu-id="c5394-p107">Somente leitura. Anulável. A coleção de buckets no plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-p107">Read-only. Nullable. Collection of buckets in the plan.</span></span>|
|<span data-ttu-id="c5394-161">detalhes</span><span class="sxs-lookup"><span data-stu-id="c5394-161">details</span></span>|[<span data-ttu-id="c5394-162">plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="c5394-162">plannerPlanDetails</span></span>](plannerplandetails.md)| <span data-ttu-id="c5394-p108">Somente leitura. Anulável. Outros detalhes sobre o plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-p108">Read-only. Nullable. Additional details about the plan.</span></span>|
|<span data-ttu-id="c5394-166">tarefas</span><span class="sxs-lookup"><span data-stu-id="c5394-166">tasks</span></span>|<span data-ttu-id="c5394-167">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="c5394-167">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="c5394-p109">Somente leitura. Anulável. A coleção de tarefas no plano.</span><span class="sxs-lookup"><span data-stu-id="c5394-p109">Read-only. Nullable. Collection of tasks in the plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5394-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5394-171">JSON representation</span></span>

<span data-ttu-id="c5394-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5394-172">Here is a JSON representation of the resource.</span></span>

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