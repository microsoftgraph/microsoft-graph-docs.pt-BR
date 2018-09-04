# <a name="chartlineformat-resource-type"></a><span data-ttu-id="1a1cb-101">Tipo de recurso ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="1a1cb-101">ChartLineFormat resource type</span></span>

<span data-ttu-id="1a1cb-102">Abrange as opções de formatação dos elementos de linha.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-102">Enapsulates the formatting options for line elements.</span></span>


## <a name="methods"></a><span data-ttu-id="1a1cb-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a1cb-103">Methods</span></span>

| <span data-ttu-id="1a1cb-104">Método</span><span class="sxs-lookup"><span data-stu-id="1a1cb-104">Method</span></span>           | <span data-ttu-id="1a1cb-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a1cb-105">Return Type</span></span>    |<span data-ttu-id="1a1cb-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1cb-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1a1cb-107">Obter ChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="1a1cb-107">Get ChartLineFormat</span></span>](../api/chartlineformat_get.md) | [<span data-ttu-id="1a1cb-108">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="1a1cb-108">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="1a1cb-109">Propriedades de leitura e relacionamentos do objeto chartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-109">Read properties and relationships of chartLineFormat object.</span></span>|
|[<span data-ttu-id="1a1cb-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="1a1cb-110">Update</span></span>](../api/chartlineformat_update.md) | [<span data-ttu-id="1a1cb-111">WorkbookChartLineFormat</span><span class="sxs-lookup"><span data-stu-id="1a1cb-111">WorkbookChartLineFormat</span></span>](chartlineformat.md) |<span data-ttu-id="1a1cb-112">Atualize o objeto ChartLineFormat.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-112">Update ChartLineFormat object.</span></span> |
|[<span data-ttu-id="1a1cb-113">Limpar</span><span class="sxs-lookup"><span data-stu-id="1a1cb-113">Clear</span></span>](../api/chartlineformat_clear.md)|<span data-ttu-id="1a1cb-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a1cb-114">None</span></span>|<span data-ttu-id="1a1cb-115">Limpe a formatação da linha de um elemento do gráfico.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-115">Clear the line format of a chart element.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a1cb-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a1cb-116">Properties</span></span>
| <span data-ttu-id="1a1cb-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a1cb-117">Property</span></span>     | <span data-ttu-id="1a1cb-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1cb-118">Type</span></span>   |<span data-ttu-id="1a1cb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1cb-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1cb-120">color</span><span class="sxs-lookup"><span data-stu-id="1a1cb-120">color</span></span>|<span data-ttu-id="1a1cb-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1cb-121">string</span></span>|<span data-ttu-id="1a1cb-122">Código de cor HTML que representa a cor das linhas no gráfico.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-122">HTML color code representing the color of lines in the chart.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1cb-123">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="1a1cb-123">Relationships</span></span>
<span data-ttu-id="1a1cb-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a1cb-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1a1cb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a1cb-125">JSON representation</span></span>

<span data-ttu-id="1a1cb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a1cb-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->