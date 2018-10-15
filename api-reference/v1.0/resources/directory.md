# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="c718e-101">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="c718e-101">directory resource type (deleted items)</span></span>

<span data-ttu-id="c718e-102">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="c718e-102">Represents a deleted item in the directory.</span></span> <span data-ttu-id="c718e-103">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="c718e-103">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="c718e-104">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="c718e-104">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="c718e-105">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="c718e-105">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="c718e-106">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="c718e-106">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c718e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c718e-107">Methods</span></span>

| <span data-ttu-id="c718e-108">Método</span><span class="sxs-lookup"><span data-stu-id="c718e-108">Method</span></span>         | <span data-ttu-id="c718e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c718e-109">Return Type</span></span> | <span data-ttu-id="c718e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c718e-110">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="c718e-111">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="c718e-111">Get deleted item</span></span>](../api/directory_deleteditems_get.md) | [<span data-ttu-id="c718e-112">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c718e-112">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="c718e-113">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="c718e-113">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="c718e-114">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="c718e-114">Restore deleted item</span></span>](../api/directory_deleteditems_restore.md) |[<span data-ttu-id="c718e-115">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c718e-115">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="c718e-116">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="c718e-116">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="c718e-117">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="c718e-117">List deleted items</span></span>](../api/directory_deleteditems_list.md) |<span data-ttu-id="c718e-118">coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c718e-118">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c718e-119">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="c718e-119">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="c718e-120">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="c718e-120">Permanently delete an item</span></span>](../api/directory_deleteditems_delete.md) | <span data-ttu-id="c718e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c718e-121">None</span></span> | <span data-ttu-id="c718e-122">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="c718e-122">Permanently deletes an item.</span></span> |
|<span data-ttu-id="c718e-123">[Lista itens excluídos pertencentes a um usuário](../api/directory_deleteditems_user_owned.md)</span><span class="sxs-lookup"><span data-stu-id="c718e-123">Added [List deleted items owned by a user](../api/directory_deleteditems_user_owned.md) action to directory (deleted items) resource</span></span> | <span data-ttu-id="c718e-124">coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c718e-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="c718e-125">Lista os itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="c718e-125">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c718e-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c718e-126">Relationships</span></span>
| <span data-ttu-id="c718e-127">Relação</span><span class="sxs-lookup"><span data-stu-id="c718e-127">Relationship</span></span> | <span data-ttu-id="c718e-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="c718e-128">Type</span></span>   |<span data-ttu-id="c718e-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="c718e-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c718e-130">deleteditems</span><span class="sxs-lookup"><span data-stu-id="c718e-130">deleteditems</span></span>|<span data-ttu-id="c718e-131">coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c718e-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c718e-132">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="c718e-132">Recently deleted items.</span></span> <span data-ttu-id="c718e-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c718e-133">Read-only.</span></span> <span data-ttu-id="c718e-134">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c718e-134">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c718e-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c718e-135">JSON representation</span></span>
<span data-ttu-id="c718e-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c718e-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="c718e-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c718e-137">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
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