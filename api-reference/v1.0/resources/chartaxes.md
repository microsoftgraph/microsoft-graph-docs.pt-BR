# <a name="chartaxes-resource-type"></a><span data-ttu-id="04be4-101">Tipo de recurso ChartAxes</span><span class="sxs-lookup"><span data-stu-id="04be4-101">ChartAxes resource type</span></span>

<span data-ttu-id="04be4-102">Representa os eixos de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="04be4-102">Represents the chart axes.</span></span>


## <a name="methods"></a><span data-ttu-id="04be4-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="04be4-103">Methods</span></span>
<span data-ttu-id="04be4-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04be4-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="04be4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04be4-105">Properties</span></span>
<span data-ttu-id="04be4-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04be4-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="04be4-107">Relações</span><span class="sxs-lookup"><span data-stu-id="04be4-107">Relationships</span></span>
| <span data-ttu-id="04be4-108">Relação</span><span class="sxs-lookup"><span data-stu-id="04be4-108">Relationship</span></span> | <span data-ttu-id="04be4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="04be4-109">Type</span></span>   |<span data-ttu-id="04be4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="04be4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04be4-111">categoryAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-111">categoryAxis</span></span>|[<span data-ttu-id="04be4-112">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-112">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="04be4-p101">Representa o eixo de categoria em um gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04be4-p101">Represents the category axis in a chart. Read-only.</span></span>|
|<span data-ttu-id="04be4-115">seriesAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-115">seriesAxis</span></span>|[<span data-ttu-id="04be4-116">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-116">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="04be4-p102">Representa o eixo das séries de um gráfico 3D. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04be4-p102">Represents the series axis of a 3-dimensional chart. Read-only.</span></span>|
|<span data-ttu-id="04be4-119">valueAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-119">valueAxis</span></span>|[<span data-ttu-id="04be4-120">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="04be4-120">WorkbookChartAxis</span></span>](chartaxis.md)|<span data-ttu-id="04be4-p103">Representa o eixo dos valores em um eixo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="04be4-p103">Represents the value axis in an axis. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="04be4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04be4-123">JSON representation</span></span>

<span data-ttu-id="04be4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04be4-124">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxes"
}-->

```json
{
  "categoryAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "seriesAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"},
  "valueAxis": {"@odata.type": "microsoft.graph.workbookChartAxis"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->