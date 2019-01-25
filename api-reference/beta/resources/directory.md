---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 22c5b959f87b6178fa406bc4fd5d00ad52e5cf55
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517481"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="a827a-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="a827a-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a827a-106">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="a827a-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="a827a-107">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="a827a-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="a827a-108">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="a827a-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="a827a-109">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="a827a-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="a827a-110">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a827a-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a827a-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="a827a-111">Methods</span></span>

| <span data-ttu-id="a827a-112">Método</span><span class="sxs-lookup"><span data-stu-id="a827a-112">Method</span></span>         | <span data-ttu-id="a827a-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a827a-113">Return Type</span></span> | <span data-ttu-id="a827a-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="a827a-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="a827a-115">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="a827a-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="a827a-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a827a-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="a827a-117">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="a827a-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="a827a-118">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="a827a-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="a827a-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a827a-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a827a-120">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="a827a-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="a827a-121">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="a827a-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="a827a-122">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a827a-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a827a-123">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="a827a-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="a827a-124">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="a827a-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="a827a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a827a-125">None</span></span> | <span data-ttu-id="a827a-126">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="a827a-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="a827a-127">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="a827a-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="a827a-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a827a-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a827a-129">Lista os itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="a827a-129">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="a827a-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a827a-130">Properties</span></span>
| <span data-ttu-id="a827a-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a827a-131">Property</span></span>   | <span data-ttu-id="a827a-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a827a-132">Type</span></span> |<span data-ttu-id="a827a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a827a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a827a-134">id</span><span class="sxs-lookup"><span data-stu-id="a827a-134">id</span></span>|<span data-ttu-id="a827a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a827a-135">String</span></span>| <span data-ttu-id="a827a-136">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="a827a-136">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="a827a-137">Chave.</span><span class="sxs-lookup"><span data-stu-id="a827a-137">Key.</span></span> <span data-ttu-id="a827a-138">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="a827a-138">Not nullable.</span></span> <span data-ttu-id="a827a-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a827a-139">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a827a-140">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="a827a-140">Relationships</span></span>
| <span data-ttu-id="a827a-141">Relação</span><span class="sxs-lookup"><span data-stu-id="a827a-141">Relationship</span></span> | <span data-ttu-id="a827a-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="a827a-142">Type</span></span>   |<span data-ttu-id="a827a-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a827a-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a827a-144">deleteditems</span><span class="sxs-lookup"><span data-stu-id="a827a-144">deleteditems</span></span>|<span data-ttu-id="a827a-145">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a827a-145">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a827a-146">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="a827a-146">Recently deleted items.</span></span> <span data-ttu-id="a827a-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a827a-147">Read-only.</span></span> <span data-ttu-id="a827a-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a827a-148">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a827a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a827a-149">JSON representation</span></span>
<span data-ttu-id="a827a-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a827a-150">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
