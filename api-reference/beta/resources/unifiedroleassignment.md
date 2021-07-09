---
title: Tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o link entre uma definição de função e uma entidade principal em um escopo específico para a finalidade de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 16e03168f9eee4af8c6e69c7ee4fb774494643b4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350996"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="86dbd-103">Tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="86dbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86dbd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86dbd-105">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="86dbd-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="86dbd-106">Ele representa uma definição de função atribuída a uma entidade principal (normalmente um usuário) em um escopo específico.</span><span class="sxs-lookup"><span data-stu-id="86dbd-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="86dbd-107">É necessário fornecer um directoryScopeId ou um appScopeId.</span><span class="sxs-lookup"><span data-stu-id="86dbd-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="86dbd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="86dbd-108">Methods</span></span>

| <span data-ttu-id="86dbd-109">Método</span><span class="sxs-lookup"><span data-stu-id="86dbd-109">Method</span></span>       | <span data-ttu-id="86dbd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="86dbd-110">Return Type</span></span> | <span data-ttu-id="86dbd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86dbd-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="86dbd-112">Listar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-112">List unifiedRoleAssignment</span></span>](../api/rbacapplication-list-roleassignments.md) | [<span data-ttu-id="86dbd-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="86dbd-114">Leia uma lista de objetos unifiedRoleAssignment e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="86dbd-114">Read a list of unifiedRoleAssignment objects and their properties.</span></span> |
| [<span data-ttu-id="86dbd-115">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-115">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="86dbd-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="86dbd-117">Leia propriedades e relações do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="86dbd-117">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="86dbd-118">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-118">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="86dbd-119">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-119">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="86dbd-120">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="86dbd-120">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="86dbd-121">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="86dbd-121">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="86dbd-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="86dbd-122">None</span></span> | <span data-ttu-id="86dbd-123">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="86dbd-123">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86dbd-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86dbd-124">Properties</span></span>

| <span data-ttu-id="86dbd-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86dbd-125">Property</span></span>     | <span data-ttu-id="86dbd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="86dbd-126">Type</span></span>        | <span data-ttu-id="86dbd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="86dbd-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86dbd-128">id</span><span class="sxs-lookup"><span data-stu-id="86dbd-128">id</span></span>|<span data-ttu-id="86dbd-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-129">String</span></span>| <span data-ttu-id="86dbd-130">O identificador exclusivo do unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="86dbd-130">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="86dbd-131">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86dbd-131">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="86dbd-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="86dbd-132">roleDefinitionId</span></span>|<span data-ttu-id="86dbd-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-133">String</span></span>| <span data-ttu-id="86dbd-134">Identificador do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="86dbd-134">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="86dbd-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86dbd-135">Read-only.</span></span> <span data-ttu-id="86dbd-136">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="86dbd-136">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="86dbd-137">principalId</span><span class="sxs-lookup"><span data-stu-id="86dbd-137">principalId</span></span>|<span data-ttu-id="86dbd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-138">String</span></span>| <span data-ttu-id="86dbd-139">Identificador da entidade à qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="86dbd-139">Identifier of the principal to which the assignment is granted.</span></span> <span data-ttu-id="86dbd-140">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="86dbd-140">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="86dbd-141">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="86dbd-141">directoryScopeId</span></span>|<span data-ttu-id="86dbd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-142">String</span></span>|<span data-ttu-id="86dbd-143">Identificador do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="86dbd-143">Identifier of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="86dbd-144">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="86dbd-144">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="86dbd-145">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="86dbd-145">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="86dbd-146">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86dbd-146">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="86dbd-147">appScopeId</span><span class="sxs-lookup"><span data-stu-id="86dbd-147">appScopeId</span></span>|<span data-ttu-id="86dbd-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-148">String</span></span>|<span data-ttu-id="86dbd-149">Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86dbd-149">Identifier of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="86dbd-150">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="86dbd-150">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="86dbd-151">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="86dbd-151">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="86dbd-152">Use `/` para escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="86dbd-152">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="86dbd-153">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86dbd-153">App scopes are scopes that are defined and understood by this application only.</span></span>  <span data-ttu-id="86dbd-154">Para o provedor de gerenciamento de direitos, use escopos de aplicativo para especificar um catálogo, por exemplo `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997` .</span><span class="sxs-lookup"><span data-stu-id="86dbd-154">For the entitlement management provider, use app scopes to specify a catalog, for example `/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997`.</span></span>|
|<span data-ttu-id="86dbd-155">resourceScope</span><span class="sxs-lookup"><span data-stu-id="86dbd-155">resourceScope</span></span>|<span data-ttu-id="86dbd-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86dbd-156">String</span></span>| <span data-ttu-id="86dbd-157">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="86dbd-157">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="86dbd-158">Isso é `/` para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="86dbd-158">This is `/` for service-wide.</span></span> <span data-ttu-id="86dbd-159">**NÃO USE. Essa propriedade será preterida em breve.**</span><span class="sxs-lookup"><span data-stu-id="86dbd-159">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="86dbd-160">Relações</span><span class="sxs-lookup"><span data-stu-id="86dbd-160">Relationships</span></span>

| <span data-ttu-id="86dbd-161">Relação</span><span class="sxs-lookup"><span data-stu-id="86dbd-161">Relationship</span></span> | <span data-ttu-id="86dbd-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="86dbd-162">Type</span></span>   |<span data-ttu-id="86dbd-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="86dbd-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86dbd-164">appScope</span><span class="sxs-lookup"><span data-stu-id="86dbd-164">appScope</span></span>|[<span data-ttu-id="86dbd-165">appScope</span><span class="sxs-lookup"><span data-stu-id="86dbd-165">appScope</span></span>](appscope.md)|<span data-ttu-id="86dbd-166">Detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86dbd-166">Details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="86dbd-167">Entidade de contenção.</span><span class="sxs-lookup"><span data-stu-id="86dbd-167">Containment entity.</span></span> |
|<span data-ttu-id="86dbd-168">directoryScope</span><span class="sxs-lookup"><span data-stu-id="86dbd-168">directoryScope</span></span>|[<span data-ttu-id="86dbd-169">directoryObject</span><span class="sxs-lookup"><span data-stu-id="86dbd-169">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="86dbd-170">O objeto directory que é o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="86dbd-170">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="86dbd-171">Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="86dbd-171">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="86dbd-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86dbd-172">Read-only.</span></span> <span data-ttu-id="86dbd-173">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="86dbd-173">Supports `$expand`.</span></span> |
|<span data-ttu-id="86dbd-174">principal</span><span class="sxs-lookup"><span data-stu-id="86dbd-174">principal</span></span>|[<span data-ttu-id="86dbd-175">directoryObject</span><span class="sxs-lookup"><span data-stu-id="86dbd-175">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="86dbd-176">A entidade atribuída.</span><span class="sxs-lookup"><span data-stu-id="86dbd-176">The assigned principal.</span></span> <span data-ttu-id="86dbd-177">Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="86dbd-177">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="86dbd-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="86dbd-178">Read-only.</span></span> <span data-ttu-id="86dbd-179">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="86dbd-179">Supports `$expand`.</span></span> |
|<span data-ttu-id="86dbd-180">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86dbd-180">roleDefinition</span></span>|[<span data-ttu-id="86dbd-181">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="86dbd-181">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="86dbd-182">A funçãoDefinition para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="86dbd-182">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="86dbd-183">Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="86dbd-183">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="86dbd-184">**roleDefinition.id** será expandido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="86dbd-184">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="86dbd-185">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="86dbd-185">Supports `$expand`.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="86dbd-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86dbd-186">JSON representation</span></span>

<span data-ttu-id="86dbd-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86dbd-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalId": "String",
  "principal": {"@odata.type": "microsoft.graph.directoryObject"},
  "directoryScopeId": "String",
  "directoryScope": {"@odata.type": "microsoft.graph.directoryObject"},
  "appScopeId": "String",
  "appScope": {"@odata.type": "microsoft.graph.appScope"},
  "resourceScope": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
