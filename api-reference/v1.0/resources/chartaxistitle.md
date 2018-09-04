# <a name="chartaxistitle-resource-type"></a><span data-ttu-id="503bb-101">Tipo de recurso ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="503bb-101">ChartAxisTitle resource type</span></span>

<span data-ttu-id="503bb-102">Representa o título de um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="503bb-102">Represents the title of a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="503bb-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="503bb-103">Methods</span></span>

| <span data-ttu-id="503bb-104">Método</span><span class="sxs-lookup"><span data-stu-id="503bb-104">Method</span></span>           | <span data-ttu-id="503bb-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="503bb-105">Return Type</span></span>    |<span data-ttu-id="503bb-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="503bb-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="503bb-107">Obter ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="503bb-107">Get ChartAxisTitle</span></span>](../api/chartaxistitle_get.md) | [<span data-ttu-id="503bb-108">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="503bb-108">WorkbookChartAxisTitle</span></span>](chartaxistitle.md) |<span data-ttu-id="503bb-109">Recupere as propriedades e os relacionamentos do objeto chartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="503bb-109">Read properties and relationships of chartAxisTitle object.</span></span>|
|[<span data-ttu-id="503bb-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="503bb-110">Update</span></span>](../api/chartaxistitle_update.md) | [<span data-ttu-id="503bb-111">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="503bb-111">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)    |<span data-ttu-id="503bb-112">Atualize o objeto ChartAxisTitle.</span><span class="sxs-lookup"><span data-stu-id="503bb-112">Update ChartAxisTitle object.</span></span> |

## <a name="properties"></a><span data-ttu-id="503bb-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="503bb-113">Properties</span></span>
| <span data-ttu-id="503bb-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="503bb-114">Property</span></span>     | <span data-ttu-id="503bb-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="503bb-115">Type</span></span>   |<span data-ttu-id="503bb-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="503bb-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="503bb-117">texto</span><span class="sxs-lookup"><span data-stu-id="503bb-117">text</span></span>|<span data-ttu-id="503bb-118">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="503bb-118">string</span></span>|<span data-ttu-id="503bb-119">Representa o título do eixo.</span><span class="sxs-lookup"><span data-stu-id="503bb-119">Represents the axis title.</span></span>|
|<span data-ttu-id="503bb-120">visível</span><span class="sxs-lookup"><span data-stu-id="503bb-120">visible</span></span>|<span data-ttu-id="503bb-121">booliano</span><span class="sxs-lookup"><span data-stu-id="503bb-121">boolean</span></span>|<span data-ttu-id="503bb-122">Um booliano que especifica a visibilidade de um título do eixo.</span><span class="sxs-lookup"><span data-stu-id="503bb-122">A boolean that specifies the visibility of an axis title.</span></span>|

## <a name="relationships"></a><span data-ttu-id="503bb-123">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="503bb-123">Relationships</span></span>
| <span data-ttu-id="503bb-124">Relação</span><span class="sxs-lookup"><span data-stu-id="503bb-124">Relationship</span></span> | <span data-ttu-id="503bb-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="503bb-125">Type</span></span>   |<span data-ttu-id="503bb-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="503bb-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="503bb-127">formato</span><span class="sxs-lookup"><span data-stu-id="503bb-127">format</span></span>|[<span data-ttu-id="503bb-128">WorkbookChartAxisTitleFormat</span><span class="sxs-lookup"><span data-stu-id="503bb-128">WorkbookChartAxisTitleFormat</span></span>](chartaxistitleformat.md)|<span data-ttu-id="503bb-p101">Representa a formatação do título do eixo do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="503bb-p101">Represents the formatting of chart axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="503bb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="503bb-131">JSON representation</span></span>

<span data-ttu-id="503bb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="503bb-132">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true,
  "format": {"@odata.type":"microsoft.graph.workbookChartAxisTitleFormat"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->