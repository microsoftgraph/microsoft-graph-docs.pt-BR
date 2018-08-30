# <a name="chartaxistitleformat-resource-type"></a><span data-ttu-id="e6d6d-101">Tipo de recurso ChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="e6d6d-101">ChartAxisTitleFormat resource type</span></span>

<span data-ttu-id="e6d6d-102">Representa a formatação do título do eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="e6d6d-102">Represents the chart axis title formatting.</span></span>


## <a name="methods"></a><span data-ttu-id="e6d6d-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6d6d-103">Methods</span></span>
<span data-ttu-id="e6d6d-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6d6d-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="e6d6d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6d6d-105">Properties</span></span>
<span data-ttu-id="e6d6d-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6d6d-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e6d6d-107">Relações</span><span class="sxs-lookup"><span data-stu-id="e6d6d-107">Relationships</span></span>
| <span data-ttu-id="e6d6d-108">Relação</span><span class="sxs-lookup"><span data-stu-id="e6d6d-108">Relationship</span></span> | <span data-ttu-id="e6d6d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6d6d-109">Type</span></span>   |<span data-ttu-id="e6d6d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6d6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6d6d-111">font</span><span class="sxs-lookup"><span data-stu-id="e6d6d-111">font</span></span>|[<span data-ttu-id="e6d6d-112">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="e6d6d-112">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="e6d6d-p101">Representa os atributos de fonte, como nome, tamanho, cor etc., do objeto do título do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6d6d-p101">Represents the font attributes, such as font name, font size, color, etc. of chart axis title object. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6d6d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6d6d-115">JSON representation</span></span>

<span data-ttu-id="e6d6d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6d6d-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxisTitleFormat"
}-->

```json
{
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->