# <a name="nameditem-resource-type"></a><span data-ttu-id="c7a21-101">Tipo de recurso NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-101">NamedItem resource type</span></span>

<span data-ttu-id="c7a21-p101">Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p101">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="c7a21-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c7a21-105">Methods</span></span>

| <span data-ttu-id="c7a21-106">Método</span><span class="sxs-lookup"><span data-stu-id="c7a21-106">Method</span></span>           | <span data-ttu-id="c7a21-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c7a21-107">Return Type</span></span>    |<span data-ttu-id="c7a21-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a21-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c7a21-109">Add</span><span class="sxs-lookup"><span data-stu-id="c7a21-109">Add</span></span>](../api/nameditem_add.md)|[<span data-ttu-id="c7a21-110">NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-110">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="c7a21-111">Adiciona um novo nome à coleção do escopo fornecido.</span><span class="sxs-lookup"><span data-stu-id="c7a21-111">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="c7a21-112">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="c7a21-112">AddFormulaLocal</span></span>](../api/nameditem_addformulalocal.md)|[<span data-ttu-id="c7a21-113">NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-113">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="c7a21-114">Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.</span><span class="sxs-lookup"><span data-stu-id="c7a21-114">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="c7a21-115">Get NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-115">Get NamedItem</span></span>](../api/nameditem_get.md) | [<span data-ttu-id="c7a21-116">NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-116">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="c7a21-117">Leia as propriedades e os relacionamentos do objeto namedItem.</span><span class="sxs-lookup"><span data-stu-id="c7a21-117">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="c7a21-118">Update</span><span class="sxs-lookup"><span data-stu-id="c7a21-118">Update</span></span>](../api/nameditem_update.md) | [<span data-ttu-id="c7a21-119">NamedItem</span><span class="sxs-lookup"><span data-stu-id="c7a21-119">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="c7a21-120">Atualize o objeto NamedItem.</span><span class="sxs-lookup"><span data-stu-id="c7a21-120">Update NamedItem object.</span></span> |
|[<span data-ttu-id="c7a21-121">Range</span><span class="sxs-lookup"><span data-stu-id="c7a21-121">Range</span></span>](../api/nameditem_range.md)|[<span data-ttu-id="c7a21-122">Range</span><span class="sxs-lookup"><span data-stu-id="c7a21-122">Range</span></span>](range.md)|<span data-ttu-id="c7a21-p102">Retorna o objeto Range associado ao nome. Gera uma exceção se o tipo de item nomeado não for um intervalo.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p102">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="c7a21-125">List</span><span class="sxs-lookup"><span data-stu-id="c7a21-125">List</span></span>](../api/nameditem_list.md) | <span data-ttu-id="c7a21-126">Coleção [NamedItem](nameditem.md)</span><span class="sxs-lookup"><span data-stu-id="c7a21-126">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="c7a21-127">Obtenha uma coleção de objetos namedItem.</span><span class="sxs-lookup"><span data-stu-id="c7a21-127">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="c7a21-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7a21-128">Properties</span></span>
| <span data-ttu-id="c7a21-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7a21-129">Property</span></span>     | <span data-ttu-id="c7a21-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a21-130">Type</span></span>   |<span data-ttu-id="c7a21-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a21-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7a21-132">name</span><span class="sxs-lookup"><span data-stu-id="c7a21-132">name</span></span>|<span data-ttu-id="c7a21-133">string</span><span class="sxs-lookup"><span data-stu-id="c7a21-133">string</span></span>|<span data-ttu-id="c7a21-p103">O nome do objeto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p103">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="c7a21-136">comment</span><span class="sxs-lookup"><span data-stu-id="c7a21-136">comment</span></span>|<span data-ttu-id="c7a21-137">string</span><span class="sxs-lookup"><span data-stu-id="c7a21-137">string</span></span>|<span data-ttu-id="c7a21-138">Representa o comentário associado a esse nome.</span><span class="sxs-lookup"><span data-stu-id="c7a21-138">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="c7a21-139">scope</span><span class="sxs-lookup"><span data-stu-id="c7a21-139">scope</span></span>|<span data-ttu-id="c7a21-140">string</span><span class="sxs-lookup"><span data-stu-id="c7a21-140">string</span></span>|<span data-ttu-id="c7a21-p104">Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p104">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="c7a21-143">type</span><span class="sxs-lookup"><span data-stu-id="c7a21-143">type</span></span>|<span data-ttu-id="c7a21-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7a21-144">string</span></span>|<span data-ttu-id="c7a21-p105">Indica o tipo de referência associado ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean` e `Range`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p105">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="c7a21-148">value</span><span class="sxs-lookup"><span data-stu-id="c7a21-148">value</span></span>|<span data-ttu-id="c7a21-149">objeto</span><span class="sxs-lookup"><span data-stu-id="c7a21-149">object</span></span>|<span data-ttu-id="c7a21-p106">Representa a fórmula à qual o nome está definido para fazer referência. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p106">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="c7a21-153">visible</span><span class="sxs-lookup"><span data-stu-id="c7a21-153">visible</span></span>|<span data-ttu-id="c7a21-154">booliano</span><span class="sxs-lookup"><span data-stu-id="c7a21-154">boolean</span></span>|<span data-ttu-id="c7a21-155">Determina se o objeto fica visível ou não.</span><span class="sxs-lookup"><span data-stu-id="c7a21-155">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7a21-156">Relações</span><span class="sxs-lookup"><span data-stu-id="c7a21-156">Relationships</span></span>
| <span data-ttu-id="c7a21-157">Relação</span><span class="sxs-lookup"><span data-stu-id="c7a21-157">Relationship</span></span>     | <span data-ttu-id="c7a21-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7a21-158">Type</span></span>   |<span data-ttu-id="c7a21-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7a21-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c7a21-160">planilha</span><span class="sxs-lookup"><span data-stu-id="c7a21-160">worksheet</span></span>|[<span data-ttu-id="c7a21-161">worksheet</span><span class="sxs-lookup"><span data-stu-id="c7a21-161">worksheet</span></span>](worksheet.md)|<span data-ttu-id="c7a21-p107">Retorna a planilha em que o item nomeado está no escopo. Disponível somente se o item estiver com escopo de planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c7a21-p107">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c7a21-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7a21-165">JSON representation</span></span>

<span data-ttu-id="c7a21-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7a21-166">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.range"},
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
