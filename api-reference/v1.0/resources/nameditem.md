# <a name="nameditem-resource-type"></a><span data-ttu-id="3826a-101">Tipo de recurso NamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-101">NamedItem resource type</span></span>

<span data-ttu-id="3826a-p101">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="3826a-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="3826a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="3826a-105">Methods</span></span>

| <span data-ttu-id="3826a-106">Método</span><span class="sxs-lookup"><span data-stu-id="3826a-106">Method</span></span>           | <span data-ttu-id="3826a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3826a-107">Return Type</span></span>    |<span data-ttu-id="3826a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3826a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3826a-109">Add</span><span class="sxs-lookup"><span data-stu-id="3826a-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="3826a-110">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-110">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="3826a-111">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="3826a-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="3826a-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="3826a-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="3826a-113">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-113">WorkbookNamedItem</span></span>](nameditem.md)|<span data-ttu-id="3826a-114">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="3826a-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="3826a-115">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="3826a-116">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-116">WorkbookNamedItem</span></span>](nameditem.md) |<span data-ttu-id="3826a-117">Propriedades de leitura e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="3826a-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="3826a-118">Update</span><span class="sxs-lookup"><span data-stu-id="3826a-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="3826a-119">WorkbookNamedItem</span><span class="sxs-lookup"><span data-stu-id="3826a-119">WorkbookNamedItem</span></span>](nameditem.md)   |<span data-ttu-id="3826a-120">Atualiza o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="3826a-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="3826a-121">Range</span><span class="sxs-lookup"><span data-stu-id="3826a-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="3826a-122">Range</span><span class="sxs-lookup"><span data-stu-id="3826a-122">Range</span></span>](range.md)|<span data-ttu-id="3826a-p102">Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.</span><span class="sxs-lookup"><span data-stu-id="3826a-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="3826a-125">List</span><span class="sxs-lookup"><span data-stu-id="3826a-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="3826a-126">Coleção [WorkbookNamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="3826a-126">[WorkbookNamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="3826a-127">Obtém uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="3826a-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="3826a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3826a-128">Properties</span></span>
| <span data-ttu-id="3826a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3826a-129">Property</span></span>     | <span data-ttu-id="3826a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3826a-130">Type</span></span>   |<span data-ttu-id="3826a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3826a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3826a-132">name</span><span class="sxs-lookup"><span data-stu-id="3826a-132">name</span></span>|<span data-ttu-id="3826a-133">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3826a-133">string</span></span>|<span data-ttu-id="3826a-p103">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3826a-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="3826a-136">comment</span><span class="sxs-lookup"><span data-stu-id="3826a-136">comment</span></span>|<span data-ttu-id="3826a-137">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3826a-137">string</span></span>|<span data-ttu-id="3826a-138">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="3826a-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="3826a-139">scope</span><span class="sxs-lookup"><span data-stu-id="3826a-139">scope</span></span>|<span data-ttu-id="3826a-140">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3826a-140">string</span></span>|<span data-ttu-id="3826a-p104">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3826a-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="3826a-143">type</span><span class="sxs-lookup"><span data-stu-id="3826a-143">type</span></span>|<span data-ttu-id="3826a-144">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="3826a-144">string</span></span>|<span data-ttu-id="3826a-145">Indica o tipo de referência associada ao nome.</span><span class="sxs-lookup"><span data-stu-id="3826a-145">Indicates what type of reference is associated with the name. Possible values are: , , , , . Read-only.</span></span> <span data-ttu-id="3826a-146">Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean`, `Range`.</span><span class="sxs-lookup"><span data-stu-id="3826a-146">The possible values are `String`, `Integer`, `Double`, `Boolean`, `Range`, , , , , , , or .</span></span> <span data-ttu-id="3826a-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3826a-147">Read-only.</span></span>|
|<span data-ttu-id="3826a-148">value</span><span class="sxs-lookup"><span data-stu-id="3826a-148">value</span></span>|<span data-ttu-id="3826a-149">Json</span><span class="sxs-lookup"><span data-stu-id="3826a-149">Json</span></span>|<span data-ttu-id="3826a-p106">Representa a fórmula definida como referência para o nome. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3826a-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="3826a-153">visible</span><span class="sxs-lookup"><span data-stu-id="3826a-153">visible</span></span>|<span data-ttu-id="3826a-154">booliano</span><span class="sxs-lookup"><span data-stu-id="3826a-154">boolean</span></span>|<span data-ttu-id="3826a-155">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="3826a-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3826a-156">Relações</span><span class="sxs-lookup"><span data-stu-id="3826a-156">Relationships</span></span>
| <span data-ttu-id="3826a-157">Relação</span><span class="sxs-lookup"><span data-stu-id="3826a-157">Relationship</span></span>     | <span data-ttu-id="3826a-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="3826a-158">Type</span></span>   |<span data-ttu-id="3826a-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="3826a-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3826a-160">worksheet</span><span class="sxs-lookup"><span data-stu-id="3826a-160">worksheet</span></span>|[<span data-ttu-id="3826a-161">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="3826a-161">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="3826a-p107">Retorna a planilha do escopo do item nomeado. Disponível somente se o item estiver no escopo da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3826a-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3826a-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3826a-165">JSON representation</span></span>

<span data-ttu-id="3826a-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3826a-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
