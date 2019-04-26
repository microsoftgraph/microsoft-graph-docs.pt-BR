---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 92235775143b3f8341724340e4ad301a40571adb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340872"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="85baa-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="85baa-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85baa-106">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="85baa-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="85baa-107">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="85baa-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="85baa-108">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="85baa-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="85baa-109">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="85baa-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="85baa-110">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="85baa-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="85baa-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="85baa-111">Methods</span></span>

| <span data-ttu-id="85baa-112">Método</span><span class="sxs-lookup"><span data-stu-id="85baa-112">Method</span></span>         | <span data-ttu-id="85baa-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85baa-113">Return Type</span></span> | <span data-ttu-id="85baa-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="85baa-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="85baa-115">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="85baa-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="85baa-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="85baa-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="85baa-117">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="85baa-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="85baa-118">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="85baa-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="85baa-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="85baa-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="85baa-120">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="85baa-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="85baa-121">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="85baa-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="85baa-122">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="85baa-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="85baa-123">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="85baa-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="85baa-124">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="85baa-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="85baa-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85baa-125">None</span></span> | <span data-ttu-id="85baa-126">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="85baa-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="85baa-127">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="85baa-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="85baa-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="85baa-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="85baa-129">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="85baa-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="85baa-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85baa-130">Properties</span></span>
| <span data-ttu-id="85baa-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85baa-131">Property</span></span>   | <span data-ttu-id="85baa-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="85baa-132">Type</span></span> |<span data-ttu-id="85baa-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="85baa-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85baa-134">id</span><span class="sxs-lookup"><span data-stu-id="85baa-134">id</span></span>|<span data-ttu-id="85baa-135">String</span><span class="sxs-lookup"><span data-stu-id="85baa-135">String</span></span>| <span data-ttu-id="85baa-136">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="85baa-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="85baa-137">Chave.</span><span class="sxs-lookup"><span data-stu-id="85baa-137">Key.</span></span> <span data-ttu-id="85baa-138">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="85baa-138">Not nullable.</span></span> <span data-ttu-id="85baa-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85baa-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85baa-140">Relações</span><span class="sxs-lookup"><span data-stu-id="85baa-140">Relationships</span></span>
| <span data-ttu-id="85baa-141">Relação</span><span class="sxs-lookup"><span data-stu-id="85baa-141">Relationship</span></span> | <span data-ttu-id="85baa-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="85baa-142">Type</span></span>   |<span data-ttu-id="85baa-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="85baa-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85baa-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="85baa-144">deleteditems</span></span>|<span data-ttu-id="85baa-145">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="85baa-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="85baa-146">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="85baa-146">Recently deleted items.</span></span> <span data-ttu-id="85baa-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85baa-147">Read-only.</span></span> <span data-ttu-id="85baa-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="85baa-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85baa-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85baa-149">JSON representation</span></span>
<span data-ttu-id="85baa-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85baa-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
