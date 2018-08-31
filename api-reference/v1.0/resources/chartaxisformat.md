# <a name="chartaxisformat-resource-type"></a><span data-ttu-id="2b12e-101">Tipo de recurso ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="2b12e-101">ChartAxisFormat resource type</span></span>

<span data-ttu-id="2b12e-102">Abrange as propriedades de formatação do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="2b12e-102">Encapsulates the format properties for the chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="2b12e-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b12e-103">Methods</span></span>
<span data-ttu-id="2b12e-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b12e-104">None</span></span>
## <a name="properties"></a><span data-ttu-id="2b12e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b12e-105">Properties</span></span>
<span data-ttu-id="2b12e-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b12e-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="2b12e-107">Relações</span><span class="sxs-lookup"><span data-stu-id="2b12e-107">Relationships</span></span>
| <span data-ttu-id="2b12e-108">Relação</span><span class="sxs-lookup"><span data-stu-id="2b12e-108">Relationship</span></span> | <span data-ttu-id="2b12e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b12e-109">Type</span></span>   |<span data-ttu-id="2b12e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b12e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b12e-111">font</span><span class="sxs-lookup"><span data-stu-id="2b12e-111">font</span></span>|[<span data-ttu-id="2b12e-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="2b12e-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="2b12e-p101">Representa os atributos de fonte (nome, tamanho, cor etc.) de um elemento do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b12e-p101">Represents the font attributes (font name, font size, color, etc.) for a chart axis element. Read-only.</span></span>|
|<span data-ttu-id="2b12e-115">line</span><span class="sxs-lookup"><span data-stu-id="2b12e-115">line</span></span>|[<span data-ttu-id="2b12e-116">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="2b12e-116">WorkbookChartLineFormat</span></span>](chartlineformat.md)|<span data-ttu-id="2b12e-p102">Representa a formatação de linha do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b12e-p102">Represents chart line formatting. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2b12e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b12e-119">JSON representation</span></span>

<span data-ttu-id="2b12e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b12e-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"},
  "line": {"@odata.type": "microsoft.graph.workbookChartLineFormat"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->