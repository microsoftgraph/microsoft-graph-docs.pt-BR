# <a name="planneruser-resource-type"></a><span data-ttu-id="75908-101">Tipo de recurso plannerUser</span><span class="sxs-lookup"><span data-stu-id="75908-101">plannerUser resource type</span></span>

<span data-ttu-id="75908-p101">O recurso **plannerUser** oferece acesso aos recursos do Planner para um [usuário](user.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="75908-p101">The **plannerUser** resource provide access to Planner resources for a [user](user.md). It doesn't contain any usable properties.</span></span>


## <a name="methods"></a><span data-ttu-id="75908-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="75908-104">Methods</span></span>

| <span data-ttu-id="75908-105">Método</span><span class="sxs-lookup"><span data-stu-id="75908-105">Method</span></span>           | <span data-ttu-id="75908-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75908-106">Return Type</span></span>    |<span data-ttu-id="75908-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="75908-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75908-108">Listar planos</span><span class="sxs-lookup"><span data-stu-id="75908-108">List plans</span></span>](../api/planneruser_list_plans.md) |<span data-ttu-id="75908-109">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="75908-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="75908-110">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="75908-110">Get a **plannerPlan** object collection.</span></span>|
|[<span data-ttu-id="75908-111">Listar tarefas</span><span class="sxs-lookup"><span data-stu-id="75908-111">List tasks</span></span>](../api/planneruser_list_tasks.md) |<span data-ttu-id="75908-112">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="75908-112">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="75908-113">Obter uma coleção de objetos **plannerTask**.</span><span class="sxs-lookup"><span data-stu-id="75908-113">Get a **plannerTask** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="75908-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75908-114">Properties</span></span>
| <span data-ttu-id="75908-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75908-115">Property</span></span>     | <span data-ttu-id="75908-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="75908-116">Type</span></span>   |<span data-ttu-id="75908-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="75908-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75908-118">id</span><span class="sxs-lookup"><span data-stu-id="75908-118">id</span></span>|<span data-ttu-id="75908-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="75908-119">String</span></span>| <span data-ttu-id="75908-p102">Somente leitura. O identificador do plannerUser</span><span class="sxs-lookup"><span data-stu-id="75908-p102">Read-only. Identifier of the planenrUser</span></span>|

## <a name="relationships"></a><span data-ttu-id="75908-122">Relações</span><span class="sxs-lookup"><span data-stu-id="75908-122">Relationships</span></span>
| <span data-ttu-id="75908-123">Relação</span><span class="sxs-lookup"><span data-stu-id="75908-123">Relationship</span></span> | <span data-ttu-id="75908-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="75908-124">Type</span></span>   |<span data-ttu-id="75908-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="75908-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75908-126">plans</span><span class="sxs-lookup"><span data-stu-id="75908-126">plans</span></span>|<span data-ttu-id="75908-127">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="75908-127">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="75908-p103">Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.</span><span class="sxs-lookup"><span data-stu-id="75908-p103">Read-only. Nullable. Returns the [plannerTasks](plannertask.md) assigned to the user.</span></span>|
|<span data-ttu-id="75908-131">tarefas</span><span class="sxs-lookup"><span data-stu-id="75908-131">tasks</span></span>|<span data-ttu-id="75908-132">Coleção [plannerTask](plannertask.md)</span><span class="sxs-lookup"><span data-stu-id="75908-132">[plannerTask](plannertask.md) collection</span></span>| <span data-ttu-id="75908-p104">Somente leitura. Anulável. Returna o objeto [plannerTasks](plannerplan.md) atribuído ao usuário.</span><span class="sxs-lookup"><span data-stu-id="75908-p104">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) shared with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75908-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75908-136">JSON representation</span></span>
<span data-ttu-id="75908-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75908-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->