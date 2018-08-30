# <a name="chartdatalabels-resource-type"></a><span data-ttu-id="bdf12-101">Tipo de recurso ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="bdf12-101">ChartDataLabels resource type</span></span>

<span data-ttu-id="bdf12-102">Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.</span><span class="sxs-lookup"><span data-stu-id="bdf12-102">Represents a collection of all the data labels on a chart point.</span></span>


## <a name="methods"></a><span data-ttu-id="bdf12-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="bdf12-103">Methods</span></span>

| <span data-ttu-id="bdf12-104">Método</span><span class="sxs-lookup"><span data-stu-id="bdf12-104">Method</span></span>           | <span data-ttu-id="bdf12-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bdf12-105">Return Type</span></span>    |<span data-ttu-id="bdf12-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf12-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bdf12-107">Get ChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="bdf12-107">Get ChartDataLabels</span></span>](../api/chartdatalabels_get.md) | [<span data-ttu-id="bdf12-108">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="bdf12-108">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="bdf12-109">Leia as propriedades e os relacionamentos do objeto chartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="bdf12-109">Read properties and relationships of chartDataLabels object.</span></span>|
|[<span data-ttu-id="bdf12-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="bdf12-110">Update</span></span>](../api/chartdatalabels_update.md) | [<span data-ttu-id="bdf12-111">WorkbookChartDataLabels</span><span class="sxs-lookup"><span data-stu-id="bdf12-111">WorkbookChartDataLabels</span></span>](chartdatalabels.md) |<span data-ttu-id="bdf12-112">Atualize o objeto ChartDataLabels.</span><span class="sxs-lookup"><span data-stu-id="bdf12-112">Update ChartDataLabels object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bdf12-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdf12-113">Properties</span></span>
| <span data-ttu-id="bdf12-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf12-114">Property</span></span>     | <span data-ttu-id="bdf12-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf12-115">Type</span></span>   |<span data-ttu-id="bdf12-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf12-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdf12-117">position</span><span class="sxs-lookup"><span data-stu-id="bdf12-117">position</span></span>|<span data-ttu-id="bdf12-118">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdf12-118">string</span></span>|<span data-ttu-id="bdf12-119">Valor de DataLabelPosition que representa a posição do rótulo de dados.</span><span class="sxs-lookup"><span data-stu-id="bdf12-119">DataLabelPosition value that represents the position of the data label. Possible values are: , , , , , , , , , , .</span></span> <span data-ttu-id="bdf12-120">Os valores possíveis são: `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`.</span><span class="sxs-lookup"><span data-stu-id="bdf12-120">The possible values are `None`, `Center`, `InsideEnd`, `InsideBase`, `OutsideEnd`, `Left`, `Right`, `Top`, `Bottom`, `BestFit`, `Callout`, or .</span></span>|
|<span data-ttu-id="bdf12-121">separador</span><span class="sxs-lookup"><span data-stu-id="bdf12-121">separator</span></span>|<span data-ttu-id="bdf12-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdf12-122">string</span></span>|<span data-ttu-id="bdf12-123">Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.</span><span class="sxs-lookup"><span data-stu-id="bdf12-123">String representing the separator used for the data labels on a chart.</span></span>|
|<span data-ttu-id="bdf12-124">showBubbleSize</span><span class="sxs-lookup"><span data-stu-id="bdf12-124">showBubbleSize</span></span>|<span data-ttu-id="bdf12-125">booleano</span><span class="sxs-lookup"><span data-stu-id="bdf12-125">boolean</span></span>|<span data-ttu-id="bdf12-126">Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-126">Boolean value representing if the data label bubble size is visible or not.</span></span>|
|<span data-ttu-id="bdf12-127">showCategoryName</span><span class="sxs-lookup"><span data-stu-id="bdf12-127">showCategoryName</span></span>|<span data-ttu-id="bdf12-128">booliano</span><span class="sxs-lookup"><span data-stu-id="bdf12-128">boolean</span></span>|<span data-ttu-id="bdf12-129">Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-129">Boolean value representing if the data label category name is visible or not.</span></span>|
|<span data-ttu-id="bdf12-130">showLegendKey</span><span class="sxs-lookup"><span data-stu-id="bdf12-130">showLegendKey</span></span>|<span data-ttu-id="bdf12-131">booliano</span><span class="sxs-lookup"><span data-stu-id="bdf12-131">boolean</span></span>|<span data-ttu-id="bdf12-132">Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-132">Boolean value representing if the data label legend key is visible or not.</span></span>|
|<span data-ttu-id="bdf12-133">showPercentage</span><span class="sxs-lookup"><span data-stu-id="bdf12-133">showPercentage</span></span>|<span data-ttu-id="bdf12-134">booleano</span><span class="sxs-lookup"><span data-stu-id="bdf12-134">boolean</span></span>|<span data-ttu-id="bdf12-135">Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-135">Boolean value representing if the data label percentage is visible or not.</span></span>|
|<span data-ttu-id="bdf12-136">showSeriesName</span><span class="sxs-lookup"><span data-stu-id="bdf12-136">showSeriesName</span></span>|<span data-ttu-id="bdf12-137">booliano</span><span class="sxs-lookup"><span data-stu-id="bdf12-137">boolean</span></span>|<span data-ttu-id="bdf12-138">Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-138">Boolean value representing if the data label series name is visible or not.</span></span>|
|<span data-ttu-id="bdf12-139">showValue</span><span class="sxs-lookup"><span data-stu-id="bdf12-139">showValue</span></span>|<span data-ttu-id="bdf12-140">booliano</span><span class="sxs-lookup"><span data-stu-id="bdf12-140">boolean</span></span>|<span data-ttu-id="bdf12-141">Valor booliano que determina se o valor do rótulo de dados fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="bdf12-141">Boolean value representing if the data label value is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdf12-142">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="bdf12-142">Relationships</span></span>
| <span data-ttu-id="bdf12-143">Relação</span><span class="sxs-lookup"><span data-stu-id="bdf12-143">Relationship</span></span> | <span data-ttu-id="bdf12-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf12-144">Type</span></span>   |<span data-ttu-id="bdf12-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf12-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bdf12-146">formato</span><span class="sxs-lookup"><span data-stu-id="bdf12-146">format</span></span>|[<span data-ttu-id="bdf12-147">WorkbookChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="bdf12-147">WorkbookChartDataLabelFormat</span></span>](chartdatalabelformat.md)|<span data-ttu-id="bdf12-p102">Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf12-p102">Represents the format of chart data labels, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bdf12-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdf12-150">JSON representation</span></span>

<span data-ttu-id="bdf12-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdf12-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->