# <a name="tablerow-resource-type"></a><span data-ttu-id="be022-101">Tipo de recurso TableRow</span><span class="sxs-lookup"><span data-stu-id="be022-101">TableRow resource type</span></span>

<span data-ttu-id="be022-102">Representa uma linha em uma tabela.</span><span class="sxs-lookup"><span data-stu-id="be022-102">Represents a row in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="be022-103">Métodos</span><span class="sxs-lookup"><span data-stu-id="be022-103">Methods</span></span>

| <span data-ttu-id="be022-104">Método</span><span class="sxs-lookup"><span data-stu-id="be022-104">Method</span></span>           | <span data-ttu-id="be022-105">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="be022-105">Return Type</span></span>    |<span data-ttu-id="be022-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="be022-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be022-107">Get TableRow</span><span class="sxs-lookup"><span data-stu-id="be022-107">Get TableRow</span></span>](../api/tablerow_get.md) | [<span data-ttu-id="be022-108">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="be022-108">WorkbookTableRow</span></span>](tablerow.md) |<span data-ttu-id="be022-109">Leia as propriedades e os relacionamentos do objeto tableRow.</span><span class="sxs-lookup"><span data-stu-id="be022-109">Read properties and relationships of tableRow object.</span></span>|
|[<span data-ttu-id="be022-110">Atualizar</span><span class="sxs-lookup"><span data-stu-id="be022-110">Update</span></span>](../api/tablerow_update.md) | [<span data-ttu-id="be022-111">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="be022-111">WorkbookTableRow</span></span>](tablerow.md)  |<span data-ttu-id="be022-112">Atualize o objeto TableRow.</span><span class="sxs-lookup"><span data-stu-id="be022-112">Update TableRow object.</span></span> |
|[<span data-ttu-id="be022-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="be022-113">Range</span></span>](../api/tablerow_range.md)|[<span data-ttu-id="be022-114">Intervalo</span><span class="sxs-lookup"><span data-stu-id="be022-114">Range</span></span>](range.md)|<span data-ttu-id="be022-115">Retorna o objeto de intervalo associado a toda a linha.</span><span class="sxs-lookup"><span data-stu-id="be022-115">Returns the range object associated with the entire row.</span></span>|
|[<span data-ttu-id="be022-116">Excluir</span><span class="sxs-lookup"><span data-stu-id="be022-116">Delete</span></span>](../api/tablerow_delete.md)|<span data-ttu-id="be022-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be022-117">None</span></span>|<span data-ttu-id="be022-118">Exclui a linha da tabela.</span><span class="sxs-lookup"><span data-stu-id="be022-118">Deletes the row from the table.</span></span>|
|[<span data-ttu-id="be022-119">Lista</span><span class="sxs-lookup"><span data-stu-id="be022-119">List</span></span>](../api/tablerow_list.md) | <span data-ttu-id="be022-120">Coleção [WorkbookTableRow](tablerow.md)</span><span class="sxs-lookup"><span data-stu-id="be022-120">[WorkbookTableRow](tablerow.md) collection</span></span> |<span data-ttu-id="be022-121">Obtenha uma coleção de objetos tableRow.</span><span class="sxs-lookup"><span data-stu-id="be022-121">Get tableRow object collection.</span></span> |
|[<span data-ttu-id="be022-122">Itemat</span><span class="sxs-lookup"><span data-stu-id="be022-122">Itemat</span></span>](../api/tablerowcollection_itemat.md)|[<span data-ttu-id="be022-123">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="be022-123">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="be022-124">Obtém uma linha com base em sua posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="be022-124">Gets a row based on its position in the collection.</span></span>|
|[<span data-ttu-id="be022-125">Adicionar</span><span class="sxs-lookup"><span data-stu-id="be022-125">Add</span></span>](../api/tablerowcollection_add.md)|[<span data-ttu-id="be022-126">WorkbookTableRow</span><span class="sxs-lookup"><span data-stu-id="be022-126">WorkbookTableRow</span></span>](tablerow.md)|<span data-ttu-id="be022-127">Adiciona uma nova linha à tabela.</span><span class="sxs-lookup"><span data-stu-id="be022-127">Adds a new row to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="be022-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be022-128">Properties</span></span>
| <span data-ttu-id="be022-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be022-129">Property</span></span>     | <span data-ttu-id="be022-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="be022-130">Type</span></span>   |<span data-ttu-id="be022-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="be022-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be022-132">índice</span><span class="sxs-lookup"><span data-stu-id="be022-132">index</span></span>|<span data-ttu-id="be022-133">int</span><span class="sxs-lookup"><span data-stu-id="be022-133">int</span></span>|<span data-ttu-id="be022-p101">Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be022-p101">Returns the index number of the row within the rows collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="be022-137">values</span><span class="sxs-lookup"><span data-stu-id="be022-137">values</span></span>|<span data-ttu-id="be022-138">Json</span><span class="sxs-lookup"><span data-stu-id="be022-138">Json</span></span>|<span data-ttu-id="be022-p102">Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.</span><span class="sxs-lookup"><span data-stu-id="be022-p102">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be022-142">Relações</span><span class="sxs-lookup"><span data-stu-id="be022-142">Relationships</span></span>
<span data-ttu-id="be022-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be022-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="be022-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be022-144">JSON representation</span></span>

<span data-ttu-id="be022-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be022-145">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->