# <a name="chartdatalabelformat-resource-type"></a><span data-ttu-id="ba4c4-101">Tipo de recurso ChartDataLabelFormat</span><span class="sxs-lookup"><span data-stu-id="ba4c4-101">ChartDataLabelFormat resource type</span></span>

<span data-ttu-id="ba4c4-102">Abrange as propriedades de formatação dos rótulos de dados do gráfico.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-102">Encapsulates the format properties for the chart data labels.</span></span>


## <a name="methods"></a><span data-ttu-id="ba4c4-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="ba4c4-103">Methods</span></span>
<span data-ttu-id="ba4c4-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba4c4-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="ba4c4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba4c4-105">Properties</span></span>
<span data-ttu-id="ba4c4-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba4c4-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ba4c4-107">Relações</span><span class="sxs-lookup"><span data-stu-id="ba4c4-107">Relationships</span></span>
| <span data-ttu-id="ba4c4-108">Relação</span><span class="sxs-lookup"><span data-stu-id="ba4c4-108">Relationship</span></span> | <span data-ttu-id="ba4c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba4c4-109">Type</span></span>   |<span data-ttu-id="ba4c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba4c4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba4c4-111">fill</span><span class="sxs-lookup"><span data-stu-id="ba4c4-111">fill</span></span>|[<span data-ttu-id="ba4c4-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="ba4c4-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="ba4c4-p101">Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-p101">Represents the fill format of the current chart data label. Read-only.</span></span>|
|<span data-ttu-id="ba4c4-115">font</span><span class="sxs-lookup"><span data-stu-id="ba4c4-115">font</span></span>|[<span data-ttu-id="ba4c4-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="ba4c4-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="ba4c4-p102">Representa os atributos de fonte (nome, tamanho, cor, etc.) do rótulo de dados do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-p102">Represents the font attributes (font name, font size, color, etc.) for a chart data label. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ba4c4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba4c4-119">JSON representation</span></span>

<span data-ttu-id="ba4c4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba4c4-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->