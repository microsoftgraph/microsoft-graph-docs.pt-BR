# <a name="chartseriesformat-resource-type"></a><span data-ttu-id="90e40-101">Tipo de recurso ChartSeriesFormat</span><span class="sxs-lookup"><span data-stu-id="90e40-101">ChartSeriesFormat resource type</span></span>

<span data-ttu-id="90e40-102">Abrange as propriedades de formatação da série do gráfico.</span><span class="sxs-lookup"><span data-stu-id="90e40-102">encapsulates the format properties for the chart series</span></span>


## <a name="methods"></a><span data-ttu-id="90e40-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="90e40-103">Methods</span></span>
<span data-ttu-id="90e40-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90e40-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="90e40-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90e40-105">Properties</span></span>
<span data-ttu-id="90e40-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90e40-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="90e40-107">Relações</span><span class="sxs-lookup"><span data-stu-id="90e40-107">Relationships</span></span>
| <span data-ttu-id="90e40-108">Relação</span><span class="sxs-lookup"><span data-stu-id="90e40-108">Relationship</span></span> | <span data-ttu-id="90e40-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="90e40-109">Type</span></span>   |<span data-ttu-id="90e40-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90e40-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90e40-111">fill</span><span class="sxs-lookup"><span data-stu-id="90e40-111">fill</span></span>|[<span data-ttu-id="90e40-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="90e40-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="90e40-p101">Representa o formato de preenchimento de uma série do gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90e40-p101">Represents the fill format of a chart series, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="90e40-115">line</span><span class="sxs-lookup"><span data-stu-id="90e40-115">line</span></span>|[<span data-ttu-id="90e40-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="90e40-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="90e40-p102">Representa a formatação de linha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90e40-p102">Represents line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="90e40-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90e40-119">JSON representation</span></span>

<span data-ttu-id="90e40-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90e40-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartSeriesFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeriesFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->