---
title: tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: eb763490e9d60ca386400eef3dae1b9e2d382d21
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038659"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="776aa-103">tipo de recurso unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="776aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="776aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="776aa-105">Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="776aa-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="776aa-106">Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) em uma matriz de escopo.</span><span class="sxs-lookup"><span data-stu-id="776aa-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="776aa-107">Um exemplo de um provedor RBAC é o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="776aa-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="776aa-108">No Microsoft Intune, você pode criar uma atribuição de função com várias entidades e vários escopos.</span><span class="sxs-lookup"><span data-stu-id="776aa-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="776aa-109">É necessário fornecer o **directoryScopeIds** ou o **appScopeIds** .</span><span class="sxs-lookup"><span data-stu-id="776aa-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="776aa-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="776aa-110">Methods</span></span>

| <span data-ttu-id="776aa-111">Método</span><span class="sxs-lookup"><span data-stu-id="776aa-111">Method</span></span>       | <span data-ttu-id="776aa-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="776aa-112">Return Type</span></span> | <span data-ttu-id="776aa-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="776aa-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="776aa-114">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="776aa-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="776aa-116">Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="776aa-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="776aa-117">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="776aa-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="776aa-119">Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="776aa-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="776aa-120">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="776aa-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="776aa-122">Atualize um objeto unifiedRoleAssignmentMultiple existente.</span><span class="sxs-lookup"><span data-stu-id="776aa-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="776aa-123">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="776aa-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="776aa-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="776aa-124">None</span></span> | <span data-ttu-id="776aa-125">Exclua o objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="776aa-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="776aa-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="776aa-126">Properties</span></span>

| <span data-ttu-id="776aa-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="776aa-127">Property</span></span>     | <span data-ttu-id="776aa-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="776aa-128">Type</span></span>        | <span data-ttu-id="776aa-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="776aa-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="776aa-130">id</span><span class="sxs-lookup"><span data-stu-id="776aa-130">id</span></span> | <span data-ttu-id="776aa-131">String</span><span class="sxs-lookup"><span data-stu-id="776aa-131">String</span></span> | <span data-ttu-id="776aa-132">O identificador exclusivo para o unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="776aa-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="776aa-133">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="776aa-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="776aa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="776aa-134">displayName</span></span> | <span data-ttu-id="776aa-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="776aa-135">String</span></span> | <span data-ttu-id="776aa-136">Nome da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="776aa-136">Name of the role assignment.</span></span> <span data-ttu-id="776aa-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="776aa-137">Required.</span></span> |
| <span data-ttu-id="776aa-138">description</span><span class="sxs-lookup"><span data-stu-id="776aa-138">description</span></span> | <span data-ttu-id="776aa-139">String</span><span class="sxs-lookup"><span data-stu-id="776aa-139">String</span></span> | <span data-ttu-id="776aa-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="776aa-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="776aa-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="776aa-141">roleDefinitionId</span></span> | <span data-ttu-id="776aa-142">String</span><span class="sxs-lookup"><span data-stu-id="776aa-142">String</span></span> | <span data-ttu-id="776aa-143">ID do unifiedRoleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="776aa-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="776aa-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="776aa-144">roleDefinition</span></span> | [<span data-ttu-id="776aa-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="776aa-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="776aa-146">Propriedade que indica o roleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="776aa-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="776aa-147">Fornecido de modo que os chamadores possam obter a definição de função usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="776aa-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="776aa-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="776aa-148">Read-only.</span></span>  |
| <span data-ttu-id="776aa-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="776aa-149">principalIds</span></span> | <span data-ttu-id="776aa-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="776aa-150">String collection</span></span> | <span data-ttu-id="776aa-151">ObjectIDs das entidades de segurança para as quais a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="776aa-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="776aa-152">entidades</span><span class="sxs-lookup"><span data-stu-id="776aa-152">principals</span></span>| <span data-ttu-id="776aa-153">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="776aa-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="776aa-154">Coleção somente leitura fazendo referência a entidades de segurança atribuídas.</span><span class="sxs-lookup"><span data-stu-id="776aa-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="776aa-155">Desde que os chamadores possam obter as entidades usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="776aa-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="776aa-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="776aa-156">Read-only.</span></span> |
| <span data-ttu-id="776aa-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="776aa-157">directoryScopeIds</span></span> | <span data-ttu-id="776aa-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="776aa-158">String collection</span></span> | <span data-ttu-id="776aa-159">IDs dos objetos de diretório que representam os escopos da atribuição.</span><span class="sxs-lookup"><span data-stu-id="776aa-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="776aa-160">Os escopos de uma atribuição determinam o conjunto de recursos para o qual foram concedidos acesso a entidades de segurança.</span><span class="sxs-lookup"><span data-stu-id="776aa-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="776aa-161">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="776aa-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="776aa-162">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="776aa-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="776aa-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="776aa-163">directoryScopes</span></span> | <span data-ttu-id="776aa-164">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="776aa-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="776aa-165">Coleção somente leitura fazendo referência aos objetos de diretório que são o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="776aa-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="776aa-166">Desde que os chamadores possam obter os objetos de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="776aa-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="776aa-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="776aa-167">Read-only.</span></span> |
| <span data-ttu-id="776aa-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="776aa-168">appScopeIds</span></span> | <span data-ttu-id="776aa-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="776aa-169">String collection</span></span> | <span data-ttu-id="776aa-170">IDs dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="776aa-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="776aa-171">Os escopos de uma atribuição determinam o conjunto de recursos para o qual a entidade de segurança recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="776aa-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="776aa-172">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="776aa-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="776aa-173">Use "/" para escopo em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="776aa-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="776aa-174">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="776aa-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="776aa-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="776aa-175">appScopes</span></span> | <span data-ttu-id="776aa-176">coleção [appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="776aa-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="776aa-177">Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="776aa-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="776aa-178">Entidade de confinamento.</span><span class="sxs-lookup"><span data-stu-id="776aa-178">Containment entity.</span></span> <span data-ttu-id="776aa-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="776aa-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="776aa-180">Relações</span><span class="sxs-lookup"><span data-stu-id="776aa-180">Relationships</span></span>

<span data-ttu-id="776aa-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="776aa-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="776aa-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="776aa-182">JSON representation</span></span>

<span data-ttu-id="776aa-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="776aa-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleDefinitionId": "String",
  "roleDefinition": {"@odata.type": "microsoft.graph.unifiedRoleDefinition"},
  "principalIds": ["string"],
  "principals": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directoryScopeIds": ["string"],
  "directoryScopes": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "appScopeIds": ["string"],
  "appScopes": [{"@odata.type": "microsoft.graph.appScope"}],
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignmentMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
