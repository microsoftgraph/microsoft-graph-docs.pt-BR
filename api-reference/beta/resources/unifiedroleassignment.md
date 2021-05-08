---
title: Tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o link entre uma definição de função e uma entidade principal em um escopo específico para a finalidade de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: c52e6bb05c9258680a36f04ad428c24a3a2829fc
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239958"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="51506-103">Tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="51506-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51506-105">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="51506-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="51506-106">Ele representa uma definição de função atribuída a uma entidade principal (normalmente um usuário) em um escopo específico.</span><span class="sxs-lookup"><span data-stu-id="51506-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="51506-107">É necessário fornecer um directoryScopeId ou um appScopeId.</span><span class="sxs-lookup"><span data-stu-id="51506-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="51506-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="51506-108">Methods</span></span>

| <span data-ttu-id="51506-109">Método</span><span class="sxs-lookup"><span data-stu-id="51506-109">Method</span></span>       | <span data-ttu-id="51506-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51506-110">Return Type</span></span> | <span data-ttu-id="51506-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="51506-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="51506-112">Listar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-112">List unifiedRoleAssignment</span></span>](../api/rbacapplication-list-roleassignments.md) | [<span data-ttu-id="51506-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="51506-114">Leia uma lista de objetos unifiedRoleAssignment e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="51506-114">Read a list of unifiedRoleAssignment objects and their properties.</span></span> |
| [<span data-ttu-id="51506-115">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-115">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="51506-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="51506-117">Leia propriedades e relações do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="51506-117">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="51506-118">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-118">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="51506-119">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-119">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="51506-120">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="51506-120">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="51506-121">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="51506-121">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="51506-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51506-122">None</span></span> | <span data-ttu-id="51506-123">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="51506-123">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51506-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51506-124">Properties</span></span>

| <span data-ttu-id="51506-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51506-125">Property</span></span>     | <span data-ttu-id="51506-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="51506-126">Type</span></span>        | <span data-ttu-id="51506-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="51506-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51506-128">id</span><span class="sxs-lookup"><span data-stu-id="51506-128">id</span></span>|<span data-ttu-id="51506-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-129">String</span></span>| <span data-ttu-id="51506-130">O identificador exclusivo do unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="51506-130">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="51506-131">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51506-131">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="51506-132">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="51506-132">roleDefinitionId</span></span>|<span data-ttu-id="51506-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-133">String</span></span>| <span data-ttu-id="51506-134">Identificador do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="51506-134">Identifier of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="51506-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51506-135">Read-only.</span></span> <span data-ttu-id="51506-136">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="51506-136">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="51506-137">principalId</span><span class="sxs-lookup"><span data-stu-id="51506-137">principalId</span></span>|<span data-ttu-id="51506-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-138">String</span></span>| <span data-ttu-id="51506-139">Identificador da entidade à qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="51506-139">Identifier of the principal to which the assignment is granted.</span></span> <span data-ttu-id="51506-140">Suporta `$filter` ( `eq` somente operador).</span><span class="sxs-lookup"><span data-stu-id="51506-140">Supports `$filter` (`eq` operator only).</span></span> |
|<span data-ttu-id="51506-141">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="51506-141">directoryScopeId</span></span>|<span data-ttu-id="51506-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-142">String</span></span>|<span data-ttu-id="51506-143">Identificador do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="51506-143">Identifier of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="51506-144">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="51506-144">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="51506-145">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="51506-145">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="51506-146">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51506-146">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="51506-147">appScopeId</span><span class="sxs-lookup"><span data-stu-id="51506-147">appScopeId</span></span>|<span data-ttu-id="51506-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-148">String</span></span>|<span data-ttu-id="51506-149">Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51506-149">Identifier of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="51506-150">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="51506-150">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="51506-151">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="51506-151">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="51506-152">Use `/` para escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="51506-152">Use `/` for tenant-wide scope.</span></span> <span data-ttu-id="51506-153">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51506-153">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="51506-154">resourceScope</span><span class="sxs-lookup"><span data-stu-id="51506-154">resourceScope</span></span>|<span data-ttu-id="51506-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51506-155">String</span></span>| <span data-ttu-id="51506-156">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="51506-156">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="51506-157">Isso é `/` para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="51506-157">This is `/` for service-wide.</span></span> <span data-ttu-id="51506-158">**NÃO USE. Essa propriedade será preterida em breve.**</span><span class="sxs-lookup"><span data-stu-id="51506-158">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="51506-159">Relações</span><span class="sxs-lookup"><span data-stu-id="51506-159">Relationships</span></span>

| <span data-ttu-id="51506-160">Relação</span><span class="sxs-lookup"><span data-stu-id="51506-160">Relationship</span></span> | <span data-ttu-id="51506-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="51506-161">Type</span></span>   |<span data-ttu-id="51506-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="51506-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51506-163">appScope</span><span class="sxs-lookup"><span data-stu-id="51506-163">appScope</span></span>|[<span data-ttu-id="51506-164">appScope</span><span class="sxs-lookup"><span data-stu-id="51506-164">appScope</span></span>](appscope.md)|<span data-ttu-id="51506-165">Detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="51506-165">Details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="51506-166">Entidade de contenção.</span><span class="sxs-lookup"><span data-stu-id="51506-166">Containment entity.</span></span> |
|<span data-ttu-id="51506-167">directoryScope</span><span class="sxs-lookup"><span data-stu-id="51506-167">directoryScope</span></span>|[<span data-ttu-id="51506-168">directoryObject</span><span class="sxs-lookup"><span data-stu-id="51506-168">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="51506-169">O objeto directory que é o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="51506-169">The directory object that is the scope of the assignment.</span></span> <span data-ttu-id="51506-170">Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="51506-170">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="51506-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51506-171">Read-only.</span></span> <span data-ttu-id="51506-172">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="51506-172">Supports `$expand`.</span></span> |
|<span data-ttu-id="51506-173">principal</span><span class="sxs-lookup"><span data-stu-id="51506-173">principal</span></span>|[<span data-ttu-id="51506-174">directoryObject</span><span class="sxs-lookup"><span data-stu-id="51506-174">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="51506-175">A entidade atribuída.</span><span class="sxs-lookup"><span data-stu-id="51506-175">The assigned principal.</span></span> <span data-ttu-id="51506-176">Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="51506-176">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="51506-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51506-177">Read-only.</span></span> <span data-ttu-id="51506-178">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="51506-178">Supports `$expand`.</span></span> |
|<span data-ttu-id="51506-179">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="51506-179">roleDefinition</span></span>|[<span data-ttu-id="51506-180">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="51506-180">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="51506-181">A funçãoDefinition para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="51506-181">The roleDefinition the assignment is for.</span></span> <span data-ttu-id="51506-182">Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="51506-182">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="51506-183">**roleDefinition.id** será expandido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="51506-183">**roleDefinition.id** will be auto expanded.</span></span> <span data-ttu-id="51506-184">Oferece suporte para `$expand`.</span><span class="sxs-lookup"><span data-stu-id="51506-184">Supports `$expand`.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="51506-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51506-185">JSON representation</span></span>

<span data-ttu-id="51506-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51506-186">The following is a JSON representation of the resource.</span></span>

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

