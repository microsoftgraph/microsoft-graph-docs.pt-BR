# <a name="chartfont-resource-type"></a><span data-ttu-id="33eee-101">Tipo de recurso ChartFont</span><span class="sxs-lookup"><span data-stu-id="33eee-101">ChartFont resource type</span></span>

<span data-ttu-id="33eee-102">Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.</span><span class="sxs-lookup"><span data-stu-id="33eee-102">This object represents the font attributes (font name, font size, color, etc.) for a chart object.</span></span>


## <a name="methods"></a><span data-ttu-id="33eee-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="33eee-103">Methods</span></span>

| <span data-ttu-id="33eee-104">Método</span><span class="sxs-lookup"><span data-stu-id="33eee-104">Method</span></span>           | <span data-ttu-id="33eee-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33eee-105">Return Type</span></span>    |<span data-ttu-id="33eee-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="33eee-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33eee-107">Get ChartFont</span><span class="sxs-lookup"><span data-stu-id="33eee-107">Get ChartFont</span></span>](../api/chartfont_get.md) | [<span data-ttu-id="33eee-108">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="33eee-108">WorkbookChartFont</span></span>](chartfont.md) |<span data-ttu-id="33eee-109">Leia as propriedades e os relacionamentos do objeto chartFont.</span><span class="sxs-lookup"><span data-stu-id="33eee-109">Read properties and relationships of chartFont object.</span></span>|
|[<span data-ttu-id="33eee-110">Update</span><span class="sxs-lookup"><span data-stu-id="33eee-110">Update</span></span>](../api/chartfont_update.md) | [<span data-ttu-id="33eee-111">WorkbookChartFont</span><span class="sxs-lookup"><span data-stu-id="33eee-111">WorkbookChartFont</span></span>](chartfont.md)   |<span data-ttu-id="33eee-112">Atualize o objeto ChartFont.</span><span class="sxs-lookup"><span data-stu-id="33eee-112">Update ChartFont object.</span></span> |

## <a name="properties"></a><span data-ttu-id="33eee-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33eee-113">Properties</span></span>
| <span data-ttu-id="33eee-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33eee-114">Property</span></span>     | <span data-ttu-id="33eee-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="33eee-115">Type</span></span>   |<span data-ttu-id="33eee-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="33eee-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33eee-117">bold</span><span class="sxs-lookup"><span data-stu-id="33eee-117">bold</span></span>|<span data-ttu-id="33eee-118">booliano</span><span class="sxs-lookup"><span data-stu-id="33eee-118">boolean</span></span>|<span data-ttu-id="33eee-119">Representa o status da fonte em negrito.</span><span class="sxs-lookup"><span data-stu-id="33eee-119">Represents the bold status of font.</span></span>|
|<span data-ttu-id="33eee-120">color</span><span class="sxs-lookup"><span data-stu-id="33eee-120">color</span></span>|<span data-ttu-id="33eee-121">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="33eee-121">string</span></span>|<span data-ttu-id="33eee-p101">Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.</span><span class="sxs-lookup"><span data-stu-id="33eee-p101">HTML color code representation of the text color. E.g. #FF0000 represents Red.</span></span>|
|<span data-ttu-id="33eee-125">italic</span><span class="sxs-lookup"><span data-stu-id="33eee-125">italic</span></span>|<span data-ttu-id="33eee-126">booliano</span><span class="sxs-lookup"><span data-stu-id="33eee-126">boolean</span></span>|<span data-ttu-id="33eee-127">Representa o status da fonte em itálico.</span><span class="sxs-lookup"><span data-stu-id="33eee-127">Represents the italic status of the font.</span></span>|
|<span data-ttu-id="33eee-128">name</span><span class="sxs-lookup"><span data-stu-id="33eee-128">name</span></span>|<span data-ttu-id="33eee-129">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="33eee-129">string</span></span>|<span data-ttu-id="33eee-130">Nome da fonte (por exemplo, "Calibri")</span><span class="sxs-lookup"><span data-stu-id="33eee-130">Font name (e.g. "Calibri")</span></span>|
|<span data-ttu-id="33eee-131">size</span><span class="sxs-lookup"><span data-stu-id="33eee-131">size</span></span>|<span data-ttu-id="33eee-132">Double</span><span class="sxs-lookup"><span data-stu-id="33eee-132">double</span></span>|<span data-ttu-id="33eee-133">Tamanho da fonte, por exemplo, 11.</span><span class="sxs-lookup"><span data-stu-id="33eee-133">Size of the font (e.g. 11)</span></span>|
|<span data-ttu-id="33eee-134">underline</span><span class="sxs-lookup"><span data-stu-id="33eee-134">underline</span></span>|<span data-ttu-id="33eee-135">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="33eee-135">string</span></span>|<span data-ttu-id="33eee-136">Tipo de sublinhado aplicado à fonte.</span><span class="sxs-lookup"><span data-stu-id="33eee-136">Returns or sets the type of underline applied to the font.</span></span> <span data-ttu-id="33eee-137">Os valores possíveis são: `None`, `Single`.</span><span class="sxs-lookup"><span data-stu-id="33eee-137">The possible values are:</span></span>|

## <a name="relationships"></a><span data-ttu-id="33eee-138">Relações</span><span class="sxs-lookup"><span data-stu-id="33eee-138">Relationships</span></span>
<span data-ttu-id="33eee-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33eee-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="33eee-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33eee-140">JSON representation</span></span>

<span data-ttu-id="33eee-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33eee-141">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->