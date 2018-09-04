# <a name="rangeformat-resource-type"></a><span data-ttu-id="546cd-101">Tipo de recurso RangeFormat</span><span class="sxs-lookup"><span data-stu-id="546cd-101">RangeFormat resource type</span></span>

<span data-ttu-id="546cd-102">Um objeto de formatação que engloba a fonte, o preenchimento, as bordas, o alinhamento e outras propriedades do intervalo.</span><span class="sxs-lookup"><span data-stu-id="546cd-102">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="546cd-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="546cd-103">Methods</span></span>

| <span data-ttu-id="546cd-104">Método</span><span class="sxs-lookup"><span data-stu-id="546cd-104">Method</span></span>           | <span data-ttu-id="546cd-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="546cd-105">Return Type</span></span>    |<span data-ttu-id="546cd-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="546cd-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="546cd-107">Get RangeFormat</span><span class="sxs-lookup"><span data-stu-id="546cd-107">Get RangeFormat</span></span>](../api/rangeformat_get.md) | [<span data-ttu-id="546cd-108">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="546cd-108">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="546cd-109">Leia as propriedades e relacionamentos do objeto rangeFormat.</span><span class="sxs-lookup"><span data-stu-id="546cd-109">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="546cd-110">Criar RangeBorder</span><span class="sxs-lookup"><span data-stu-id="546cd-110">Create RangeBorder</span></span>](../api/rangeformat_post_borders.md) |[<span data-ttu-id="546cd-111">WorkbookRangeBorder</span><span class="sxs-lookup"><span data-stu-id="546cd-111">WorkbookRangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="546cd-112">Crie uma nova RangeBorder postando na coleção de bordas.</span><span class="sxs-lookup"><span data-stu-id="546cd-112">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="546cd-113">Bordas de lista</span><span class="sxs-lookup"><span data-stu-id="546cd-113">List borders</span></span>](../api/rangeformat_list_borders.md) |<span data-ttu-id="546cd-114">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="546cd-114">[WorkbookRangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="546cd-115">Obtenha uma coleção de objetos RangeBorder.</span><span class="sxs-lookup"><span data-stu-id="546cd-115">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="546cd-116">Atualizar</span><span class="sxs-lookup"><span data-stu-id="546cd-116">Update</span></span>](../api/rangeformat_update.md) | [<span data-ttu-id="546cd-117">WorkbookRangeFormat</span><span class="sxs-lookup"><span data-stu-id="546cd-117">WorkbookRangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="546cd-118">Atualize o objeto RangeFormat.</span><span class="sxs-lookup"><span data-stu-id="546cd-118">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="546cd-119">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="546cd-119">Autofitcolumns</span></span>](../api/rangeformat_autofitcolumns.md)|<span data-ttu-id="546cd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="546cd-120">None</span></span>|<span data-ttu-id="546cd-121">Altera a largura das colunas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="546cd-121">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="546cd-122">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="546cd-122">Autofitrows</span></span>](../api/rangeformat_autofitrows.md)|<span data-ttu-id="546cd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="546cd-123">None</span></span>|<span data-ttu-id="546cd-124">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="546cd-124">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="546cd-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="546cd-125">Properties</span></span>
| <span data-ttu-id="546cd-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="546cd-126">Property</span></span>     | <span data-ttu-id="546cd-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="546cd-127">Type</span></span>   |<span data-ttu-id="546cd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="546cd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="546cd-129">columnWidth</span><span class="sxs-lookup"><span data-stu-id="546cd-129">columnWidth</span></span>|<span data-ttu-id="546cd-130">double</span><span class="sxs-lookup"><span data-stu-id="546cd-130">double</span></span>|<span data-ttu-id="546cd-p101">Obtém ou define a largura de todas as colunas dentro do intervalo. Se as larguras das colunas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="546cd-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="546cd-133">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="546cd-133">horizontalAlignment</span></span>|<span data-ttu-id="546cd-134">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="546cd-134">string</span></span>|<span data-ttu-id="546cd-135">Representa o alinhamento horizontal do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="546cd-135">Returns or sets the horizontal alignment for the specified object.</span></span> <span data-ttu-id="546cd-136">Os valores possíveis são: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="546cd-136">The possible values are `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`, , , , or .</span></span>|
|<span data-ttu-id="546cd-137">rowHeight</span><span class="sxs-lookup"><span data-stu-id="546cd-137">rowHeight</span></span>|<span data-ttu-id="546cd-138">double</span><span class="sxs-lookup"><span data-stu-id="546cd-138">double</span></span>|<span data-ttu-id="546cd-p103">Obtém ou define a altura de todas as linhas do intervalo. Se as alturas das linhas não forem uniformes, será retornado null.</span><span class="sxs-lookup"><span data-stu-id="546cd-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="546cd-141">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="546cd-141">verticalAlignment</span></span>|<span data-ttu-id="546cd-142">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="546cd-142">string</span></span>|<span data-ttu-id="546cd-143">Representa o alinhamento vertical do objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="546cd-143">Represents the vertical alignment for the specified object. Possible values are: , , , , .</span></span> <span data-ttu-id="546cd-144">Os valores possíveis são: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="546cd-144">The possible values are `Top`, `Center`, `Bottom`, `Justify`, `Distributed`, , , , , , , or .</span></span>|
|<span data-ttu-id="546cd-145">wrapText</span><span class="sxs-lookup"><span data-stu-id="546cd-145">wrapText</span></span>|<span data-ttu-id="546cd-146">booliano</span><span class="sxs-lookup"><span data-stu-id="546cd-146">boolean</span></span>|<span data-ttu-id="546cd-p105">Indica se o Excel quebra automaticamente a linha de texto no objeto. Um valor nulo indica que o intervalo inteiro não tem configuração de quebra de linha automática uniforme.</span><span class="sxs-lookup"><span data-stu-id="546cd-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="546cd-149">Relações</span><span class="sxs-lookup"><span data-stu-id="546cd-149">Relationships</span></span>
| <span data-ttu-id="546cd-150">Relação</span><span class="sxs-lookup"><span data-stu-id="546cd-150">Relationship</span></span> | <span data-ttu-id="546cd-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="546cd-151">Type</span></span>   |<span data-ttu-id="546cd-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="546cd-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="546cd-153">bordas</span><span class="sxs-lookup"><span data-stu-id="546cd-153">borders</span></span>|<span data-ttu-id="546cd-154">Coleção [WorkbookRangeBorder](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="546cd-154">[WorkbookRangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="546cd-155">Coleção de objetos de borda que se aplicam a todo o intervalo selecionado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="546cd-155">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="546cd-156">preencher</span><span class="sxs-lookup"><span data-stu-id="546cd-156">fill</span></span>|[<span data-ttu-id="546cd-157">WorkbookRangeFill</span><span class="sxs-lookup"><span data-stu-id="546cd-157">WorkbookRangeFill</span></span>](rangefill.md)|<span data-ttu-id="546cd-p106">Retorna o objeto de preenchimento definido em todo o intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="546cd-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="546cd-160">fonte</span><span class="sxs-lookup"><span data-stu-id="546cd-160">font</span></span>|[<span data-ttu-id="546cd-161">WorkbookRangeFont</span><span class="sxs-lookup"><span data-stu-id="546cd-161">WorkbookRangeFont</span></span>](rangefont.md)|<span data-ttu-id="546cd-162">Retorna o objeto fonte definido em todo o intervalo selecionado somente leitura.</span><span class="sxs-lookup"><span data-stu-id="546cd-162">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="546cd-163">proteção</span><span class="sxs-lookup"><span data-stu-id="546cd-163">protection</span></span>|[<span data-ttu-id="546cd-164">WorkbookFormatProtection</span><span class="sxs-lookup"><span data-stu-id="546cd-164">WorkbookFormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="546cd-p107">Retorna o objeto de proteção de formato para um intervalo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="546cd-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="546cd-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="546cd-167">JSON representation</span></span>

<span data-ttu-id="546cd-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="546cd-168">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->