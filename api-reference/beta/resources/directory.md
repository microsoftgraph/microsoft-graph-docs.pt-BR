---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
ms.openlocfilehash: 20685f2d9d61726d170744efb5fd2abb571fe934
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834444"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="46cad-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="46cad-105">directory resource type (deleted items)</span></span>

> <span data-ttu-id="46cad-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="46cad-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46cad-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="46cad-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46cad-108">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="46cad-108">Represents a deleted item in the directory.</span></span> <span data-ttu-id="46cad-109">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="46cad-109">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="46cad-110">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="46cad-110">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="46cad-111">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="46cad-111">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="46cad-112">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="46cad-112">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="46cad-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="46cad-113">Methods</span></span>

| <span data-ttu-id="46cad-114">Método</span><span class="sxs-lookup"><span data-stu-id="46cad-114">Method</span></span>         | <span data-ttu-id="46cad-115">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46cad-115">Return Type</span></span> | <span data-ttu-id="46cad-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="46cad-116">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="46cad-117">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="46cad-117">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="46cad-118">directoryObject</span><span class="sxs-lookup"><span data-stu-id="46cad-118">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="46cad-119">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="46cad-119">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="46cad-120">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="46cad-120">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="46cad-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="46cad-121">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="46cad-122">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="46cad-122">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="46cad-123">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="46cad-123">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="46cad-124">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="46cad-124">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="46cad-125">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="46cad-125">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="46cad-126">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="46cad-126">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="46cad-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46cad-127">None</span></span> | <span data-ttu-id="46cad-128">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="46cad-128">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="46cad-129">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="46cad-129">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="46cad-130">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="46cad-130">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="46cad-131">Lista os itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="46cad-131">Lists directory items owned by a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="46cad-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46cad-132">Properties</span></span>
| <span data-ttu-id="46cad-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46cad-133">Property</span></span>   | <span data-ttu-id="46cad-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="46cad-134">Type</span></span> |<span data-ttu-id="46cad-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="46cad-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46cad-136">id</span><span class="sxs-lookup"><span data-stu-id="46cad-136">id</span></span>|<span data-ttu-id="46cad-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46cad-137">String</span></span>| <span data-ttu-id="46cad-138">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="46cad-138">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="46cad-139">Chave.</span><span class="sxs-lookup"><span data-stu-id="46cad-139">Key.</span></span> <span data-ttu-id="46cad-140">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="46cad-140">Not nullable.</span></span> <span data-ttu-id="46cad-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46cad-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46cad-142">Relações</span><span class="sxs-lookup"><span data-stu-id="46cad-142">Relationships</span></span>
| <span data-ttu-id="46cad-143">Relação</span><span class="sxs-lookup"><span data-stu-id="46cad-143">Relationship</span></span> | <span data-ttu-id="46cad-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="46cad-144">Type</span></span>   |<span data-ttu-id="46cad-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="46cad-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46cad-146">deleteditems</span><span class="sxs-lookup"><span data-stu-id="46cad-146">deleteditems</span></span>|<span data-ttu-id="46cad-147">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="46cad-147">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="46cad-148">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="46cad-148">Recently deleted items.</span></span> <span data-ttu-id="46cad-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46cad-149">Read-only.</span></span> <span data-ttu-id="46cad-150">Anulável.</span><span class="sxs-lookup"><span data-stu-id="46cad-150">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46cad-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46cad-151">JSON representation</span></span>
<span data-ttu-id="46cad-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46cad-152">Here is a JSON representation of the resource.</span></span>

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
