# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="6959d-101">Tipo de recurso plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6959d-101">plannerTaskDetails resource type</span></span>

<span data-ttu-id="6959d-p101">O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.</span><span class="sxs-lookup"><span data-stu-id="6959d-p101">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="6959d-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="6959d-104">Methods</span></span>

| <span data-ttu-id="6959d-105">Método</span><span class="sxs-lookup"><span data-stu-id="6959d-105">Method</span></span>           | <span data-ttu-id="6959d-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6959d-106">Return Type</span></span>    |<span data-ttu-id="6959d-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="6959d-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6959d-108">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6959d-108">Get plannerTaskDetails</span></span>](../api/plannertaskdetails_get.md) | [<span data-ttu-id="6959d-109">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6959d-109">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="6959d-110">Leia as propriedades e as relações do objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6959d-110">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="6959d-111">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6959d-111">Update</span></span>](../api/plannertaskdetails_update.md) | [<span data-ttu-id="6959d-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6959d-112">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="6959d-113">Atualize o objeto **plannerTaskDetails**.</span><span class="sxs-lookup"><span data-stu-id="6959d-113">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6959d-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6959d-114">Properties</span></span>
| <span data-ttu-id="6959d-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6959d-115">Property</span></span>     | <span data-ttu-id="6959d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="6959d-116">Type</span></span>   |<span data-ttu-id="6959d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6959d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6959d-118">lista de verificação</span><span class="sxs-lookup"><span data-stu-id="6959d-118">checklist</span></span>|[<span data-ttu-id="6959d-119">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="6959d-119">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="6959d-120">A coleção de itens da lista de verificação na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6959d-120">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="6959d-121">description</span><span class="sxs-lookup"><span data-stu-id="6959d-121">description</span></span>|<span data-ttu-id="6959d-122">String</span><span class="sxs-lookup"><span data-stu-id="6959d-122">String</span></span>|<span data-ttu-id="6959d-123">Descrição da tarefa</span><span class="sxs-lookup"><span data-stu-id="6959d-123">Description of the task</span></span>|
|<span data-ttu-id="6959d-124">id</span><span class="sxs-lookup"><span data-stu-id="6959d-124">id</span></span>|<span data-ttu-id="6959d-125">String</span><span class="sxs-lookup"><span data-stu-id="6959d-125">String</span></span>| <span data-ttu-id="6959d-p102">Somente leitura. ID dos detalhes da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.</span><span class="sxs-lookup"><span data-stu-id="6959d-p102">Read-only. ID of the task details. It is 28 characters long and case sensitive. [Format validation](planner_identifiers_disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6959d-130">previewType</span><span class="sxs-lookup"><span data-stu-id="6959d-130">previewType</span></span>|<span data-ttu-id="6959d-131">string</span><span class="sxs-lookup"><span data-stu-id="6959d-131">string</span></span>|<span data-ttu-id="6959d-p103">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="6959d-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="6959d-135">referências</span><span class="sxs-lookup"><span data-stu-id="6959d-135">references</span></span>|[<span data-ttu-id="6959d-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="6959d-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="6959d-137">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="6959d-137">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6959d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="6959d-138">Relationships</span></span>
<span data-ttu-id="6959d-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6959d-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6959d-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6959d-140">JSON representation</span></span>
<span data-ttu-id="6959d-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6959d-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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