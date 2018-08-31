# <a name="chartpointformat-resource-type"></a><span data-ttu-id="51e2d-101">Tipo de recurso ChartPointFormat</span><span class="sxs-lookup"><span data-stu-id="51e2d-101">ChartPointFormat resource type</span></span>

<span data-ttu-id="51e2d-102">Representa um objeto de formatação para os pontos do gráfico.</span><span class="sxs-lookup"><span data-stu-id="51e2d-102">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="51e2d-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="51e2d-103">Methods</span></span>
<span data-ttu-id="51e2d-104">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51e2d-104">None</span></span>

## <a name="properties"></a><span data-ttu-id="51e2d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51e2d-105">Properties</span></span>
<span data-ttu-id="51e2d-106">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51e2d-106">None</span></span>

## <a name="relationships"></a><span data-ttu-id="51e2d-107">Relações</span><span class="sxs-lookup"><span data-stu-id="51e2d-107">Relationships</span></span>
| <span data-ttu-id="51e2d-108">Relação</span><span class="sxs-lookup"><span data-stu-id="51e2d-108">Relationship</span></span> | <span data-ttu-id="51e2d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e2d-109">Type</span></span>   |<span data-ttu-id="51e2d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e2d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51e2d-111">fill</span><span class="sxs-lookup"><span data-stu-id="51e2d-111">fill</span></span>|[<span data-ttu-id="51e2d-112">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="51e2d-112">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="51e2d-p101">Representa o formato de preenchimento de um gráfico, que inclui informações sobre a formatação da tela de fundo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51e2d-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="51e2d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51e2d-115">JSON representation</span></span>

<span data-ttu-id="51e2d-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51e2d-116">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->