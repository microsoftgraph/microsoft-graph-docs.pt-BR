---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b35c2c56c7033cd668b311c17169f5c719e5948
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062079"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="167cf-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="167cf-105">directory resource type (deleted items)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="167cf-106">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="167cf-106">Represents a deleted item in the directory.</span></span> <span data-ttu-id="167cf-107">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="167cf-107">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="167cf-108">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="167cf-108">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="167cf-109">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="167cf-109">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="167cf-110">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para [grupos](group.md) e [usuários](users.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="167cf-110">Currently, deleted items functionality is only supported for Office 365 [groups](group.md) and [users](users.md).</span></span>

## <a name="methods"></a><span data-ttu-id="167cf-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="167cf-111">Methods</span></span>

| <span data-ttu-id="167cf-112">Método</span><span class="sxs-lookup"><span data-stu-id="167cf-112">Method</span></span>         | <span data-ttu-id="167cf-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="167cf-113">Return Type</span></span> | <span data-ttu-id="167cf-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="167cf-114">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="167cf-115">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="167cf-115">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="167cf-116">directoryObject</span><span class="sxs-lookup"><span data-stu-id="167cf-116">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="167cf-117">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="167cf-117">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="167cf-118">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="167cf-118">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="167cf-119">directoryObject</span><span class="sxs-lookup"><span data-stu-id="167cf-119">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="167cf-120">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="167cf-120">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="167cf-121">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="167cf-121">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="167cf-122">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="167cf-122">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="167cf-123">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="167cf-123">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="167cf-124">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="167cf-124">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="167cf-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="167cf-125">None</span></span> | <span data-ttu-id="167cf-126">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="167cf-126">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="167cf-127">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="167cf-127">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="167cf-128">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="167cf-128">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="167cf-129">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="167cf-129">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="167cf-130">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="167cf-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="167cf-131">coleção [featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="167cf-131">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="167cf-132">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="167cf-132">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="167cf-133">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="167cf-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="167cf-135">Criar um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="167cf-135">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="167cf-136">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-136">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="167cf-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="167cf-138">Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="167cf-138">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="167cf-139">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="167cf-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="167cf-141">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="167cf-141">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="167cf-142">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="167cf-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="167cf-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="167cf-143">None</span></span> | <span data-ttu-id="167cf-144">Excluir um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="167cf-144">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="167cf-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="167cf-145">Properties</span></span>
| <span data-ttu-id="167cf-146">Propriedade</span><span class="sxs-lookup"><span data-stu-id="167cf-146">Property</span></span>   | <span data-ttu-id="167cf-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="167cf-147">Type</span></span> |<span data-ttu-id="167cf-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="167cf-148">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="167cf-149">id</span><span class="sxs-lookup"><span data-stu-id="167cf-149">id</span></span>|<span data-ttu-id="167cf-150">String</span><span class="sxs-lookup"><span data-stu-id="167cf-150">String</span></span>| <span data-ttu-id="167cf-151">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="167cf-151">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="167cf-152">Chave.</span><span class="sxs-lookup"><span data-stu-id="167cf-152">Key.</span></span> <span data-ttu-id="167cf-153">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="167cf-153">Not nullable.</span></span> <span data-ttu-id="167cf-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="167cf-154">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="167cf-155">Relações</span><span class="sxs-lookup"><span data-stu-id="167cf-155">Relationships</span></span>
| <span data-ttu-id="167cf-156">Relação</span><span class="sxs-lookup"><span data-stu-id="167cf-156">Relationship</span></span> | <span data-ttu-id="167cf-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="167cf-157">Type</span></span>   |<span data-ttu-id="167cf-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="167cf-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="167cf-159">deleteditems</span><span class="sxs-lookup"><span data-stu-id="167cf-159">deleteditems</span></span>|<span data-ttu-id="167cf-160">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="167cf-160">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="167cf-161">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="167cf-161">Recently deleted items.</span></span> <span data-ttu-id="167cf-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="167cf-162">Read-only.</span></span> <span data-ttu-id="167cf-163">Anulável.</span><span class="sxs-lookup"><span data-stu-id="167cf-163">Nullable.</span></span>|
|<span data-ttu-id="167cf-164">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="167cf-164">featureRolloutPolicies</span></span>|<span data-ttu-id="167cf-165">coleção [featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="167cf-165">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="167cf-166">Anulável.</span><span class="sxs-lookup"><span data-stu-id="167cf-166">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="167cf-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="167cf-167">JSON representation</span></span>
<span data-ttu-id="167cf-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="167cf-168">Here is a JSON representation of the resource.</span></span>

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
