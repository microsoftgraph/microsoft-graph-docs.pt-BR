# <a name="rangefont-resource-type"></a><span data-ttu-id="29fd8-101">Tipo de recurso RangeFont</span><span class="sxs-lookup"><span data-stu-id="29fd8-101">RangeFont resource type</span></span>

<span data-ttu-id="29fd8-102">Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.</span><span class="sxs-lookup"><span data-stu-id="29fd8-102">This object represents the font attributes (font name, font size, color, etc.) for an object.</span></span>


## <a name="methods"></a><span data-ttu-id="29fd8-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="29fd8-103">Methods</span></span>

| <span data-ttu-id="29fd8-104">Método</span><span class="sxs-lookup"><span data-stu-id="29fd8-104">Method</span></span>           | <span data-ttu-id="29fd8-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29fd8-105">Return Type</span></span>    |<span data-ttu-id="29fd8-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fd8-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29fd8-107">Get RangeFont</span><span class="sxs-lookup"><span data-stu-id="29fd8-107">Get RangeFont</span></span>](../api/rangefont_get.md) | [<span data-ttu-id="29fd8-108">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="29fd8-108">WorkbookRangeFont</span></span>](rangefont.md) |<span data-ttu-id="29fd8-109">Leia as propriedades e os relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="29fd8-109">Read properties and relationships of rangeFont object.</span></span>|
|[<span data-ttu-id="29fd8-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="29fd8-110">Update</span></span>](../api/rangefont_update.md) | [<span data-ttu-id="29fd8-111">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="29fd8-111">WorkbookRangeFont</span></span>](rangefont.md)   |<span data-ttu-id="29fd8-112">Atualize o objeto RangeFont.</span><span class="sxs-lookup"><span data-stu-id="29fd8-112">Update RangeFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29fd8-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29fd8-113">Properties</span></span>
| <span data-ttu-id="29fd8-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29fd8-114">Property</span></span>     | <span data-ttu-id="29fd8-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="29fd8-115">Type</span></span>   |<span data-ttu-id="29fd8-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="29fd8-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29fd8-117">negrito</span><span class="sxs-lookup"><span data-stu-id="29fd8-117">bold</span></span>|<span data-ttu-id="29fd8-118">booliano</span><span class="sxs-lookup"><span data-stu-id="29fd8-118">boolean</span></span>|<span data-ttu-id="29fd8-119">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="29fd8-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="29fd8-120">cor</span><span class="sxs-lookup"><span data-stu-id="29fd8-120">color</span></span>|<span data-ttu-id="29fd8-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="29fd8-121">string</span></span>|<span data-ttu-id="29fd8-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="29fd8-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="29fd8-125">italico</span><span class="sxs-lookup"><span data-stu-id="29fd8-125">italic</span></span>|<span data-ttu-id="29fd8-126">booliano</span><span class="sxs-lookup"><span data-stu-id="29fd8-126">boolean</span></span>|<span data-ttu-id="29fd8-127">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="29fd8-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="29fd8-128">nome</span><span class="sxs-lookup"><span data-stu-id="29fd8-128">name</span></span>|<span data-ttu-id="29fd8-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="29fd8-129">string</span></span>|<span data-ttu-id="29fd8-130">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="29fd8-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="29fd8-131">dimensionar</span><span class="sxs-lookup"><span data-stu-id="29fd8-131">size</span></span>|<span data-ttu-id="29fd8-132">Double</span><span class="sxs-lookup"><span data-stu-id="29fd8-132">double</span></span>|<span data-ttu-id="29fd8-133">Font Size</span><span class="sxs-lookup"><span data-stu-id="29fd8-133">Font size.</span></span>|
|<span data-ttu-id="29fd8-134">underline</span><span class="sxs-lookup"><span data-stu-id="29fd8-134">underline</span></span>|<span data-ttu-id="29fd8-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="29fd8-135">string</span></span>|<span data-ttu-id="29fd8-136">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="29fd8-136">Returns or sets the type of underline applied to the font.</span></span> <span data-ttu-id="29fd8-137">Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.</span><span class="sxs-lookup"><span data-stu-id="29fd8-137">The possible values are `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`, , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="29fd8-138">Relações</span><span class="sxs-lookup"><span data-stu-id="29fd8-138">Relationships</span></span>
<span data-ttu-id="29fd8-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29fd8-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29fd8-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29fd8-140">JSON representation</span></span>

<span data-ttu-id="29fd8-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29fd8-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->