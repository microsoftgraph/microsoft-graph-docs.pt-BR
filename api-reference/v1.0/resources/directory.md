---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09f6059ca10b64e30aab06f4dd9ee4f3dc281ef4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34658033"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="50fa1-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="50fa1-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="50fa1-106">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="50fa1-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="50fa1-107">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="50fa1-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="50fa1-108">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="50fa1-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="50fa1-109">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="50fa1-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="50fa1-110">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="50fa1-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="50fa1-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="50fa1-111">Methods</span></span>

| <span data-ttu-id="50fa1-112">Método</span><span class="sxs-lookup"><span data-stu-id="50fa1-112">Method</span></span>         | <span data-ttu-id="50fa1-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50fa1-113">Return Type</span></span> | <span data-ttu-id="50fa1-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="50fa1-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="50fa1-115">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="50fa1-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="50fa1-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50fa1-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="50fa1-117">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="50fa1-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="50fa1-118">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="50fa1-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="50fa1-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="50fa1-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="50fa1-120">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="50fa1-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="50fa1-121">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="50fa1-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="50fa1-122">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="50fa1-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50fa1-123">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="50fa1-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="50fa1-124">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="50fa1-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="50fa1-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50fa1-125">None</span></span> | <span data-ttu-id="50fa1-126">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="50fa1-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="50fa1-127">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="50fa1-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="50fa1-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="50fa1-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="50fa1-129">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="50fa1-129">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="50fa1-130">Relações</span><span class="sxs-lookup"><span data-stu-id="50fa1-130">Relationships</span></span>
| <span data-ttu-id="50fa1-131">Relação</span><span class="sxs-lookup"><span data-stu-id="50fa1-131">Relationship</span></span> | <span data-ttu-id="50fa1-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="50fa1-132">Type</span></span>   |<span data-ttu-id="50fa1-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="50fa1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50fa1-134">deletedItems</span><span class="sxs-lookup"><span data-stu-id="50fa1-134">deletedItems</span></span>|<span data-ttu-id="50fa1-135">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="50fa1-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="50fa1-136">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="50fa1-136">Recently deleted items.</span></span> <span data-ttu-id="50fa1-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50fa1-137">Read-only.</span></span> <span data-ttu-id="50fa1-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="50fa1-138">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50fa1-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50fa1-139">JSON representation</span></span>
<span data-ttu-id="50fa1-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50fa1-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="50fa1-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50fa1-141">Example</span></span>

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
