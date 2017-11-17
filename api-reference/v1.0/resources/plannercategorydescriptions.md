<span data-ttu-id="20505-p101">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto [plan details](plannerplandetails.md). Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="20505-p101">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span>

O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto [plan details](plannerplandetails.md). Pode haver até 6 categorias definidas. 


## <span data-ttu-id="20505-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20505-105">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="20505-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20505-106">Property</span></span>     | <span data-ttu-id="20505-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="20505-107">Type</span></span>   |<span data-ttu-id="20505-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="20505-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20505-109">categoria1</span><span class="sxs-lookup"><span data-stu-id="20505-109">category1</span></span>|<span data-ttu-id="20505-110">String</span><span class="sxs-lookup"><span data-stu-id="20505-110">String</span></span>|<span data-ttu-id="20505-111">O rótulo associado à Categoria 1.</span><span class="sxs-lookup"><span data-stu-id="20505-111">The label associated with Category 1</span></span>|
|<span data-ttu-id="20505-112">categoria2</span><span class="sxs-lookup"><span data-stu-id="20505-112">category2</span></span>|<span data-ttu-id="20505-113">String</span><span class="sxs-lookup"><span data-stu-id="20505-113">String</span></span>|<span data-ttu-id="20505-114">O rótulo associado à Categoria 2.</span><span class="sxs-lookup"><span data-stu-id="20505-114">The label associated with Category 2</span></span>|
|<span data-ttu-id="20505-115">categoria3</span><span class="sxs-lookup"><span data-stu-id="20505-115">category3</span></span>|<span data-ttu-id="20505-116">String</span><span class="sxs-lookup"><span data-stu-id="20505-116">String</span></span>|<span data-ttu-id="20505-117">O rótulo associado à Categoria 3.</span><span class="sxs-lookup"><span data-stu-id="20505-117">The label associated with Category 3</span></span>|
|<span data-ttu-id="20505-118">categoria4</span><span class="sxs-lookup"><span data-stu-id="20505-118">category4</span></span>|<span data-ttu-id="20505-119">String</span><span class="sxs-lookup"><span data-stu-id="20505-119">String</span></span>|<span data-ttu-id="20505-120">O rótulo associado à Categoria 4.</span><span class="sxs-lookup"><span data-stu-id="20505-120">The label associated with Category 4</span></span>|
|<span data-ttu-id="20505-121">categoria5</span><span class="sxs-lookup"><span data-stu-id="20505-121">category5</span></span>|<span data-ttu-id="20505-122">String</span><span class="sxs-lookup"><span data-stu-id="20505-122">String</span></span>|<span data-ttu-id="20505-123">O rótulo associado à Categoria 5.</span><span class="sxs-lookup"><span data-stu-id="20505-123">The label associated with Category 5</span></span>|
|<span data-ttu-id="20505-124">categoria6</span><span class="sxs-lookup"><span data-stu-id="20505-124">category6</span></span>|<span data-ttu-id="20505-125">String</span><span class="sxs-lookup"><span data-stu-id="20505-125">String</span></span>|<span data-ttu-id="20505-126">O rótulo associado à Categoria 6.</span><span class="sxs-lookup"><span data-stu-id="20505-126">The label associated with Category 6</span></span>|

## <span data-ttu-id="20505-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20505-127">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="20505-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20505-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->