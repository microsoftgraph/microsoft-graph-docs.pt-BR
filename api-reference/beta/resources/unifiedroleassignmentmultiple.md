---
title: Tipo de recurso unifiedRoleAssignmentMultiple
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de serviço em um escopo específico para fins de concessão de acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4df17c6b112cefe03a12631ee763f49e976fb568
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159840"
---
# <a name="unifiedroleassignmentmultiple-resource-type"></a><span data-ttu-id="372fe-103">Tipo de recurso unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-103">unifiedRoleAssignmentMultiple resource type</span></span>

<span data-ttu-id="372fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="372fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="372fe-105">Um unifiedRoleAssignmentMultiple é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="372fe-105">A unifiedRoleAssignmentMultiple is used to grant access to resources.</span></span> <span data-ttu-id="372fe-106">Ele representa uma definição de função atribuída a uma matriz de entidades de segurança (normalmente um usuário) em uma matriz de escopo.</span><span class="sxs-lookup"><span data-stu-id="372fe-106">It represents a role definition assigned to an array of principals (typically a user) over an array of scope.</span></span> <span data-ttu-id="372fe-107">Um exemplo desse provedor de RBAC é o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="372fe-107">An example of such an RBAC provider is Microsoft Intune.</span></span> <span data-ttu-id="372fe-108">No Microsoft Intune, você pode criar uma atribuição de função com várias entidades e vários escopos.</span><span class="sxs-lookup"><span data-stu-id="372fe-108">In Microsoft Intune, you can create a role assignment with multiple principals and multiple scopes.</span></span>

<span data-ttu-id="372fe-109">É necessário **fornecer directoryScopeIds** ou **appScopeIds.**</span><span class="sxs-lookup"><span data-stu-id="372fe-109">Providing either **directoryScopeIds** or **appScopeIds** is required.</span></span>

## <a name="methods"></a><span data-ttu-id="372fe-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="372fe-110">Methods</span></span>

| <span data-ttu-id="372fe-111">Método</span><span class="sxs-lookup"><span data-stu-id="372fe-111">Method</span></span>       | <span data-ttu-id="372fe-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="372fe-112">Return Type</span></span> | <span data-ttu-id="372fe-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="372fe-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="372fe-114">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-114">Get unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-get.md) | [<span data-ttu-id="372fe-115">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-115">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="372fe-116">Ler propriedades e relações do objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="372fe-116">Read properties and relationships of unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="372fe-117">Criar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-117">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="372fe-118">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-118">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="372fe-119">Crie um novo unifiedRoleAssignmentMultiple postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="372fe-119">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="372fe-120">Atualizar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-120">Update unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-update.md) | [<span data-ttu-id="372fe-121">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-121">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="372fe-122">Atualize um objeto unifiedRoleAssignmentMultiple existente.</span><span class="sxs-lookup"><span data-stu-id="372fe-122">Update an existing unifiedRoleAssignmentMultiple object.</span></span> |
| [<span data-ttu-id="372fe-123">Excluir unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="372fe-123">Delete unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-delete.md) | <span data-ttu-id="372fe-124">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="372fe-124">None</span></span> | <span data-ttu-id="372fe-125">Exclua o objeto unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="372fe-125">Delete unifiedRoleAssignmentMultiple object.</span></span> |

## <a name="properties"></a><span data-ttu-id="372fe-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="372fe-126">Properties</span></span>

| <span data-ttu-id="372fe-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="372fe-127">Property</span></span>     | <span data-ttu-id="372fe-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="372fe-128">Type</span></span>        | <span data-ttu-id="372fe-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="372fe-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="372fe-130">id</span><span class="sxs-lookup"><span data-stu-id="372fe-130">id</span></span> | <span data-ttu-id="372fe-131">String</span><span class="sxs-lookup"><span data-stu-id="372fe-131">String</span></span> | <span data-ttu-id="372fe-132">O identificador exclusivo do unifiedRoleAssignmentMultiple.</span><span class="sxs-lookup"><span data-stu-id="372fe-132">The unique identifier for the unifiedRoleAssignmentMultiple.</span></span> <span data-ttu-id="372fe-133">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="372fe-133">Key, not nullable, Read-only.</span></span> |
| <span data-ttu-id="372fe-134">displayName</span><span class="sxs-lookup"><span data-stu-id="372fe-134">displayName</span></span> | <span data-ttu-id="372fe-135">String</span><span class="sxs-lookup"><span data-stu-id="372fe-135">String</span></span> | <span data-ttu-id="372fe-136">Nome da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="372fe-136">Name of the role assignment.</span></span> <span data-ttu-id="372fe-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="372fe-137">Required.</span></span> |
| <span data-ttu-id="372fe-138">description</span><span class="sxs-lookup"><span data-stu-id="372fe-138">description</span></span> | <span data-ttu-id="372fe-139">String</span><span class="sxs-lookup"><span data-stu-id="372fe-139">String</span></span> | <span data-ttu-id="372fe-140">Descrição da atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="372fe-140">Description of the role assignment.</span></span> |
| <span data-ttu-id="372fe-141">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="372fe-141">roleDefinitionId</span></span> | <span data-ttu-id="372fe-142">String</span><span class="sxs-lookup"><span data-stu-id="372fe-142">String</span></span> | <span data-ttu-id="372fe-143">ID do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="372fe-143">ID of the unifiedRoleDefinition the assignment is for.</span></span> |
| <span data-ttu-id="372fe-144">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="372fe-144">roleDefinition</span></span> | [<span data-ttu-id="372fe-145">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="372fe-145">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) |<span data-ttu-id="372fe-146">Propriedade que indica a funçãoDefinition para a qual a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="372fe-146">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="372fe-147">Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="372fe-147">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="372fe-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="372fe-148">Read-only.</span></span>  |
| <span data-ttu-id="372fe-149">principalIds</span><span class="sxs-lookup"><span data-stu-id="372fe-149">principalIds</span></span> | <span data-ttu-id="372fe-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="372fe-150">String collection</span></span> | <span data-ttu-id="372fe-151">Objectids das entidades às quais a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="372fe-151">Objectids of the principals to which the assignment is granted.</span></span> |
| <span data-ttu-id="372fe-152">entidades de</span><span class="sxs-lookup"><span data-stu-id="372fe-152">principals</span></span>| <span data-ttu-id="372fe-153">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="372fe-153">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="372fe-154">Coleção somente leitura fazendo referência às entidades atribuídas.</span><span class="sxs-lookup"><span data-stu-id="372fe-154">Read-only collection referencing the assigned principals.</span></span> <span data-ttu-id="372fe-155">Fornecido para que os chamadores possam obter as entidades de `$expand` serviço usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="372fe-155">Provided so that callers can get the principals using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="372fe-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="372fe-156">Read-only.</span></span> |
| <span data-ttu-id="372fe-157">directoryScopeIds</span><span class="sxs-lookup"><span data-stu-id="372fe-157">directoryScopeIds</span></span> | <span data-ttu-id="372fe-158">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="372fe-158">String collection</span></span> | <span data-ttu-id="372fe-159">IDs dos objetos de diretório que representam os escopos da atribuição.</span><span class="sxs-lookup"><span data-stu-id="372fe-159">Ids of the directory objects representing the scopes of the assignment.</span></span> <span data-ttu-id="372fe-160">Os escopos de uma atribuição determinam o conjunto de recursos para os quais as entidades foram concedidas acesso.</span><span class="sxs-lookup"><span data-stu-id="372fe-160">The scopes of an assignment determine the set of resources for which the principals have been granted access.</span></span> <span data-ttu-id="372fe-161">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="372fe-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="372fe-162">Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="372fe-162">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="372fe-163">directoryScopes</span><span class="sxs-lookup"><span data-stu-id="372fe-163">directoryScopes</span></span> | <span data-ttu-id="372fe-164">Coleção [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="372fe-164">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="372fe-165">Coleção somente leitura fazendo referência aos objetos de diretório que são escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="372fe-165">Read-only collection referencing the directory objects that are scope of the assignment.</span></span> <span data-ttu-id="372fe-166">Fornecido para que os chamadores possam obter os objetos de diretório `$expand` usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="372fe-166">Provided so that callers can get the directory objects using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="372fe-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="372fe-167">Read-only.</span></span> |
| <span data-ttu-id="372fe-168">appScopeIds</span><span class="sxs-lookup"><span data-stu-id="372fe-168">appScopeIds</span></span> | <span data-ttu-id="372fe-169">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="372fe-169">String collection</span></span> | <span data-ttu-id="372fe-170">IDs dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="372fe-170">Ids of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="372fe-171">Os escopos de uma atribuição determinam o conjunto de recursos para os quais a entidade de serviço recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="372fe-171">The scopes of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="372fe-172">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="372fe-172">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="372fe-173">Use "/" para escopo em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="372fe-173">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="372fe-174">Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="372fe-174">App scopes are scopes that are defined and understood by this application only.</span></span> |
| <span data-ttu-id="372fe-175">appScopes</span><span class="sxs-lookup"><span data-stu-id="372fe-175">appScopes</span></span> | <span data-ttu-id="372fe-176">[Coleção appScope](appscope.md)</span><span class="sxs-lookup"><span data-stu-id="372fe-176">[appScope](appscope.md) collection</span></span> |<span data-ttu-id="372fe-177">Coleção somente leitura com detalhes dos escopos específicos do aplicativo quando os escopos de atribuição são específicos do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="372fe-177">Read-only collection with details of the app specific scopes when the assignment scopes are app specific.</span></span> <span data-ttu-id="372fe-178">Entidade de contenção.</span><span class="sxs-lookup"><span data-stu-id="372fe-178">Containment entity.</span></span> <span data-ttu-id="372fe-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="372fe-179">Read-only.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="372fe-180">Relações</span><span class="sxs-lookup"><span data-stu-id="372fe-180">Relationships</span></span>

<span data-ttu-id="372fe-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="372fe-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="372fe-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="372fe-182">JSON representation</span></span>

<span data-ttu-id="372fe-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="372fe-183">The following is a JSON representation of the resource.</span></span>

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


