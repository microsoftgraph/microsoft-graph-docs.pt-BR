---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4eb1cbdcbf0a1256c2bf2bf0cec35479b8bbc2cc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962620"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="acc77-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="acc77-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="acc77-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acc77-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acc77-107">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="acc77-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="acc77-108">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="acc77-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="acc77-109">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="acc77-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="acc77-110">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="acc77-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="acc77-111">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](application.md)aplicativo, [grupo](group.md) [e](user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="acc77-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="acc77-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="acc77-112">Methods</span></span>

| <span data-ttu-id="acc77-113">Método</span><span class="sxs-lookup"><span data-stu-id="acc77-113">Method</span></span>         | <span data-ttu-id="acc77-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="acc77-114">Return Type</span></span> | <span data-ttu-id="acc77-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="acc77-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="acc77-116">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="acc77-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="acc77-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="acc77-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="acc77-118">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="acc77-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="acc77-119">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="acc77-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="acc77-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="acc77-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="acc77-121">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="acc77-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="acc77-122">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="acc77-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="acc77-123">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="acc77-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="acc77-124">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="acc77-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="acc77-125">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="acc77-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="acc77-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acc77-126">None</span></span> | <span data-ttu-id="acc77-127">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="acc77-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="acc77-128">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="acc77-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="acc77-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="acc77-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="acc77-130">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="acc77-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="acc77-131">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="acc77-131">List featureRolloutPolicies</span></span>](../api/list-featurerolloutpolicies.md) | <span data-ttu-id="acc77-132">[Coleção featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="acc77-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="acc77-133">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="acc77-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="acc77-134">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-134">Create featureRolloutPolicy</span></span>](../api/post-featurerolloutpolicies.md) | [<span data-ttu-id="acc77-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="acc77-136">Crie um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="acc77-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="acc77-137">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="acc77-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="acc77-139">Recupere as propriedades e as relações do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="acc77-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="acc77-140">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="acc77-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="acc77-142">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="acc77-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="acc77-143">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="acc77-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="acc77-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="acc77-144">None</span></span> | <span data-ttu-id="acc77-145">Exclua um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="acc77-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="acc77-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acc77-146">Properties</span></span>
| <span data-ttu-id="acc77-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acc77-147">Property</span></span>   | <span data-ttu-id="acc77-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="acc77-148">Type</span></span> |<span data-ttu-id="acc77-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="acc77-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acc77-150">id</span><span class="sxs-lookup"><span data-stu-id="acc77-150">id</span></span>|<span data-ttu-id="acc77-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="acc77-151">String</span></span>| <span data-ttu-id="acc77-152">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="acc77-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="acc77-153">Chave.</span><span class="sxs-lookup"><span data-stu-id="acc77-153">Key.</span></span> <span data-ttu-id="acc77-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="acc77-154">Not nullable.</span></span> <span data-ttu-id="acc77-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acc77-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acc77-156">Relações</span><span class="sxs-lookup"><span data-stu-id="acc77-156">Relationships</span></span>
| <span data-ttu-id="acc77-157">Relação</span><span class="sxs-lookup"><span data-stu-id="acc77-157">Relationship</span></span> | <span data-ttu-id="acc77-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="acc77-158">Type</span></span>   |<span data-ttu-id="acc77-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="acc77-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="acc77-160">deleteditems</span><span class="sxs-lookup"><span data-stu-id="acc77-160">deleteditems</span></span>|<span data-ttu-id="acc77-161">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="acc77-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="acc77-162">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="acc77-162">Recently deleted items.</span></span> <span data-ttu-id="acc77-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="acc77-163">Read-only.</span></span> <span data-ttu-id="acc77-164">Anulável.</span><span class="sxs-lookup"><span data-stu-id="acc77-164">Nullable.</span></span>|
|<span data-ttu-id="acc77-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="acc77-165">featureRolloutPolicies</span></span>|<span data-ttu-id="acc77-166">[Coleção featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="acc77-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="acc77-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="acc77-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acc77-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acc77-168">JSON representation</span></span>
<span data-ttu-id="acc77-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acc77-169">Here is a JSON representation of the resource.</span></span>

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


