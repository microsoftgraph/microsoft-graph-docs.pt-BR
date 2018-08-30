# <a name="charttitle-resource-type"></a><span data-ttu-id="f5cbc-101">Tipo de recurso ChartTitle</span><span class="sxs-lookup"><span data-stu-id="f5cbc-101">ChartTitle resource type</span></span>

<span data-ttu-id="f5cbc-102">Representa um objeto de título de gráfico de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-102">Represents a chart title object of a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f5cbc-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="f5cbc-103">Methods</span></span>

| <span data-ttu-id="f5cbc-104">Método</span><span class="sxs-lookup"><span data-stu-id="f5cbc-104">Method</span></span>           | <span data-ttu-id="f5cbc-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f5cbc-105">Return Type</span></span>    |<span data-ttu-id="f5cbc-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5cbc-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5cbc-107">Obter ChartTitle</span><span class="sxs-lookup"><span data-stu-id="f5cbc-107">Get ChartTitle</span></span>](../api/charttitle_get.md) | [<span data-ttu-id="f5cbc-108">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="f5cbc-108">WorkbookChartTitle</span></span>](charttitle.md) |<span data-ttu-id="f5cbc-109">Leia as propriedades e as relações do objeto chartTitle.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-109">Read properties and relationships of chartTitle object.</span></span>|
|[<span data-ttu-id="f5cbc-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="f5cbc-110">Update</span></span>](../api/charttitle_update.md) | [<span data-ttu-id="f5cbc-111">WorkbookChartTitle</span><span class="sxs-lookup"><span data-stu-id="f5cbc-111">WorkbookChartTitle</span></span>](charttitle.md)    |<span data-ttu-id="f5cbc-112">Atualize o objeto ChartTitle.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-112">Update ChartTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5cbc-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5cbc-113">Properties</span></span>
| <span data-ttu-id="f5cbc-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5cbc-114">Property</span></span>     | <span data-ttu-id="f5cbc-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5cbc-115">Type</span></span>   |<span data-ttu-id="f5cbc-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5cbc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5cbc-117">overlay</span><span class="sxs-lookup"><span data-stu-id="f5cbc-117">overlay</span></span>|<span data-ttu-id="f5cbc-118">booliano</span><span class="sxs-lookup"><span data-stu-id="f5cbc-118">boolean</span></span>|<span data-ttu-id="f5cbc-119">Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-119">Boolean value representing if the chart title will overlay the chart or not.</span></span>|
|<span data-ttu-id="f5cbc-120">texto</span><span class="sxs-lookup"><span data-stu-id="f5cbc-120">text</span></span>|<span data-ttu-id="f5cbc-121">string</span><span class="sxs-lookup"><span data-stu-id="f5cbc-121">string</span></span>|<span data-ttu-id="f5cbc-122">Representa o texto do título de um gráfico.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-122">Represents the title text of a chart.</span></span>|
|<span data-ttu-id="f5cbc-123">visible</span><span class="sxs-lookup"><span data-stu-id="f5cbc-123">visible</span></span>|<span data-ttu-id="f5cbc-124">booliano</span><span class="sxs-lookup"><span data-stu-id="f5cbc-124">boolean</span></span>|<span data-ttu-id="f5cbc-125">Um valor booliano que representa a visibilidade de um objeto de título de gráfico.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-125">A boolean value the represents the visibility of a chart title object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5cbc-126">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="f5cbc-126">Relationships</span></span>
| <span data-ttu-id="f5cbc-127">Relação</span><span class="sxs-lookup"><span data-stu-id="f5cbc-127">Relationship</span></span> | <span data-ttu-id="f5cbc-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5cbc-128">Type</span></span>   |<span data-ttu-id="f5cbc-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5cbc-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5cbc-130">format</span><span class="sxs-lookup"><span data-stu-id="f5cbc-130">format</span></span>|[<span data-ttu-id="f5cbc-131">WorkbookChartTitleFormat</span><span class="sxs-lookup"><span data-stu-id="f5cbc-131">WorkbookChartTitleFormat</span></span>](charttitleformat.md)|<span data-ttu-id="f5cbc-p101">Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-p101">Represents the formatting of a chart title, which includes fill and font formatting. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5cbc-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5cbc-134">JSON representation</span></span>

<span data-ttu-id="f5cbc-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5cbc-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->