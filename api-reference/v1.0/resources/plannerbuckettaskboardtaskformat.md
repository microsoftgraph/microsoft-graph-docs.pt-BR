# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="c472e-101">Tipo de recurso plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c472e-101">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="c472e-p101">O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="c472e-p101">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="c472e-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="c472e-104">Methods</span></span>

| <span data-ttu-id="c472e-105">Método</span><span class="sxs-lookup"><span data-stu-id="c472e-105">Method</span></span>           | <span data-ttu-id="c472e-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c472e-106">Return Type</span></span>    |<span data-ttu-id="c472e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="c472e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c472e-108">Get plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c472e-108">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat_get.md) | [<span data-ttu-id="c472e-109">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c472e-109">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="c472e-110">Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="c472e-110">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="c472e-111">Update</span><span class="sxs-lookup"><span data-stu-id="c472e-111">Update</span></span>](../api/plannerbuckettaskboardtaskformat_update.md) | [<span data-ttu-id="c472e-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c472e-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="c472e-113">Atualize o objeto **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="c472e-113">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c472e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c472e-114">Properties</span></span>
| <span data-ttu-id="c472e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c472e-115">Property</span></span>     | <span data-ttu-id="c472e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="c472e-116">Type</span></span>   |<span data-ttu-id="c472e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c472e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c472e-118">id</span><span class="sxs-lookup"><span data-stu-id="c472e-118">id</span></span>|<span data-ttu-id="c472e-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c472e-119">String</span></span>| <span data-ttu-id="c472e-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c472e-120">Read-only.</span></span> <span data-ttu-id="c472e-121">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="c472e-121">The ID of the resource.</span></span> <span data-ttu-id="c472e-122">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="c472e-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c472e-123">[Validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="c472e-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c472e-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="c472e-124">orderHint</span></span>|<span data-ttu-id="c472e-125">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c472e-125">String</span></span>|<span data-ttu-id="c472e-p103">Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="c472e-p103">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c472e-128">Relações</span><span class="sxs-lookup"><span data-stu-id="c472e-128">Relationships</span></span>
<span data-ttu-id="c472e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c472e-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c472e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c472e-130">JSON representation</span></span>
<span data-ttu-id="c472e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c472e-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->