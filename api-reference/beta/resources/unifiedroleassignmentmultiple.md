---
title: tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c49034c0d050c928b8a9192af6b2adee27a2a516
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988748"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="fdfeb-103">tipo de recurso unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="fdfeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdfeb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdfeb-105">Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="fdfeb-106">Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) em uma matriz de escopo.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="fdfeb-107">Um exemplo de um provedor RBAC é o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="fdfeb-108">No Microsoft Intune, você pode criar uma atribuição de função com várias entidades e vários escopos.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="fdfeb-109">É necessário fornecer o **directoryScopeIds** ou o **appScopeIds** .</span><span class="sxs-lookup"><span data-stu-id="fdfeb-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="fdfeb-110">Methods</span><span class="sxs-lookup"><span data-stu-id="fdfeb-110">Methods</span></span>

| <span data-ttu-id="fdfeb-111">Método</span><span class="sxs-lookup"><span data-stu-id="fdfeb-111">Method</span></span>       | <span data-ttu-id="fdfeb-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fdfeb-112">Return Type</span></span> | <span data-ttu-id="fdfeb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdfeb-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fdfeb-114">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="fdfeb-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="fdfeb-116">Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="fdfeb-117">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="fdfeb-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="fdfeb-119">Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="fdfeb-120">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="fdfeb-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="fdfeb-122">Atualize um objeto unifiedRoleAssignmentMultiple existente.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="fdfeb-123">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="fdfeb-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="fdfeb-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdfeb-124">None</span></span> | <span data-ttu-id="fdfeb-125">Exclua o objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fdfeb-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdfeb-126">Properties</span></span>

| <span data-ttu-id="fdfeb-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdfeb-127">Property</span></span>     | <span data-ttu-id="fdfeb-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdfeb-128">Type</span></span>        | <span data-ttu-id="fdfeb-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdfeb-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="fdfeb-130">id</span><span class="sxs-lookup"><span data-stu-id="fdfeb-130">id</span></span> | <span data-ttu-id="fdfeb-131">String</span><span class="sxs-lookup"><span data-stu-id="fdfeb-131">String</span></span> | <span data-ttu-id="fdfeb-132">O identificador exclusivo para o unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="fdfeb-133">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="fdfeb-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fdfeb-134">displayName</span></span> | <span data-ttu-id="fdfeb-135">String</span><span class="sxs-lookup"><span data-stu-id="fdfeb-135">String</span></span> | <span data-ttu-id="fdfeb-136">Nome da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-136">Name of the role assignment.</span></span> <span data-ttu-id="fdfeb-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-137">Required.</span></span> |
| <span data-ttu-id="fdfeb-138">description</span><span class="sxs-lookup"><span data-stu-id="fdfeb-138">description</span></span> | <span data-ttu-id="fdfeb-139">String</span><span class="sxs-lookup"><span data-stu-id="fdfeb-139">String</span></span> | <span data-ttu-id="fdfeb-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="fdfeb-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fdfeb-141">roleDefinitionId</span></span> | <span data-ttu-id="fdfeb-142">String</span><span class="sxs-lookup"><span data-stu-id="fdfeb-142">String</span></span> | <span data-ttu-id="fdfeb-143">ID do unifiedRoleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="fdfeb-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="fdfeb-144">roleDefinition</span></span> | [<span data-ttu-id="fdfeb-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="fdfeb-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="fdfeb-146">Propriedade que indica o roleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="fdfeb-147">Fornecido de modo que os chamadores possam obter a definição de função usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="fdfeb-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-148">Read-only.</span></span>  |
| <span data-ttu-id="fdfeb-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="fdfeb-149">principalIds</span></span> | <span data-ttu-id="fdfeb-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdfeb-150">String collection</span></span> | <span data-ttu-id="fdfeb-151">ObjectIDs das entidades de segurança para as quais a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="fdfeb-152">entidades</span><span class="sxs-lookup"><span data-stu-id="fdfeb-152">principals</span></span>| <span data-ttu-id="fdfeb-153">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fdfeb-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fdfeb-154">Coleção somente leitura fazendo referência a entidades de segurança atribuídas.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="fdfeb-155">Desde que os chamadores possam obter as entidades usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="fdfeb-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-156">Read-only.</span></span> |
| <span data-ttu-id="fdfeb-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="fdfeb-157">directoryScopeIds</span></span> | <span data-ttu-id="fdfeb-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdfeb-158">String collection</span></span> | <span data-ttu-id="fdfeb-159">IDs dos objetos de diretório que representam os escopos da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="fdfeb-160">Os escopos de uma atribuição determinam o conjunto de recursos para o qual foram concedidos acesso a entidades de segurança.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="fdfeb-161">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="fdfeb-162">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="fdfeb-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="fdfeb-163">directoryScopes</span></span> | <span data-ttu-id="fdfeb-164">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fdfeb-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="fdfeb-165">Coleção somente leitura fazendo referência aos objetos de diretório que são o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="fdfeb-166">Desde que os chamadores possam obter os objetos de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="fdfeb-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-167">Read-only.</span></span> |
| <span data-ttu-id="fdfeb-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="fdfeb-168">appScopeIds</span></span> | <span data-ttu-id="fdfeb-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="fdfeb-169">String collection</span></span> | <span data-ttu-id="fdfeb-170">IDs dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="fdfeb-171">Os escopos de uma atribuição determinam o conjunto de recursos para o qual a entidade de segurança recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="fdfeb-172">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="fdfeb-173">Use "/" para escopo em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="fdfeb-174">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="fdfeb-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="fdfeb-175">appScopes</span></span> | <span data-ttu-id="fdfeb-176">coleção [appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="fdfeb-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="fdfeb-177">Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="fdfeb-178">Entidade de confinamento.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-178">Containment entity.</span></span> <span data-ttu-id="fdfeb-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="fdfeb-180">Relações</span><span class="sxs-lookup"><span data-stu-id="fdfeb-180">Relationships</span></span>

<span data-ttu-id="fdfeb-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdfeb-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdfeb-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdfeb-182">JSON representation</span></span>

<span data-ttu-id="fdfeb-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdfeb-183">The following is a JSON representation of the resource.</span></span>

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


