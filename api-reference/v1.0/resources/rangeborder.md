# <a name="rangeborder-resource-type"></a><span data-ttu-id="deb93-101">Tipo de recurso RangeBorder</span><span class="sxs-lookup"><span data-stu-id="deb93-101">RangeBorder resource type</span></span>

<span data-ttu-id="deb93-102">Representa a borda de um objeto.</span><span class="sxs-lookup"><span data-stu-id="deb93-102">Represents the border of an object.</span></span>


## <a name="methods"></a><span data-ttu-id="deb93-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="deb93-103">Methods</span></span>

| <span data-ttu-id="deb93-104">Método</span><span class="sxs-lookup"><span data-stu-id="deb93-104">Method</span></span>           | <span data-ttu-id="deb93-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="deb93-105">Return Type</span></span>    |<span data-ttu-id="deb93-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="deb93-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="deb93-107">Get RangeBorder</span><span class="sxs-lookup"><span data-stu-id="deb93-107">Get RangeBorder</span></span>](../api/rangeborder_get.md) | [<span data-ttu-id="deb93-108">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="deb93-108">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="deb93-109">Propriedades de leitura e relacionamentos do objeto rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="deb93-109">Read properties and relationships of rangeBorder object.</span></span>|
|[<span data-ttu-id="deb93-110">Update</span><span class="sxs-lookup"><span data-stu-id="deb93-110">Update</span></span>](../api/rangeborder_update.md) | [<span data-ttu-id="deb93-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="deb93-111">WorkbookRangeBorder</span></span>](rangeborder.md) |<span data-ttu-id="deb93-112">Atualiza o objeto RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="deb93-112">Update RangeBorder object.</span></span> |
|[<span data-ttu-id="deb93-113">List</span><span class="sxs-lookup"><span data-stu-id="deb93-113">List</span></span>](../api/rangeborder_list.md) | <span data-ttu-id="deb93-114">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="deb93-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span> |<span data-ttu-id="deb93-115">Obtém a coleção de objetos rangeBorder.</span><span class="sxs-lookup"><span data-stu-id="deb93-115">Get rangeBorder object collection.</span></span> |
|[<span data-ttu-id="deb93-116">Itemat</span><span class="sxs-lookup"><span data-stu-id="deb93-116">Itemat</span></span>](../api/rangebordercollection_itemat.md)|[<span data-ttu-id="deb93-117">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="deb93-117">WorkbookRangeBorder</span></span>](rangeborder.md)|<span data-ttu-id="deb93-118">Obtém um objeto de borda usando seu índice</span><span class="sxs-lookup"><span data-stu-id="deb93-118">Gets a border object using its index</span></span>|

## <a name="properties"></a><span data-ttu-id="deb93-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="deb93-119">Properties</span></span>
| <span data-ttu-id="deb93-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="deb93-120">Property</span></span>     | <span data-ttu-id="deb93-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="deb93-121">Type</span></span>   |<span data-ttu-id="deb93-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="deb93-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="deb93-123">color</span><span class="sxs-lookup"><span data-stu-id="deb93-123">color</span></span>|<span data-ttu-id="deb93-124">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="deb93-124">string</span></span>|<span data-ttu-id="deb93-125">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="deb93-125">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange").</span></span>|
|<span data-ttu-id="deb93-126">id</span><span class="sxs-lookup"><span data-stu-id="deb93-126">id</span></span>|<span data-ttu-id="deb93-127">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="deb93-127">string</span></span>|<span data-ttu-id="deb93-128">Representa o identificador da borda.</span><span class="sxs-lookup"><span data-stu-id="deb93-128">Represents border identifier. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="deb93-129">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="deb93-129">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="deb93-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="deb93-130">Read-only.</span></span>|
|<span data-ttu-id="deb93-131">sideIndex</span><span class="sxs-lookup"><span data-stu-id="deb93-131">sideIndex</span></span>|<span data-ttu-id="deb93-132">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="deb93-132">string</span></span>|<span data-ttu-id="deb93-133">Valor constante que indica o lado específico da borda.</span><span class="sxs-lookup"><span data-stu-id="deb93-133">Constant value that indicates the specific side of the border. Possible values are: , , , , , , , . Read-only.</span></span> <span data-ttu-id="deb93-134">Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`.</span><span class="sxs-lookup"><span data-stu-id="deb93-134">The possible values are `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`, , , , or .</span></span> <span data-ttu-id="deb93-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="deb93-135">Read-only.</span></span>|
|<span data-ttu-id="deb93-136">style</span><span class="sxs-lookup"><span data-stu-id="deb93-136">style</span></span>|<span data-ttu-id="deb93-137">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="deb93-137">string</span></span>|<span data-ttu-id="deb93-138">Uma das constantes do estilo da linha, especificando o estilo da linha da borda.</span><span class="sxs-lookup"><span data-stu-id="deb93-138">One of the constants of line style specifying the line style for the border. Possible values are: , , , , , , , .</span></span> <span data-ttu-id="deb93-139">Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.</span><span class="sxs-lookup"><span data-stu-id="deb93-139">The possible values are `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`, , , , or .</span></span>|
|<span data-ttu-id="deb93-140">weight</span><span class="sxs-lookup"><span data-stu-id="deb93-140">weight</span></span>|<span data-ttu-id="deb93-141">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="deb93-141">string</span></span>|<span data-ttu-id="deb93-142">Especifica o peso da borda em um intervalo.</span><span class="sxs-lookup"><span data-stu-id="deb93-142">Specifies the weight of the border around a range.</span></span> <span data-ttu-id="deb93-143">Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.</span><span class="sxs-lookup"><span data-stu-id="deb93-143">The possible values are `Hairline`, `Thin`, `Medium`, `Thick`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="deb93-144">Relações</span><span class="sxs-lookup"><span data-stu-id="deb93-144">Relationships</span></span>
<span data-ttu-id="deb93-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="deb93-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="deb93-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="deb93-146">JSON representation</span></span>

<span data-ttu-id="deb93-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="deb93-147">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->