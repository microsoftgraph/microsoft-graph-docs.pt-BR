# <a name="chartgridlines-resource-type"></a><span data-ttu-id="9656f-101">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9656f-101">ChartGridlines resource type</span></span>

<span data-ttu-id="9656f-102">Representa as linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="9656f-102">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="9656f-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="9656f-103">Methods</span></span>

| <span data-ttu-id="9656f-104">Método</span><span class="sxs-lookup"><span data-stu-id="9656f-104">Method</span></span>           | <span data-ttu-id="9656f-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9656f-105">Return Type</span></span>    |<span data-ttu-id="9656f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9656f-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9656f-107">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9656f-107">Get ChartGridlines</span></span>](../api/chartgridlines_get.md) | [<span data-ttu-id="9656f-108">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9656f-108">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="9656f-109">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="9656f-109">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="9656f-110">Update</span><span class="sxs-lookup"><span data-stu-id="9656f-110">Update</span></span>](../api/chartgridlines_update.md) | [<span data-ttu-id="9656f-111">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="9656f-111">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="9656f-112">Atualiza o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="9656f-112">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9656f-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9656f-113">Properties</span></span>
| <span data-ttu-id="9656f-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9656f-114">Property</span></span>     | <span data-ttu-id="9656f-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="9656f-115">Type</span></span>   |<span data-ttu-id="9656f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9656f-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9656f-117">visible</span><span class="sxs-lookup"><span data-stu-id="9656f-117">visible</span></span>|<span data-ttu-id="9656f-118">boolean</span><span class="sxs-lookup"><span data-stu-id="9656f-118">boolean</span></span>|<span data-ttu-id="9656f-119">Valor booleano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="9656f-119">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9656f-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9656f-120">Relationships</span></span>
| <span data-ttu-id="9656f-121">Relação</span><span class="sxs-lookup"><span data-stu-id="9656f-121">Relationship</span></span> | <span data-ttu-id="9656f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9656f-122">Type</span></span>   |<span data-ttu-id="9656f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9656f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9656f-124">formato</span><span class="sxs-lookup"><span data-stu-id="9656f-124">format</span></span>|[<span data-ttu-id="9656f-125">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="9656f-125">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="9656f-p101">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9656f-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9656f-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9656f-128">JSON representation</span></span>

<span data-ttu-id="9656f-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9656f-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->