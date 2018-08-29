# <a name="charttitleformat-resource-type"></a><span data-ttu-id="81306-101">Tipo de recurso ChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="81306-101">ChartTitleFormat resource type</span></span>

<span data-ttu-id="81306-102">Abrange as propriedades de formatação do título do gráfico.</span><span class="sxs-lookup"><span data-stu-id="81306-102">Encapsulates the format properties for the chart title.</span></span>


## <a name="methods"></a><span data-ttu-id="81306-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="81306-103">Methods</span></span>
<span data-ttu-id="81306-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81306-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="81306-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81306-105">Properties</span></span>
<span data-ttu-id="81306-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81306-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="81306-107">Relações</span><span class="sxs-lookup"><span data-stu-id="81306-107">Relationships</span></span>
| <span data-ttu-id="81306-108">Relação</span><span class="sxs-lookup"><span data-stu-id="81306-108">Relationship</span></span> | <span data-ttu-id="81306-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81306-109">Type</span></span>   |<span data-ttu-id="81306-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81306-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81306-111">fill</span><span class="sxs-lookup"><span data-stu-id="81306-111">fill</span></span>|[<span data-ttu-id="81306-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="81306-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="81306-p101">Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81306-p101">Represents the fill format of an object, which includes background formatting information. Read-only.</span></span>|
|<span data-ttu-id="81306-115">font</span><span class="sxs-lookup"><span data-stu-id="81306-115">font</span></span>|[<span data-ttu-id="81306-116">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="81306-116">WorkbookChartFont</span></span>](chartfont.md)|<span data-ttu-id="81306-p102">Representa os atributos de fonte do objeto atual (nome, tamanho, cor, dentre outros). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="81306-p102">Represents the font attributes (font name, font size, color, etc.) for the current object. Read-only.</span></span>|



## <a name="json-representation"></a><span data-ttu-id="81306-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81306-119">JSON representation</span></span>

<span data-ttu-id="81306-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81306-120">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
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
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
