---
title: Tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de serviço em um escopo específico para fins de concessão de acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4dc0ec6bb692c88d2b01a440bae1d7789bd042a5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159021"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="85e20-103">Tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="85e20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85e20-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85e20-105">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="85e20-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="85e20-106">Ele representa uma definição de função atribuída a uma entidade de segurança (normalmente um usuário) em um escopo específico.</span><span class="sxs-lookup"><span data-stu-id="85e20-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="85e20-107">É necessário fornecer um directoryScopeId ou um appScopeId.</span><span class="sxs-lookup"><span data-stu-id="85e20-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="85e20-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="85e20-108">Methods</span></span>

| <span data-ttu-id="85e20-109">Método</span><span class="sxs-lookup"><span data-stu-id="85e20-109">Method</span></span>       | <span data-ttu-id="85e20-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85e20-110">Return Type</span></span> | <span data-ttu-id="85e20-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85e20-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="85e20-112">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="85e20-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="85e20-114">Ler propriedades e relações do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="85e20-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="85e20-115">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="85e20-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="85e20-117">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="85e20-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="85e20-118">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="85e20-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="85e20-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="85e20-119">None</span></span> | <span data-ttu-id="85e20-120">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="85e20-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85e20-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85e20-121">Properties</span></span>

| <span data-ttu-id="85e20-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85e20-122">Property</span></span>     | <span data-ttu-id="85e20-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="85e20-123">Type</span></span>        | <span data-ttu-id="85e20-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="85e20-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85e20-125">id</span><span class="sxs-lookup"><span data-stu-id="85e20-125">id</span></span>|<span data-ttu-id="85e20-126">String</span><span class="sxs-lookup"><span data-stu-id="85e20-126">String</span></span>| <span data-ttu-id="85e20-127">O identificador exclusivo do unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="85e20-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="85e20-128">Chave, não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85e20-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="85e20-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="85e20-129">roleDefinitionId</span></span>|<span data-ttu-id="85e20-130">String</span><span class="sxs-lookup"><span data-stu-id="85e20-130">String</span></span>| <span data-ttu-id="85e20-131">ID do unifiedRoleDefinition para o que a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="85e20-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="85e20-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85e20-132">Read only.</span></span> |
|<span data-ttu-id="85e20-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="85e20-133">roleDefinition</span></span>|[<span data-ttu-id="85e20-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="85e20-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="85e20-135">Propriedade que indica a funçãoDefinition para a qual a atribuição se destina.</span><span class="sxs-lookup"><span data-stu-id="85e20-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="85e20-136">Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="85e20-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="85e20-137">roleDefinition.Id será expandido automaticamente</span><span class="sxs-lookup"><span data-stu-id="85e20-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="85e20-138">principalId</span><span class="sxs-lookup"><span data-stu-id="85e20-138">principalId</span></span>|<span data-ttu-id="85e20-139">String</span><span class="sxs-lookup"><span data-stu-id="85e20-139">String</span></span>| <span data-ttu-id="85e20-140">Objectid da entidade à qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="85e20-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="85e20-141">principal</span><span class="sxs-lookup"><span data-stu-id="85e20-141">principal</span></span>|[<span data-ttu-id="85e20-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="85e20-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="85e20-143">Propriedade que se refere à entidade atribuída.</span><span class="sxs-lookup"><span data-stu-id="85e20-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="85e20-144">Fornecido para que os chamadores possam obter a entidade de `$expand` serviço usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="85e20-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="85e20-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85e20-145">Read-only.</span></span> |
|<span data-ttu-id="85e20-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="85e20-146">directoryScopeId</span></span>|<span data-ttu-id="85e20-147">String</span><span class="sxs-lookup"><span data-stu-id="85e20-147">String</span></span>|<span data-ttu-id="85e20-148">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="85e20-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="85e20-149">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade de serviço recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="85e20-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="85e20-150">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="85e20-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="85e20-151">Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85e20-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="85e20-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="85e20-152">directoryScope</span></span>|[<span data-ttu-id="85e20-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="85e20-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="85e20-154">Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="85e20-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="85e20-155">Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="85e20-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="85e20-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85e20-156">Read-only.</span></span> |
|<span data-ttu-id="85e20-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="85e20-157">appScopeId</span></span>|<span data-ttu-id="85e20-158">String</span><span class="sxs-lookup"><span data-stu-id="85e20-158">String</span></span>|<span data-ttu-id="85e20-159">ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85e20-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="85e20-160">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade de serviço recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="85e20-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="85e20-161">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="85e20-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="85e20-162">Use "/" para escopo em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="85e20-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="85e20-163">Escopos de aplicativo são escopos definidos e compreendidos apenas por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85e20-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="85e20-164">appScope</span><span class="sxs-lookup"><span data-stu-id="85e20-164">appScope</span></span>|[<span data-ttu-id="85e20-165">appScope</span><span class="sxs-lookup"><span data-stu-id="85e20-165">appScope</span></span>](appscope.md)|<span data-ttu-id="85e20-166">Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="85e20-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="85e20-167">Entidade de contenção.</span><span class="sxs-lookup"><span data-stu-id="85e20-167">Containment entity.</span></span> |
|<span data-ttu-id="85e20-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="85e20-168">resourceScope</span></span>|<span data-ttu-id="85e20-169">String</span><span class="sxs-lookup"><span data-stu-id="85e20-169">String</span></span>| <span data-ttu-id="85e20-170">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="85e20-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="85e20-171">Isso é "/" para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="85e20-171">This is "/" for service-wide.</span></span> <span data-ttu-id="85e20-172">**NÃO USE. Essa propriedade será preterida em breve.**</span><span class="sxs-lookup"><span data-stu-id="85e20-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="85e20-173">Relações</span><span class="sxs-lookup"><span data-stu-id="85e20-173">Relationships</span></span>

<span data-ttu-id="85e20-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85e20-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e20-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85e20-175">JSON representation</span></span>

<span data-ttu-id="85e20-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85e20-176">The following is a JSON representation of the resource.</span></span>

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

