# <a name="plannergroup-resource-type"></a><span data-ttu-id="e80fc-101">Tipo de recurso plannerGroup</span><span class="sxs-lookup"><span data-stu-id="e80fc-101">plannerGroup resource type</span></span>

<span data-ttu-id="e80fc-p101">O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.</span><span class="sxs-lookup"><span data-stu-id="e80fc-p101">The **plannerGroup** resource provides access to Planner resources for a [group](group.md). It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e80fc-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="e80fc-104">Methods</span></span>

| <span data-ttu-id="e80fc-105">Método</span><span class="sxs-lookup"><span data-stu-id="e80fc-105">Method</span></span>           | <span data-ttu-id="e80fc-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e80fc-106">Return Type</span></span>    |<span data-ttu-id="e80fc-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80fc-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e80fc-108">Listar planos</span><span class="sxs-lookup"><span data-stu-id="e80fc-108">List plans</span></span>](../api/plannergroup_list_plans.md) |<span data-ttu-id="e80fc-109">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="e80fc-109">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="e80fc-110">Obtenha uma coleção de objetos **plannerPlan**.</span><span class="sxs-lookup"><span data-stu-id="e80fc-110">Get a **plannerPlan** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e80fc-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e80fc-111">Properties</span></span>
| <span data-ttu-id="e80fc-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e80fc-112">Property</span></span>     | <span data-ttu-id="e80fc-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80fc-113">Type</span></span>   |<span data-ttu-id="e80fc-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80fc-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e80fc-115">id</span><span class="sxs-lookup"><span data-stu-id="e80fc-115">id</span></span>|<span data-ttu-id="e80fc-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="e80fc-116">String</span></span>| <span data-ttu-id="e80fc-p102">Somente leitura. O identificador do **plannerGroup**</span><span class="sxs-lookup"><span data-stu-id="e80fc-p102">Read-only. Identifier of the **plannerGroup**</span></span>|

## <a name="relationships"></a><span data-ttu-id="e80fc-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e80fc-119">Relationships</span></span>
| <span data-ttu-id="e80fc-120">Relação</span><span class="sxs-lookup"><span data-stu-id="e80fc-120">Relationship</span></span> | <span data-ttu-id="e80fc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80fc-121">Type</span></span>   |<span data-ttu-id="e80fc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80fc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e80fc-123">plans</span><span class="sxs-lookup"><span data-stu-id="e80fc-123">plans</span></span>|<span data-ttu-id="e80fc-124">Coleção [plannerPlan](plannerplan.md)</span><span class="sxs-lookup"><span data-stu-id="e80fc-124">[plannerPlan](plannerplan.md) collection</span></span>| <span data-ttu-id="e80fc-p103">Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.</span><span class="sxs-lookup"><span data-stu-id="e80fc-p103">Read-only. Nullable. Returns the [plannerPlans](plannerplan.md) owned by the group.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e80fc-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e80fc-128">JSON representation</span></span>
<span data-ttu-id="e80fc-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e80fc-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
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
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->