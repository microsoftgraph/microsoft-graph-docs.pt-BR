# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="ba85e-101">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ba85e-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="ba85e-p101">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="ba85e-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="ba85e-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="ba85e-104">Methods</span></span>

| <span data-ttu-id="ba85e-105">Método</span><span class="sxs-lookup"><span data-stu-id="ba85e-105">Method</span></span>           | <span data-ttu-id="ba85e-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba85e-106">Return Type</span></span>    |<span data-ttu-id="ba85e-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba85e-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ba85e-108">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ba85e-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="ba85e-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ba85e-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="ba85e-110">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="ba85e-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="ba85e-111">Atualizar</span><span class="sxs-lookup"><span data-stu-id="ba85e-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="ba85e-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ba85e-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="ba85e-113">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="ba85e-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba85e-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba85e-114">Properties</span></span>
| <span data-ttu-id="ba85e-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba85e-115">Property</span></span>     | <span data-ttu-id="ba85e-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba85e-116">Type</span></span>   |<span data-ttu-id="ba85e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba85e-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba85e-118">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="ba85e-118">checklist</span></span>|[<span data-ttu-id="ba85e-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="ba85e-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="ba85e-120">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="ba85e-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="ba85e-121">description</span><span class="sxs-lookup"><span data-stu-id="ba85e-121">description</span></span>|<span data-ttu-id="ba85e-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba85e-122">String</span></span>|<span data-ttu-id="ba85e-123">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="ba85e-123">Description of the task</span></span>|
|<span data-ttu-id="ba85e-124">id</span><span class="sxs-lookup"><span data-stu-id="ba85e-124">id</span></span>|<span data-ttu-id="ba85e-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba85e-125">String</span></span>| <span data-ttu-id="ba85e-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba85e-126">Read-only.</span></span> <span data-ttu-id="ba85e-127">ID dos detalhes da tarefa.</span><span class="sxs-lookup"><span data-stu-id="ba85e-127">ID of the task details.</span></span> <span data-ttu-id="ba85e-128">Tem 28 caracteres e diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ba85e-128">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="ba85e-129">A [validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.</span><span class="sxs-lookup"><span data-stu-id="ba85e-129">[Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="ba85e-130">previewType</span><span class="sxs-lookup"><span data-stu-id="ba85e-130">previewType</span></span>|<span data-ttu-id="ba85e-131">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba85e-131">string</span></span>|<span data-ttu-id="ba85e-132">Isto define o tipo de visualização que aparecerá na tarefa.</span><span class="sxs-lookup"><span data-stu-id="ba85e-132">This sets the type of preview that shows up on the task. Possible values are: , , , , .</span></span> <span data-ttu-id="ba85e-133">Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span><span class="sxs-lookup"><span data-stu-id="ba85e-133">The possible values are `automatic`, `noPreview`, `checklist`, `description`, `reference`, , , , , , , or .</span></span> <span data-ttu-id="ba85e-134">Quando definido como `automatic` a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="ba85e-134">This sets the type of preview that shows up on the task. Possible values are: , , , , . When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="ba85e-135">referências</span><span class="sxs-lookup"><span data-stu-id="ba85e-135">references</span></span>|[<span data-ttu-id="ba85e-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="ba85e-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="ba85e-137">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="ba85e-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba85e-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ba85e-138">Relationships</span></span>
<span data-ttu-id="ba85e-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba85e-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ba85e-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba85e-140">JSON representation</span></span>
<span data-ttu-id="ba85e-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba85e-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
