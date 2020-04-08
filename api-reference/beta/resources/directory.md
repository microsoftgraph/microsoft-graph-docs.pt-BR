---
title: Tipo de recurso directory (itens excluídos)
description: . Itens excluídos permanecerão disponíveis para restauração por até 30 dias. Após 30 dias, esses itens serão excluídos permanentemente.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba7d1cb38e1b33d7007cf4613550868d2b634c11
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181368"
---
# <a name="directory-resource-type-deleted-items"></a><span data-ttu-id="133d6-105">Tipo de recurso directory (itens excluídos)</span><span class="sxs-lookup"><span data-stu-id="133d6-105">directory resource type (deleted items)</span></span>

<span data-ttu-id="133d6-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="133d6-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="133d6-107">Representa um item excluído no diretório.</span><span class="sxs-lookup"><span data-stu-id="133d6-107">Represents a deleted item in the directory.</span></span> <span data-ttu-id="133d6-108">Quando um item é excluído, ele é adicionado ao "contêiner" de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="133d6-108">When an item is deleted, it is added to the deleted items "container".</span></span> <span data-ttu-id="133d6-109">Itens excluídos permanecerão disponíveis para restauração por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="133d6-109">Deleted items will remain available to restore for up to 30 days.</span></span> <span data-ttu-id="133d6-110">Após 30 dias, esses itens serão excluídos permanentemente.</span><span class="sxs-lookup"><span data-stu-id="133d6-110">After 30 days, the items are permanently deleted.</span></span>

<span data-ttu-id="133d6-111">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](application.md), [grupo](group.md) e recursos do [usuário](user.md) .</span><span class="sxs-lookup"><span data-stu-id="133d6-111">Currently, deleted items functionality is only supported for the [application](application.md), [group](group.md) and [user](user.md) resources.</span></span>

## <a name="methods"></a><span data-ttu-id="133d6-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="133d6-112">Methods</span></span>

| <span data-ttu-id="133d6-113">Método</span><span class="sxs-lookup"><span data-stu-id="133d6-113">Method</span></span>         | <span data-ttu-id="133d6-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="133d6-114">Return Type</span></span> | <span data-ttu-id="133d6-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="133d6-115">Description</span></span> |
|:---------------|:------------|:------------|
|[<span data-ttu-id="133d6-116">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="133d6-116">Get deleted item</span></span>](../api/directory-deleteditems-get.md) | [<span data-ttu-id="133d6-117">directoryObject</span><span class="sxs-lookup"><span data-stu-id="133d6-117">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="133d6-118">Obtém as propriedades de um item excluído.</span><span class="sxs-lookup"><span data-stu-id="133d6-118">Gets the properties of a deleted item.</span></span> |
|[<span data-ttu-id="133d6-119">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="133d6-119">Restore deleted item</span></span>](../api/directory-deleteditems-restore.md) |[<span data-ttu-id="133d6-120">directoryObject</span><span class="sxs-lookup"><span data-stu-id="133d6-120">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="133d6-121">Restaura um item recentemente excluído.</span><span class="sxs-lookup"><span data-stu-id="133d6-121">Restores a recently deleted item.</span></span> |
|[<span data-ttu-id="133d6-122">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="133d6-122">List deleted items</span></span>](../api/directory-deleteditems-list.md) |<span data-ttu-id="133d6-123">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="133d6-123">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="133d6-124">Obtém uma lista de itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="133d6-124">Gets a list of recently deleted items.</span></span> |
|[<span data-ttu-id="133d6-125">Excluir permanentemente um item</span><span class="sxs-lookup"><span data-stu-id="133d6-125">Permanently delete an item</span></span>](../api/directory-deleteditems-delete.md) | <span data-ttu-id="133d6-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="133d6-126">None</span></span> | <span data-ttu-id="133d6-127">Exclui permanentemente um item.</span><span class="sxs-lookup"><span data-stu-id="133d6-127">Permanently deletes an item.</span></span> |
|[<span data-ttu-id="133d6-128">Listar itens excluídos pertencentes a um usuário</span><span class="sxs-lookup"><span data-stu-id="133d6-128">List deleted items owned by a user</span></span>](../api/directory-deleteditems-user-owned.md) | <span data-ttu-id="133d6-129">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="133d6-129">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="133d6-130">Lista itens de diretório pertencentes a um usuário.</span><span class="sxs-lookup"><span data-stu-id="133d6-130">Lists directory items owned by a user.</span></span> |
|[<span data-ttu-id="133d6-131">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="133d6-131">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | <span data-ttu-id="133d6-132">coleção [featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="133d6-132">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span> | <span data-ttu-id="133d6-133">Recupere uma lista de objetos featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="133d6-133">Retrieve a list of featureRolloutPolicy objects.</span></span> |
|[<span data-ttu-id="133d6-134">Criar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="133d6-135">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="133d6-136">Criar um novo objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="133d6-136">Create a new featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="133d6-137">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-137">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="133d6-138">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="133d6-139">Recupere as propriedades e os relacionamentos do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="133d6-139">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="133d6-140">Atualizar featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-140">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="133d6-141">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-141">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="133d6-142">Atualize as propriedades do objeto featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="133d6-142">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="133d6-143">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="133d6-143">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="133d6-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="133d6-144">None</span></span> | <span data-ttu-id="133d6-145">Excluir um objeto featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="133d6-145">Delete a featureRolloutPolicy object.</span></span> |

## <a name="properties"></a><span data-ttu-id="133d6-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="133d6-146">Properties</span></span>
| <span data-ttu-id="133d6-147">Propriedade</span><span class="sxs-lookup"><span data-stu-id="133d6-147">Property</span></span>   | <span data-ttu-id="133d6-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="133d6-148">Type</span></span> |<span data-ttu-id="133d6-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="133d6-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="133d6-150">id</span><span class="sxs-lookup"><span data-stu-id="133d6-150">id</span></span>|<span data-ttu-id="133d6-151">String</span><span class="sxs-lookup"><span data-stu-id="133d6-151">String</span></span>| <span data-ttu-id="133d6-152">Um identificador exclusivo para o objeto; por exemplo, 12345678-9abc-def0-1234-56789abcde.</span><span class="sxs-lookup"><span data-stu-id="133d6-152">A unique identifier for the object; for example, 12345678-9abc-def0-1234-56789abcde.</span></span> <span data-ttu-id="133d6-153">Chave.</span><span class="sxs-lookup"><span data-stu-id="133d6-153">Key.</span></span> <span data-ttu-id="133d6-154">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="133d6-154">Not nullable.</span></span> <span data-ttu-id="133d6-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="133d6-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="133d6-156">Relações</span><span class="sxs-lookup"><span data-stu-id="133d6-156">Relationships</span></span>
| <span data-ttu-id="133d6-157">Relação</span><span class="sxs-lookup"><span data-stu-id="133d6-157">Relationship</span></span> | <span data-ttu-id="133d6-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="133d6-158">Type</span></span>   |<span data-ttu-id="133d6-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="133d6-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="133d6-160">deleteditems</span><span class="sxs-lookup"><span data-stu-id="133d6-160">deleteditems</span></span>|<span data-ttu-id="133d6-161">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="133d6-161">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="133d6-162">Itens recentemente excluídos.</span><span class="sxs-lookup"><span data-stu-id="133d6-162">Recently deleted items.</span></span> <span data-ttu-id="133d6-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="133d6-163">Read-only.</span></span> <span data-ttu-id="133d6-164">Anulável.</span><span class="sxs-lookup"><span data-stu-id="133d6-164">Nullable.</span></span>|
|<span data-ttu-id="133d6-165">featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="133d6-165">featureRolloutPolicies</span></span>|<span data-ttu-id="133d6-166">coleção [featureRolloutPolicy](featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="133d6-166">[featureRolloutPolicy](featurerolloutpolicy.md) collection</span></span>| <span data-ttu-id="133d6-167">Anulável.</span><span class="sxs-lookup"><span data-stu-id="133d6-167">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="133d6-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="133d6-168">JSON representation</span></span>
<span data-ttu-id="133d6-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="133d6-169">Here is a JSON representation of the resource.</span></span>

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
