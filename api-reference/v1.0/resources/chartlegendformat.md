# <a name="chartlegendformat-resource-type"></a><span data-ttu-id="19f32-101">Tipo de recurso ChartLegendFormat</span><span class="sxs-lookup"><span data-stu-id="19f32-101">ChartLegendFormat resource type</span></span>

<span data-ttu-id="19f32-102">Abrange as propriedades de formato de uma legenda de gráfico.</span><span class="sxs-lookup"><span data-stu-id="19f32-102">Encapsulates the format properties of a chart legend.</span></span>


## <a name="methods"></a><span data-ttu-id="19f32-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="19f32-103">Methods</span></span>
<span data-ttu-id="19f32-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19f32-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="19f32-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19f32-105">Properties</span></span>
<span data-ttu-id="19f32-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19f32-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="19f32-107">Relações</span><span class="sxs-lookup"><span data-stu-id="19f32-107">Relationships</span></span>
| <span data-ttu-id="19f32-108">Relação</span><span class="sxs-lookup"><span data-stu-id="19f32-108">Relationship</span></span> | <span data-ttu-id="19f32-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="19f32-109">Type</span></span>   |<span data-ttu-id="19f32-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="19f32-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f32-111">fill</span><span class="sxs-lookup"><span data-stu-id="19f32-111">fill</span></span>|[<span data-ttu-id="19f32-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="19f32-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="19f32-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="19f32-p101">Represents the fill format of an object, which includes background formating information. Read-only.</span></span>|
|<span data-ttu-id="19f32-115">font</span><span class="sxs-lookup"><span data-stu-id="19f32-115">font</span></span>|[<span data-ttu-id="19f32-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="19f32-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="19f32-p102">Representa os atributos de fonte, como nome, tamanho, cor, etc. de uma legenda de gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="19f32-p102">Represents the font attributes such as font name, font size, color, etc. of a chart legend. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="19f32-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19f32-119">JSON representation</span></span>

<span data-ttu-id="19f32-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19f32-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartLegendFormat"
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
  "description": "ChartLegendFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->