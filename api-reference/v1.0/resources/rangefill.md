# <a name="rangefill-resource-type"></a><span data-ttu-id="9034d-101">Tipo de recurso RangeFill</span><span class="sxs-lookup"><span data-stu-id="9034d-101">RangeFill resource type</span></span>

<span data-ttu-id="9034d-102">Representa o plano de fundo de um objeto de intervalo.</span><span class="sxs-lookup"><span data-stu-id="9034d-102">Represents the background of a range object.</span></span>


## <a name="methods"></a><span data-ttu-id="9034d-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="9034d-103">Methods</span></span>

| <span data-ttu-id="9034d-104">Método</span><span class="sxs-lookup"><span data-stu-id="9034d-104">Method</span></span>           | <span data-ttu-id="9034d-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9034d-105">Return Type</span></span>    |<span data-ttu-id="9034d-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9034d-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9034d-107">Get RangeFill</span><span class="sxs-lookup"><span data-stu-id="9034d-107">Get RangeFill</span></span>](../api/rangefill_get.md) | [<span data-ttu-id="9034d-108">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="9034d-108">WorkbookRangeFill</span></span>](rangefill.md) |<span data-ttu-id="9034d-109">Leia as propriedades e os relacionamentos do objeto rangeFill.</span><span class="sxs-lookup"><span data-stu-id="9034d-109">Read properties and relationships of rangeFill object.</span></span>|
|[<span data-ttu-id="9034d-110">Update</span><span class="sxs-lookup"><span data-stu-id="9034d-110">Update</span></span>](../api/rangefill_update.md) | [<span data-ttu-id="9034d-111">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="9034d-111">WorkbookRangeFill</span></span>](rangefill.md)   |<span data-ttu-id="9034d-112">Atualize o objeto RangeFill.</span><span class="sxs-lookup"><span data-stu-id="9034d-112">Update RangeFill object.</span></span> |
|[<span data-ttu-id="9034d-113">Limpar</span><span class="sxs-lookup"><span data-stu-id="9034d-113">Clear</span></span>](../api/rangefill_clear.md)|<span data-ttu-id="9034d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9034d-114">None</span></span>|<span data-ttu-id="9034d-115">Redefine o plano de fundo do intervalo.</span><span class="sxs-lookup"><span data-stu-id="9034d-115">Resets the range background.</span></span>|

## <a name="properties"></a><span data-ttu-id="9034d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9034d-116">Properties</span></span>
| <span data-ttu-id="9034d-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9034d-117">Property</span></span>     | <span data-ttu-id="9034d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="9034d-118">Type</span></span>   |<span data-ttu-id="9034d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9034d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9034d-120">color</span><span class="sxs-lookup"><span data-stu-id="9034d-120">color</span></span>|<span data-ttu-id="9034d-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="9034d-121">string</span></span>|<span data-ttu-id="9034d-122">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="9034d-122">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="relationships"></a><span data-ttu-id="9034d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="9034d-123">Relationships</span></span>
<span data-ttu-id="9034d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9034d-124">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9034d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9034d-125">JSON representation</span></span>

<span data-ttu-id="9034d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9034d-126">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->