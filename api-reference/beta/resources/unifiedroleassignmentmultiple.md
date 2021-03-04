---
title: Tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o link entre uma definição de função e uma entidade principal em um escopo específico para a finalidade de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f612fea9ce7aa54cce505a4f2d77370f45947c44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442688"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="a23fa-103">Tipo de recurso unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="a23fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a23fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a23fa-105">Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="a23fa-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="a23fa-106">Ele representa uma definição de função atribuída a uma matriz de entidades (normalmente um usuário) sobre uma matriz de escopo.</span><span class="sxs-lookup"><span data-stu-id="a23fa-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="a23fa-107">Um exemplo desse provedor RBAC é o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a23fa-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="a23fa-108">No Microsoft Intune, você pode criar uma atribuição de função com várias entidades principais e vários escopos.</span><span class="sxs-lookup"><span data-stu-id="a23fa-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="a23fa-109">É necessário **fornecer directoryScopeIds** **ou appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="a23fa-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="a23fa-110">Methods</span><span class="sxs-lookup"><span data-stu-id="a23fa-110">Methods</span></span>

| <span data-ttu-id="a23fa-111">Método</span><span class="sxs-lookup"><span data-stu-id="a23fa-111">Method</span></span>       | <span data-ttu-id="a23fa-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a23fa-112">Return Type</span></span> | <span data-ttu-id="a23fa-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23fa-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a23fa-114">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="a23fa-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="a23fa-116">Ler propriedades e relações do objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="a23fa-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="a23fa-117">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="a23fa-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="a23fa-119">Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="a23fa-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="a23fa-120">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="a23fa-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="a23fa-122">Atualize um objeto unifiedRoleAssignmentMultiple existente.</span><span class="sxs-lookup"><span data-stu-id="a23fa-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="a23fa-123">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="a23fa-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="a23fa-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="a23fa-124">None</span></span> | <span data-ttu-id="a23fa-125">Exclua o objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="a23fa-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a23fa-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a23fa-126">Properties</span></span>

| <span data-ttu-id="a23fa-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a23fa-127">Property</span></span>     | <span data-ttu-id="a23fa-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a23fa-128">Type</span></span>        | <span data-ttu-id="a23fa-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23fa-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a23fa-130">id</span><span class="sxs-lookup"><span data-stu-id="a23fa-130">id</span></span> | <span data-ttu-id="a23fa-131">String</span><span class="sxs-lookup"><span data-stu-id="a23fa-131">String</span></span> | <span data-ttu-id="a23fa-132">O identificador exclusivo do unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="a23fa-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="a23fa-133">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a23fa-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="a23fa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a23fa-134">displayName</span></span> | <span data-ttu-id="a23fa-135">String</span><span class="sxs-lookup"><span data-stu-id="a23fa-135">String</span></span> | <span data-ttu-id="a23fa-136">Nome da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a23fa-136">Name of the role assignment.</span></span> <span data-ttu-id="a23fa-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a23fa-137">Required.</span></span> |
| <span data-ttu-id="a23fa-138">description</span><span class="sxs-lookup"><span data-stu-id="a23fa-138">description</span></span> | <span data-ttu-id="a23fa-139">String</span><span class="sxs-lookup"><span data-stu-id="a23fa-139">String</span></span> | <span data-ttu-id="a23fa-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a23fa-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="a23fa-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a23fa-141">roleDefinitionId</span></span> | <span data-ttu-id="a23fa-142">String</span><span class="sxs-lookup"><span data-stu-id="a23fa-142">String</span></span> | <span data-ttu-id="a23fa-143">ID do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="a23fa-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="a23fa-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="a23fa-144">roleDefinition</span></span> | [<span data-ttu-id="a23fa-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a23fa-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="a23fa-146">Propriedade indicando a funçãoDefinition para a qual a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="a23fa-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="a23fa-147">Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a23fa-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a23fa-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a23fa-148">Read-only.</span></span>  |
| <span data-ttu-id="a23fa-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="a23fa-149">principalIds</span></span> | <span data-ttu-id="a23fa-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a23fa-150">String collection</span></span> | <span data-ttu-id="a23fa-151">Objectids das entidades a que a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="a23fa-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="a23fa-152">principais</span><span class="sxs-lookup"><span data-stu-id="a23fa-152">principals</span></span>| <span data-ttu-id="a23fa-153">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a23fa-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a23fa-154">Coleção somente leitura fazendo referência às entidades atribuídas.</span><span class="sxs-lookup"><span data-stu-id="a23fa-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="a23fa-155">Fornecido para que os chamadores possam obter as entidades que `$expand` usam ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a23fa-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a23fa-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a23fa-156">Read-only.</span></span> |
| <span data-ttu-id="a23fa-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="a23fa-157">directoryScopeIds</span></span> | <span data-ttu-id="a23fa-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a23fa-158">String collection</span></span> | <span data-ttu-id="a23fa-159">Ids dos objetos de diretório que representam os escopos da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a23fa-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="a23fa-160">Os escopos de uma atribuição determinam o conjunto de recursos para os quais as entidades foram concedidas acesso.</span><span class="sxs-lookup"><span data-stu-id="a23fa-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="a23fa-161">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a23fa-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="a23fa-162">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a23fa-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="a23fa-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="a23fa-163">directoryScopes</span></span> | <span data-ttu-id="a23fa-164">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a23fa-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="a23fa-165">Coleção somente leitura fazendo referência aos objetos de diretório que são escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a23fa-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="a23fa-166">Fornecido para que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a23fa-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="a23fa-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a23fa-167">Read-only.</span></span> |
| <span data-ttu-id="a23fa-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="a23fa-168">appScopeIds</span></span> | <span data-ttu-id="a23fa-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a23fa-169">String collection</span></span> | <span data-ttu-id="a23fa-170">Ids dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a23fa-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="a23fa-171">Os escopos de uma atribuição determinam o conjunto de recursos para os quais a entidade recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="a23fa-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="a23fa-172">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="a23fa-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="a23fa-173">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="a23fa-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="a23fa-174">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a23fa-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="a23fa-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="a23fa-175">appScopes</span></span> | <span data-ttu-id="a23fa-176">[Coleção appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="a23fa-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="a23fa-177">Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a23fa-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="a23fa-178">Entidade de contenção.</span><span class="sxs-lookup"><span data-stu-id="a23fa-178">Containment entity.</span></span> <span data-ttu-id="a23fa-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a23fa-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="a23fa-180">Relações</span><span class="sxs-lookup"><span data-stu-id="a23fa-180">Relationships</span></span>

<span data-ttu-id="a23fa-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a23fa-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a23fa-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a23fa-182">JSON representation</span></span>

<span data-ttu-id="a23fa-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a23fa-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
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


