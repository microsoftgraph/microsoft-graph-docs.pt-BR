# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="581c6-101">Tipo de recurso plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="581c6-101">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="581c6-p101">O recurso **plannerProgressTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Progress do Quadro de Tarefas (uma exibição organizada pelo estado do campo PercentComplete no objeto da tarefa, com colunas para Não Iniciado, Em Andamento e Concluído). Cada [tarefa](plannertask.md) terá um objeto **plannerProgressTaskBoardTaskFormat** associado a ela.</span><span class="sxs-lookup"><span data-stu-id="581c6-p101">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="581c6-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="581c6-104">Methods</span></span>

| <span data-ttu-id="581c6-105">Método</span><span class="sxs-lookup"><span data-stu-id="581c6-105">Method</span></span>           | <span data-ttu-id="581c6-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="581c6-106">Return Type</span></span>    |<span data-ttu-id="581c6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="581c6-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="581c6-108">Obter plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="581c6-108">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat_get.md) | [<span data-ttu-id="581c6-109">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="581c6-109">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="581c6-110">Leia as propriedades e as relações do objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="581c6-110">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="581c6-111">Atualizar</span><span class="sxs-lookup"><span data-stu-id="581c6-111">Update</span></span>](../api/plannerprogresstaskboardtaskformat_update.md) | [<span data-ttu-id="581c6-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="581c6-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="581c6-113">Atualize o objeto **plannerProgressTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="581c6-113">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="581c6-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="581c6-114">Properties</span></span>
| <span data-ttu-id="581c6-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="581c6-115">Property</span></span>     | <span data-ttu-id="581c6-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="581c6-116">Type</span></span>   |<span data-ttu-id="581c6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="581c6-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="581c6-118">id</span><span class="sxs-lookup"><span data-stu-id="581c6-118">id</span></span>|<span data-ttu-id="581c6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="581c6-119">String</span></span>| <span data-ttu-id="581c6-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="581c6-120">Read-only.</span></span> <span data-ttu-id="581c6-121">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="581c6-121">The ID of the resource.</span></span> <span data-ttu-id="581c6-122">Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="581c6-122">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="581c6-123">[Validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="581c6-123">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="581c6-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="581c6-124">orderHint</span></span>|<span data-ttu-id="581c6-125">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="581c6-125">String</span></span>|<span data-ttu-id="581c6-p103">Valor da dica usado para ordenar a tarefa no modo de exibição Progress do Quadro de Tarefas. O formato é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="581c6-p103">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="581c6-128">Relações</span><span class="sxs-lookup"><span data-stu-id="581c6-128">Relationships</span></span>
<span data-ttu-id="581c6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="581c6-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="581c6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="581c6-130">JSON representation</span></span>
<span data-ttu-id="581c6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="581c6-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
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
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->