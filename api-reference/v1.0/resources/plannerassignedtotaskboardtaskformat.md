# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="b95e6-101">Tipo de recurso plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b95e6-101">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="b95e6-p101">O recurso **plannerAssignedToTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição AssignedTo do Quadro de Tarefas (um modo de exibição organizado por usuários aos quais as tarefas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerAssignedToTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="b95e6-p101">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="b95e6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="b95e6-104">Methods</span></span>

| <span data-ttu-id="b95e6-105">Método</span><span class="sxs-lookup"><span data-stu-id="b95e6-105">Method</span></span>           | <span data-ttu-id="b95e6-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b95e6-106">Return Type</span></span>    |<span data-ttu-id="b95e6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95e6-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b95e6-108">Get plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b95e6-108">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat_get.md) | [<span data-ttu-id="b95e6-109">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b95e6-109">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="b95e6-110">Leia as propriedades e relações do objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="b95e6-110">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="b95e6-111">Atualizar</span><span class="sxs-lookup"><span data-stu-id="b95e6-111">Update</span></span>](../api/plannerassignedtotaskboardtaskformat_update.md) | [<span data-ttu-id="b95e6-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b95e6-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="b95e6-113">Atualize o objeto **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="b95e6-113">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b95e6-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b95e6-114">Properties</span></span>
| <span data-ttu-id="b95e6-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b95e6-115">Property</span></span>     | <span data-ttu-id="b95e6-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95e6-116">Type</span></span>   |<span data-ttu-id="b95e6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95e6-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b95e6-118">id</span><span class="sxs-lookup"><span data-stu-id="b95e6-118">id</span></span>|<span data-ttu-id="b95e6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95e6-119">String</span></span>| <span data-ttu-id="b95e6-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b95e6-120">Read-only.</span></span> <span data-ttu-id="b95e6-121">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="b95e6-121">The ID of the resource.</span></span> <span data-ttu-id="b95e6-122">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="b95e6-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="b95e6-123">A [validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="b95e6-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="b95e6-124">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="b95e6-124">orderHintsByAssignee</span></span>|[<span data-ttu-id="b95e6-125">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="b95e6-125">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="b95e6-p103">O dicionário de dicas usado para ordenar tarefas no modo de exibição AssignedTo do Quadro de Tarefas. A chave de cada entrada é um dos usuários ao qual a tarefa é atribuída, e o valor é a dica de ordem. O formato de cada valor é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="b95e6-p103">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner_order_hint_format.md).</span></span>|
|<span data-ttu-id="b95e6-129">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="b95e6-129">unassignedOrderHint</span></span>|<span data-ttu-id="b95e6-130">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b95e6-130">String</span></span>|<span data-ttu-id="b95e6-p104">Valor da dica usado para ordenar a tarefa no modo de exibição AssignedTo do Quadro de Tarefas quando a tarefa não for atribuída a ninguém ou se o dicionário orderHintsByAssignee não oferecer uma dica de ordem para o usuário à qual a tarefa foi atribuída. O formato é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="b95e6-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b95e6-133">Relações</span><span class="sxs-lookup"><span data-stu-id="b95e6-133">Relationships</span></span>
<span data-ttu-id="b95e6-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b95e6-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b95e6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b95e6-135">JSON representation</span></span>
<span data-ttu-id="b95e6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b95e6-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->