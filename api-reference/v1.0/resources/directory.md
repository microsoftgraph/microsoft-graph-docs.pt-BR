---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 17939db5752c114c5c9180d318725c2553b4f1d7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531667"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="e6b80-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="e6b80-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="e6b80-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6b80-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6b80-107">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="e6b80-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="e6b80-108">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e6b80-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="e6b80-109">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="e6b80-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="e6b80-110">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="e6b80-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="e6b80-111">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](application.md), [grupo](group.md) e recursos do [usuário](user.md) .</span><span class="sxs-lookup"><span data-stu-id="e6b80-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="e6b80-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="e6b80-112">Methods</span></span>

| <span data-ttu-id="e6b80-113">Método</span><span class="sxs-lookup"><span data-stu-id="e6b80-113">Method</span></span>         | <span data-ttu-id="e6b80-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6b80-114">Return Type</span></span> | <span data-ttu-id="e6b80-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6b80-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="e6b80-116">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="e6b80-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="e6b80-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e6b80-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="e6b80-118">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="e6b80-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="e6b80-119">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="e6b80-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="e6b80-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e6b80-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="e6b80-121">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="e6b80-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="e6b80-122">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="e6b80-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="e6b80-123">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e6b80-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e6b80-124">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="e6b80-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="e6b80-125">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="e6b80-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="e6b80-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6b80-126">None</span></span> | <span data-ttu-id="e6b80-127">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="e6b80-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="e6b80-128">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="e6b80-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="e6b80-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e6b80-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="e6b80-130">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="e6b80-130">Lists directory items owned by a user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6b80-131">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="e6b80-131">Relationships</span></span>
| <span data-ttu-id="e6b80-132">Relação</span><span class="sxs-lookup"><span data-stu-id="e6b80-132">Relationship</span></span> | <span data-ttu-id="e6b80-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6b80-133">Type</span></span>   |<span data-ttu-id="e6b80-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6b80-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6b80-135">deletedItems</span><span class="sxs-lookup"><span data-stu-id="e6b80-135">deletedItems</span></span>|<span data-ttu-id="e6b80-136">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="e6b80-136">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="e6b80-137">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="e6b80-137">Recently deleted items.</span></span> <span data-ttu-id="e6b80-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6b80-138">Read-only.</span></span> <span data-ttu-id="e6b80-139">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e6b80-139">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6b80-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6b80-140">JSON representation</span></span>
<span data-ttu-id="e6b80-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6b80-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="e6b80-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6b80-142">Example</span></span>

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
