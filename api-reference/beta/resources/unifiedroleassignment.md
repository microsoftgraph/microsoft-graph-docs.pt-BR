---
title: tipo de recurso unifiedRoleAssignment
description: Uma atribuição de função é o vínculo entre uma definição de função e uma entidade de segurança em um escopo específico para o propósito de conceder acesso.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf08510d15f661f98365fe0346eb72b9b6d7b0bf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985626"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="e6067-103">tipo de recurso unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="e6067-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6067-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6067-105">Um unifiedRoleAssignment é usado para conceder acesso aos recursos.</span><span class="sxs-lookup"><span data-stu-id="e6067-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="e6067-106">Ele representa uma definição de função atribuída a uma entidade de segurança (normalmente um usuário) em um determinado escopo.</span><span class="sxs-lookup"><span data-stu-id="e6067-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

<span data-ttu-id="e6067-107">O fornecimento de um directoryScopeId ou um appScopeId é necessário.</span><span class="sxs-lookup"><span data-stu-id="e6067-107">Providing either a directoryScopeId or an appScopeId is required.</span></span>

## <a name="methods"></a><span data-ttu-id="e6067-108">Methods</span><span class="sxs-lookup"><span data-stu-id="e6067-108">Methods</span></span>

| <span data-ttu-id="e6067-109">Método</span><span class="sxs-lookup"><span data-stu-id="e6067-109">Method</span></span>       | <span data-ttu-id="e6067-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e6067-110">Return Type</span></span> | <span data-ttu-id="e6067-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6067-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e6067-112">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-112">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="e6067-113">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-113">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="e6067-114">Leia as propriedades e os relacionamentos do objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="e6067-114">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="e6067-115">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-115">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="e6067-116">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-116">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="e6067-117">Crie um novo unifiedRoleAssignment postando na coleção roleAssignment.</span><span class="sxs-lookup"><span data-stu-id="e6067-117">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="e6067-118">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e6067-118">Delete unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="e6067-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6067-119">None</span></span> | <span data-ttu-id="e6067-120">Exclua o objeto unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="e6067-120">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6067-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6067-121">Properties</span></span>

| <span data-ttu-id="e6067-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6067-122">Property</span></span>     | <span data-ttu-id="e6067-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6067-123">Type</span></span>        | <span data-ttu-id="e6067-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6067-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6067-125">id</span><span class="sxs-lookup"><span data-stu-id="e6067-125">id</span></span>|<span data-ttu-id="e6067-126">String</span><span class="sxs-lookup"><span data-stu-id="e6067-126">String</span></span>| <span data-ttu-id="e6067-127">O identificador exclusivo para o unifiedRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="e6067-127">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="e6067-128">Chave, não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6067-128">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="e6067-129">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="e6067-129">roleDefinitionId</span></span>|<span data-ttu-id="e6067-130">String</span><span class="sxs-lookup"><span data-stu-id="e6067-130">String</span></span>| <span data-ttu-id="e6067-131">ID do unifiedRoleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="e6067-131">ID of the unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="e6067-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6067-132">Read only.</span></span> |
|<span data-ttu-id="e6067-133">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6067-133">roleDefinition</span></span>|[<span data-ttu-id="e6067-134">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e6067-134">unifiedRoleDefinition</span></span>](unifiedroledefinition.md)|<span data-ttu-id="e6067-135">Propriedade que indica o roleDefinition para o qual a atribuição é.</span><span class="sxs-lookup"><span data-stu-id="e6067-135">Property indicating the roleDefinition the assignment is for.</span></span> <span data-ttu-id="e6067-136">Fornecido de modo que os chamadores possam obter a definição de função usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e6067-136">Provided so that callers can get the role definition using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="e6067-137">roleDefinition.Id será expandido automaticamente</span><span class="sxs-lookup"><span data-stu-id="e6067-137">roleDefinition.Id will be auto expanded</span></span>
|<span data-ttu-id="e6067-138">principalId</span><span class="sxs-lookup"><span data-stu-id="e6067-138">principalId</span></span>|<span data-ttu-id="e6067-139">String</span><span class="sxs-lookup"><span data-stu-id="e6067-139">String</span></span>| <span data-ttu-id="e6067-140">ObjectID da entidade de segurança para a qual a atribuição é concedida.</span><span class="sxs-lookup"><span data-stu-id="e6067-140">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="e6067-141">requere</span><span class="sxs-lookup"><span data-stu-id="e6067-141">principal</span></span>|[<span data-ttu-id="e6067-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e6067-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="e6067-143">Propriedade que faz referência à entidade de segurança atribuída.</span><span class="sxs-lookup"><span data-stu-id="e6067-143">Property referencing the assigned principal.</span></span> <span data-ttu-id="e6067-144">Desde que os chamadores possam obter a entidade de segurança usando `$expand` ao mesmo tempo que obter a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e6067-144">Provided so that callers can get the principal using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="e6067-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6067-145">Read-only.</span></span> |
|<span data-ttu-id="e6067-146">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="e6067-146">directoryScopeId</span></span>|<span data-ttu-id="e6067-147">String</span><span class="sxs-lookup"><span data-stu-id="e6067-147">String</span></span>|<span data-ttu-id="e6067-148">ID do objeto de diretório que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e6067-148">Id of the directory object representing the scope of the assignment.</span></span> <span data-ttu-id="e6067-149">O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="e6067-149">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e6067-150">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e6067-150">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="e6067-151">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="e6067-151">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="e6067-152">directoryScope</span><span class="sxs-lookup"><span data-stu-id="e6067-152">directoryScope</span></span>|[<span data-ttu-id="e6067-153">directoryObject</span><span class="sxs-lookup"><span data-stu-id="e6067-153">directoryObject</span></span>](directoryobject.md)|<span data-ttu-id="e6067-154">Propriedade fazendo referência ao objeto Directory que é o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="e6067-154">Property referencing the directory object that is the scope of the assignment.</span></span> <span data-ttu-id="e6067-155">Fornecido de modo que os chamadores possam obter o objeto de diretório usando `$expand` ao mesmo tempo em que se obtém a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="e6067-155">Provided so that callers can get the directory object using `$expand` at the same time as getting the role assignment.</span></span> <span data-ttu-id="e6067-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6067-156">Read-only.</span></span> |
|<span data-ttu-id="e6067-157">appScopeId</span><span class="sxs-lookup"><span data-stu-id="e6067-157">appScopeId</span></span>|<span data-ttu-id="e6067-158">String</span><span class="sxs-lookup"><span data-stu-id="e6067-158">String</span></span>|<span data-ttu-id="e6067-159">ID do escopo específico do aplicativo quando o escopo da atribuição é específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6067-159">Id of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="e6067-160">O escopo de uma atribuição determina o conjunto de recursos para o qual a entidade recebeu acesso.</span><span class="sxs-lookup"><span data-stu-id="e6067-160">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="e6067-161">Escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e6067-161">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="e6067-162">Use "/" para escopo em todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6067-162">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="e6067-163">Os escopos de aplicativo são escopos definidos e compreendidos por esse aplicativo apenas.</span><span class="sxs-lookup"><span data-stu-id="e6067-163">App scopes are scopes that are defined and understood by this application only.</span></span>|
|<span data-ttu-id="e6067-164">appScope</span><span class="sxs-lookup"><span data-stu-id="e6067-164">appScope</span></span>|[<span data-ttu-id="e6067-165">appScope</span><span class="sxs-lookup"><span data-stu-id="e6067-165">appScope</span></span>](appscope.md)|<span data-ttu-id="e6067-166">Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo da atribuição é específico de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e6067-166">Read-only property with details of the app specific scope when the assignment scope is app specific.</span></span> <span data-ttu-id="e6067-167">Entidade de confinamento.</span><span class="sxs-lookup"><span data-stu-id="e6067-167">Containment entity.</span></span> |
|<span data-ttu-id="e6067-168">resourceScope</span><span class="sxs-lookup"><span data-stu-id="e6067-168">resourceScope</span></span>|<span data-ttu-id="e6067-169">String</span><span class="sxs-lookup"><span data-stu-id="e6067-169">String</span></span>| <span data-ttu-id="e6067-170">O escopo no qual o unifiedRoleAssignment se aplica.</span><span class="sxs-lookup"><span data-stu-id="e6067-170">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="e6067-171">Isso é "/" para todo o serviço.</span><span class="sxs-lookup"><span data-stu-id="e6067-171">This is "/" for service-wide.</span></span> <span data-ttu-id="e6067-172">**NÃO USE. Essa propriedade será preterida em breve.**</span><span class="sxs-lookup"><span data-stu-id="e6067-172">**DO NOT USE. This property will be deprecated soon.**</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6067-173">Relações</span><span class="sxs-lookup"><span data-stu-id="e6067-173">Relationships</span></span>

<span data-ttu-id="e6067-174">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6067-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6067-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6067-175">JSON representation</span></span>

<span data-ttu-id="e6067-176">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6067-176">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
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

