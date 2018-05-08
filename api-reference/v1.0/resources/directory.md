# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="4c258-101">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="4c258-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="4c258-102">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="4c258-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="4c258-103">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4c258-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="4c258-104">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="4c258-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="4c258-105">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="4c258-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="4c258-106">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4c258-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4c258-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4c258-107">Methods</span></span>

| <span data-ttu-id="4c258-108">Método</span><span class="sxs-lookup"><span data-stu-id="4c258-108">Method</span></span>         | <span data-ttu-id="4c258-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4c258-109">Return Type</span></span> | <span data-ttu-id="4c258-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c258-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="4c258-111">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="4c258-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="4c258-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4c258-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="4c258-113">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="4c258-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="4c258-114">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="4c258-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="4c258-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4c258-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="4c258-116">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="4c258-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="4c258-117">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="4c258-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="4c258-118">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4c258-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4c258-119">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="4c258-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="4c258-120">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="4c258-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="4c258-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c258-121">None</span></span> | <span data-ttu-id="4c258-122">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="4c258-122">Permanently deletes an item.</span></span> |

## <a name="properties"></a><span data-ttu-id="4c258-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c258-123">Properties</span></span>
| <span data-ttu-id="4c258-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c258-124">Property</span></span>   | <span data-ttu-id="4c258-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c258-125">Type</span></span> |<span data-ttu-id="4c258-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c258-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c258-127">id</span><span class="sxs-lookup"><span data-stu-id="4c258-127">id</span></span>|<span data-ttu-id="4c258-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c258-128">String</span></span>| <span data-ttu-id="4c258-129">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="4c258-129">A Guid that is the unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde. Key. Not nullable. Read-only.</span></span> <span data-ttu-id="4c258-130">Chave.</span><span class="sxs-lookup"><span data-stu-id="4c258-130">Key</span></span> <span data-ttu-id="4c258-131">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="4c258-131">Not nullable.</span></span> <span data-ttu-id="4c258-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c258-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c258-133">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="4c258-133">Relationships</span></span>
| <span data-ttu-id="4c258-134">Relação</span><span class="sxs-lookup"><span data-stu-id="4c258-134">Relationship</span></span> | <span data-ttu-id="4c258-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c258-135">Type</span></span>   |<span data-ttu-id="4c258-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c258-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c258-137">deleteditems</span><span class="sxs-lookup"><span data-stu-id="4c258-137">deleteditems</span></span>|<span data-ttu-id="4c258-138">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4c258-138">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4c258-139">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="4c258-139">Recently deleted items.</span></span> <span data-ttu-id="4c258-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4c258-140">Read-only.</span></span> <span data-ttu-id="4c258-141">Anulável.</span><span class="sxs-lookup"><span data-stu-id="4c258-141">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4c258-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c258-142">JSON representation</span></span>
<span data-ttu-id="4c258-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c258-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->