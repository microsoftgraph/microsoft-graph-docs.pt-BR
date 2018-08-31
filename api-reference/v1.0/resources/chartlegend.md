# <a name="chartlegend-resource-type"></a><span data-ttu-id="b807b-101">Tipo de recurso ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b807b-101">ChartLegend resource type</span></span>

<span data-ttu-id="b807b-102">Representa a legenda de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="b807b-102">Represents the legend in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="b807b-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="b807b-103">Methods</span></span>

| <span data-ttu-id="b807b-104">Método</span><span class="sxs-lookup"><span data-stu-id="b807b-104">Method</span></span>           | <span data-ttu-id="b807b-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b807b-105">Return Type</span></span>    |<span data-ttu-id="b807b-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b807b-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b807b-107">Get ChartLegend</span><span class="sxs-lookup"><span data-stu-id="b807b-107">Get ChartLegend</span></span>](../api/chartlegend_get.md) | [<span data-ttu-id="b807b-108">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b807b-108">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b807b-109">Propriedades de leitura e relacionamentos do objeto chartLegend.</span><span class="sxs-lookup"><span data-stu-id="b807b-109">Read properties and relationships of chartLegend object.</span></span>|
|[<span data-ttu-id="b807b-110">Update</span><span class="sxs-lookup"><span data-stu-id="b807b-110">Update</span></span>](../api/chartlegend_update.md) | [<span data-ttu-id="b807b-111">WorkbookChartLegend</span><span class="sxs-lookup"><span data-stu-id="b807b-111">WorkbookChartLegend</span></span>](chartlegend.md) |<span data-ttu-id="b807b-112">Atualize o objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="b807b-112">Update ChartLegend object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b807b-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b807b-113">Properties</span></span>
| <span data-ttu-id="b807b-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b807b-114">Property</span></span>     | <span data-ttu-id="b807b-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b807b-115">Type</span></span>   |<span data-ttu-id="b807b-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b807b-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b807b-117">overlay</span><span class="sxs-lookup"><span data-stu-id="b807b-117">overlay</span></span>|<span data-ttu-id="b807b-118">booliano</span><span class="sxs-lookup"><span data-stu-id="b807b-118">boolean</span></span>|<span data-ttu-id="b807b-119">Valor booliano para determinar se a legenda do gráfico deve se sobrepor ao corpo principal do gráfico.</span><span class="sxs-lookup"><span data-stu-id="b807b-119">Boolean value for whether the chart legend should overlap with the main body of the chart.</span></span>|
|<span data-ttu-id="b807b-120">position</span><span class="sxs-lookup"><span data-stu-id="b807b-120">position</span></span>|<span data-ttu-id="b807b-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b807b-121">string</span></span>|<span data-ttu-id="b807b-122">Representa a posição da legenda no gráfico.</span><span class="sxs-lookup"><span data-stu-id="b807b-122">Represents the position of the legend on the chart. Possible values are: , , , , , .</span></span> <span data-ttu-id="b807b-123">Os valores possíveis são: `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`.</span><span class="sxs-lookup"><span data-stu-id="b807b-123">The possible values are `Top`, `Bottom`, `Left`, `Right`, `Corner`, `Custom`, , , , , , or .</span></span>|
|<span data-ttu-id="b807b-124">visible</span><span class="sxs-lookup"><span data-stu-id="b807b-124">visible</span></span>|<span data-ttu-id="b807b-125">booliano</span><span class="sxs-lookup"><span data-stu-id="b807b-125">boolean</span></span>|<span data-ttu-id="b807b-126">Um valor booliano que representa a visibilidade de um objeto ChartLegend.</span><span class="sxs-lookup"><span data-stu-id="b807b-126">A boolean value the represents the visibility of a ChartLegend object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b807b-127">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="b807b-127">Relationships</span></span>
| <span data-ttu-id="b807b-128">Relação</span><span class="sxs-lookup"><span data-stu-id="b807b-128">Relationship</span></span> | <span data-ttu-id="b807b-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b807b-129">Type</span></span>   |<span data-ttu-id="b807b-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b807b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b807b-131">format</span><span class="sxs-lookup"><span data-stu-id="b807b-131">format</span></span>|[<span data-ttu-id="b807b-132">WorkbookChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="b807b-132">WorkbookChartLegendFormat</span></span>](chartlegendformat.md)|<span data-ttu-id="b807b-p102">Representa a formatação de uma legenda de gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b807b-p102">Represents the formatting of a chart legend, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b807b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b807b-135">JSON representation</span></span>

<span data-ttu-id="b807b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b807b-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartLegend"
}-->

```json
{
  "overlay": true,
  "position": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartLegendFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLegend resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->