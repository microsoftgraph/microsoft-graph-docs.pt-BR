# <a name="chartpoint-resource-type"></a><span data-ttu-id="e6f25-101">Tipo de recurso ChartPoint</span><span class="sxs-lookup"><span data-stu-id="e6f25-101">ChartPoint resource type</span></span>

<span data-ttu-id="e6f25-102">Representa um ponto de uma série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e6f25-102">Represents a point of a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="e6f25-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6f25-103">Methods</span></span>

| <span data-ttu-id="e6f25-104">Método</span><span class="sxs-lookup"><span data-stu-id="e6f25-104">Method</span></span>           | <span data-ttu-id="e6f25-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6f25-105">Return Type</span></span>    |<span data-ttu-id="e6f25-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f25-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6f25-107">Get ChartPoint</span><span class="sxs-lookup"><span data-stu-id="e6f25-107">Get ChartPoint</span></span>](../api/chartpoint_get.md) | [<span data-ttu-id="e6f25-108">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="e6f25-108">WorkbookChartPoint</span></span>](chartpoint.md) |<span data-ttu-id="e6f25-109">Leia as propriedades e os relacionamentos do objeto chartPoint.</span><span class="sxs-lookup"><span data-stu-id="e6f25-109">Read properties and relationships of chartPoint object.</span></span>|
|[<span data-ttu-id="e6f25-110">Lista</span><span class="sxs-lookup"><span data-stu-id="e6f25-110">List</span></span>](../api/chartpoint_list.md) | <span data-ttu-id="e6f25-111">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="e6f25-111">[WorkbookChartPoint](chartpoint.md) collection</span></span> |<span data-ttu-id="e6f25-112">Obtenha a coleção de objetos chartPoint.</span><span class="sxs-lookup"><span data-stu-id="e6f25-112">Get chartPoint object collection.</span></span> |
|[<span data-ttu-id="e6f25-113">ItemAt</span><span class="sxs-lookup"><span data-stu-id="e6f25-113">Itemat</span></span>](../api/chartpointscollection_itemat.md)|[<span data-ttu-id="e6f25-114">WorkbookChartPoint</span><span class="sxs-lookup"><span data-stu-id="e6f25-114">WorkbookChartPoint</span></span>](chartpoint.md)|<span data-ttu-id="e6f25-115">Recupera um ponto com base na respectiva posição dentro da série.</span><span class="sxs-lookup"><span data-stu-id="e6f25-115">Retrieve a point based on its position within the series.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6f25-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6f25-116">Properties</span></span>
| <span data-ttu-id="e6f25-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6f25-117">Property</span></span>     | <span data-ttu-id="e6f25-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6f25-118">Type</span></span>   |<span data-ttu-id="e6f25-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f25-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f25-120">value</span><span class="sxs-lookup"><span data-stu-id="e6f25-120">value</span></span>|<span data-ttu-id="e6f25-121">Json</span><span class="sxs-lookup"><span data-stu-id="e6f25-121">Json</span></span>|<span data-ttu-id="e6f25-p101">Retorna o valor de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6f25-p101">Returns the value of a chart point. Read-only.</span></span>|
|<span data-ttu-id="e6f25-124">id</span><span class="sxs-lookup"><span data-stu-id="e6f25-124">id</span></span>|<span data-ttu-id="e6f25-125">string</span><span class="sxs-lookup"><span data-stu-id="e6f25-125">string</span></span>|<span data-ttu-id="e6f25-126">identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="e6f25-126">unique identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6f25-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e6f25-127">Relationships</span></span>
| <span data-ttu-id="e6f25-128">Relação</span><span class="sxs-lookup"><span data-stu-id="e6f25-128">Relationship</span></span> | <span data-ttu-id="e6f25-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6f25-129">Type</span></span>   |<span data-ttu-id="e6f25-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6f25-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f25-131">formato</span><span class="sxs-lookup"><span data-stu-id="e6f25-131">format</span></span>|[<span data-ttu-id="e6f25-132">WorkbookChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="e6f25-132">WorkbookChartPointFormat</span></span>](chartpointformat.md)|<span data-ttu-id="e6f25-p102">Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6f25-p102">Encapsulates the format properties chart point. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6f25-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6f25-135">JSON representation</span></span>

<span data-ttu-id="e6f25-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6f25-136">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPoint"
}-->

```json
{
  "value": "string",
  "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->