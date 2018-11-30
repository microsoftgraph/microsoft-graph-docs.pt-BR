---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
ms.openlocfilehash: e83ace1a50998b6645e059fe0f63e3922497c1cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006493"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="be396-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="be396-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="be396-106">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="be396-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="be396-107">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="be396-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="be396-108">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="be396-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="be396-109">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="be396-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="be396-110">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="be396-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="be396-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="be396-111">Methods</span></span>

| <span data-ttu-id="be396-112">Método</span><span class="sxs-lookup"><span data-stu-id="be396-112">Method</span></span>         | <span data-ttu-id="be396-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="be396-113">Return Type</span></span> | <span data-ttu-id="be396-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="be396-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="be396-115">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="be396-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="be396-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="be396-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="be396-117">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="be396-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="be396-118">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="be396-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="be396-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="be396-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="be396-120">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="be396-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="be396-121">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="be396-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="be396-122">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="be396-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="be396-123">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="be396-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="be396-124">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="be396-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="be396-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be396-125">None</span></span> | <span data-ttu-id="be396-126">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="be396-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="be396-127">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="be396-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="be396-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="be396-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="be396-129">Lista os itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="be396-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="be396-130">Relações</span><span class="sxs-lookup"><span data-stu-id="be396-130">Relationships</span></span>
| <span data-ttu-id="be396-131">Relação</span><span class="sxs-lookup"><span data-stu-id="be396-131">Relationship</span></span> | <span data-ttu-id="be396-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="be396-132">Type</span></span>   |<span data-ttu-id="be396-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="be396-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be396-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="be396-134">deletedItems</span></span>|<span data-ttu-id="be396-135">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="be396-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="be396-136">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="be396-136">Recently deleted items.</span></span> <span data-ttu-id="be396-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be396-137">Read-only.</span></span> <span data-ttu-id="be396-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="be396-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be396-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be396-139">JSON representation</span></span>
<span data-ttu-id="be396-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="be396-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="be396-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be396-141">Example</span></span>

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