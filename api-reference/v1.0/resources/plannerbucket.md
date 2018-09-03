# <a name="plannerbucket-resource-type"></a><span data-ttu-id="81076-101">Tipo de recurso plannerBucket</span><span class="sxs-lookup"><span data-stu-id="81076-101">plannerBucket resource type</span></span>

<span data-ttu-id="81076-p101">O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerPlan.md) e pode ter uma coleção de [plannerTasks](plannerTask.md).</span><span class="sxs-lookup"><span data-stu-id="81076-p101">The **plannerBucket** resource represents a bucket (or "custom column") for tasks in a plan in Office 365. It is contained in a [plannerPlan](plannerPlan.md) and can have a collection of [plannerTasks](plannerTask.md).</span></span>



## <a name="methods"></a><span data-ttu-id="81076-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="81076-104">Methods</span></span>

| <span data-ttu-id="81076-105">Método</span><span class="sxs-lookup"><span data-stu-id="81076-105">Method</span></span>           | <span data-ttu-id="81076-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81076-106">Return Type</span></span>    |<span data-ttu-id="81076-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="81076-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81076-108">Get plannerBucket</span><span class="sxs-lookup"><span data-stu-id="81076-108">Get plannerBucket</span></span>](../api/plannerbucket_get.md) | [<span data-ttu-id="81076-109">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="81076-109">plannerBucket</span></span>](plannerbucket.md) |<span data-ttu-id="81076-110">Leia as propriedades e as relações do objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="81076-110">Read properties and relationships of **plannerBucket** object.</span></span>|
|[<span data-ttu-id="81076-111">Listar plannerTasks</span><span class="sxs-lookup"><span data-stu-id="81076-111">List plannerTasks</span></span>](../api/plannerbucket_list_tasks.md) |<span data-ttu-id="81076-112">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="81076-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="81076-113">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="81076-113">Get a **plannerTask** object collection.</span></span>|
|[<span data-ttu-id="81076-114">Criar</span><span class="sxs-lookup"><span data-stu-id="81076-114">Create</span></span>](../api/planner_post_buckets.md) | [<span data-ttu-id="81076-115">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="81076-115">plannerBucket</span></span>](plannerbucket.md)   | <span data-ttu-id="81076-116">Crie um novo objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="81076-116">Create a new **plannerBucket** object.</span></span> |
|[<span data-ttu-id="81076-117">Atualizar</span><span class="sxs-lookup"><span data-stu-id="81076-117">Update</span></span>](../api/plannerbucket_update.md) | [<span data-ttu-id="81076-118">plannerBucket</span><span class="sxs-lookup"><span data-stu-id="81076-118">plannerBucket</span></span>](plannerbucket.md)   |<span data-ttu-id="81076-119">Atualize o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="81076-119">Update **plannerBucket** object.</span></span> |
|[<span data-ttu-id="81076-120">Excluir</span><span class="sxs-lookup"><span data-stu-id="81076-120">Delete</span></span>](../api/plannerbucket_delete.md) | <span data-ttu-id="81076-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81076-121">None</span></span> |<span data-ttu-id="81076-122">Exclua o objeto **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="81076-122">Delete **plannerBucket** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="81076-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81076-123">Properties</span></span>
| <span data-ttu-id="81076-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81076-124">Property</span></span>     | <span data-ttu-id="81076-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="81076-125">Type</span></span>   |<span data-ttu-id="81076-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="81076-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81076-127">id</span><span class="sxs-lookup"><span data-stu-id="81076-127">id</span></span>|<span data-ttu-id="81076-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="81076-128">String</span></span>| <span data-ttu-id="81076-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81076-129">Read-only.</span></span> <span data-ttu-id="81076-130">ID do bucket.</span><span class="sxs-lookup"><span data-stu-id="81076-130">Name of the bucket.</span></span> <span data-ttu-id="81076-131">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="81076-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="81076-132">A [validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="81076-132">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="81076-133">name</span><span class="sxs-lookup"><span data-stu-id="81076-133">name</span></span>|<span data-ttu-id="81076-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="81076-134">String</span></span>|<span data-ttu-id="81076-135">Nome do bucket.</span><span class="sxs-lookup"><span data-stu-id="81076-135">Name of the bucket.</span></span>|
|<span data-ttu-id="81076-136">orderHint</span><span class="sxs-lookup"><span data-stu-id="81076-136">orderHint</span></span>|<span data-ttu-id="81076-137">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="81076-137">String</span></span>|<span data-ttu-id="81076-p103">Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="81076-p103">Hint used to order items of this type in a list view. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="81076-140">planId</span><span class="sxs-lookup"><span data-stu-id="81076-140">planId</span></span>|<span data-ttu-id="81076-141">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="81076-141">String</span></span>|<span data-ttu-id="81076-142">ID do plano ao qual o bucket pertence.</span><span class="sxs-lookup"><span data-stu-id="81076-142">Plan ID to which the bucket belongs.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81076-143">Relações</span><span class="sxs-lookup"><span data-stu-id="81076-143">Relationships</span></span>
| <span data-ttu-id="81076-144">Relação</span><span class="sxs-lookup"><span data-stu-id="81076-144">Relationship</span></span> | <span data-ttu-id="81076-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="81076-145">Type</span></span>   |<span data-ttu-id="81076-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="81076-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81076-147">tarefas</span><span class="sxs-lookup"><span data-stu-id="81076-147">tasks</span></span>|<span data-ttu-id="81076-148">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="81076-148">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="81076-p104">Somente leitura. Anulável. A coleção de tarefas no bucket.</span><span class="sxs-lookup"><span data-stu-id="81076-p104">Read-only. Nullable. The collection of tasks in the bucket.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81076-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81076-152">JSON representation</span></span>
<span data-ttu-id="81076-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81076-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->