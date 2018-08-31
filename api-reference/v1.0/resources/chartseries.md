# <a name="chartseries-resource-type"></a><span data-ttu-id="bca45-101">Tipo de recurso ChartSeries</span><span class="sxs-lookup"><span data-stu-id="bca45-101">ChartSeries resource type</span></span>

<span data-ttu-id="bca45-102">Representa uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="bca45-102">Represents a series in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="bca45-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="bca45-103">Methods</span></span>

| <span data-ttu-id="bca45-104">Método</span><span class="sxs-lookup"><span data-stu-id="bca45-104">Method</span></span>           | <span data-ttu-id="bca45-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bca45-105">Return Type</span></span>    |<span data-ttu-id="bca45-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca45-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bca45-107">Obter ChartSeries</span><span class="sxs-lookup"><span data-stu-id="bca45-107">Get ChartSeries</span></span>](../api/chartseries_get.md) | [<span data-ttu-id="bca45-108">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bca45-108">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="bca45-109">Leia as propriedades e as relações do objeto chartSeries.</span><span class="sxs-lookup"><span data-stu-id="bca45-109">Read properties and relationships of chartSeries object.</span></span>|
|[<span data-ttu-id="bca45-110">Criar ChartPoints</span><span class="sxs-lookup"><span data-stu-id="bca45-110">Create ChartPoints</span></span>](../api/chartseries_post_points.md) |[<span data-ttu-id="bca45-111">ChartPoints</span><span class="sxs-lookup"><span data-stu-id="bca45-111">ChartPoints</span></span>](chartpoint.md)| <span data-ttu-id="bca45-112">Crie um novo ChartPoints postando na coleção de pontos.</span><span class="sxs-lookup"><span data-stu-id="bca45-112">Create a new ChartPoints by posting to the points collection.</span></span>|
|[<span data-ttu-id="bca45-113">Listar pontos</span><span class="sxs-lookup"><span data-stu-id="bca45-113">List points</span></span>](../api/chartseries_list_points.md) |<span data-ttu-id="bca45-114">Coleção [ChartPoints](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="bca45-114">[ChartPoints](chartpoint.md) collection</span></span>| <span data-ttu-id="bca45-115">Obtenha uma coleção de objetos ChartPoints.</span><span class="sxs-lookup"><span data-stu-id="bca45-115">Get a ChartPoints object collection.</span></span>|
|[<span data-ttu-id="bca45-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="bca45-116">Update</span></span>](../api/chartseries_update.md) | [<span data-ttu-id="bca45-117">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bca45-117">WorkbookChartSeries</span></span>](chartseries.md) |<span data-ttu-id="bca45-118">Atualize o objeto ChartSeries.</span><span class="sxs-lookup"><span data-stu-id="bca45-118">Update ChartSeries object.</span></span> |
|[<span data-ttu-id="bca45-119">Lista</span><span class="sxs-lookup"><span data-stu-id="bca45-119">List</span></span>](../api/chartseries_list.md) | <span data-ttu-id="bca45-120">Coleção [WorkbookChartSeries](chartseries.md)</span><span class="sxs-lookup"><span data-stu-id="bca45-120">[WorkbookChartSeries](chartseries.md) collection</span></span> |<span data-ttu-id="bca45-121">Obtenha uma coleção de objetos chartSeries.</span><span class="sxs-lookup"><span data-stu-id="bca45-121">Get chartSeries object collection.</span></span> |
|[<span data-ttu-id="bca45-122">ItemAt</span><span class="sxs-lookup"><span data-stu-id="bca45-122">Itemat</span></span>](../api/chartseriescollection_itemat.md)|[<span data-ttu-id="bca45-123">WorkbookChartSeries</span><span class="sxs-lookup"><span data-stu-id="bca45-123">WorkbookChartSeries</span></span>](chartseries.md)|<span data-ttu-id="bca45-124">Recupera uma série com base em sua posição na coleção</span><span class="sxs-lookup"><span data-stu-id="bca45-124">Retrieves a series based on its position in the collection</span></span>|

## <a name="properties"></a><span data-ttu-id="bca45-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bca45-125">Properties</span></span>
| <span data-ttu-id="bca45-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bca45-126">Property</span></span>     | <span data-ttu-id="bca45-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca45-127">Type</span></span>   |<span data-ttu-id="bca45-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca45-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bca45-129">name</span><span class="sxs-lookup"><span data-stu-id="bca45-129">name</span></span>|<span data-ttu-id="bca45-130">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="bca45-130">string</span></span>|<span data-ttu-id="bca45-131">Representa o nome de uma série em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="bca45-131">Represents the name of a series in a chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca45-132">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="bca45-132">Relationships</span></span>
| <span data-ttu-id="bca45-133">Relação</span><span class="sxs-lookup"><span data-stu-id="bca45-133">Relationship</span></span> | <span data-ttu-id="bca45-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca45-134">Type</span></span>   |<span data-ttu-id="bca45-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca45-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bca45-136">format</span><span class="sxs-lookup"><span data-stu-id="bca45-136">format</span></span>|[<span data-ttu-id="bca45-137">WorkbookChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="bca45-137">WorkbookChartSeriesFormat</span></span>](chartseriesformat.md)|<span data-ttu-id="bca45-p101">Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bca45-p101">Represents the formatting of a chart series, which includes fill and line formatting. Read-only.</span></span>|
|<span data-ttu-id="bca45-140">points</span><span class="sxs-lookup"><span data-stu-id="bca45-140">points</span></span>|<span data-ttu-id="bca45-141">Coleção [WorkbookChartPoint](chartpoint.md)</span><span class="sxs-lookup"><span data-stu-id="bca45-141">[WorkbookChartPoint](chartpoint.md) collection</span></span>|<span data-ttu-id="bca45-p102">Representa uma coleção de todos os pontos da série. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bca45-p102">Represents a collection of all points in the series. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bca45-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bca45-144">JSON representation</span></span>

<span data-ttu-id="bca45-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bca45-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->