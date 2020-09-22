---
title: tipo de recurso accessPackage
description: Um pacote do Access define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e8603904e2a1cdb6315c1f7b5264e461cfdff09b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48031785"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="73e81-103">tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-103">accessPackage resource type</span></span>

<span data-ttu-id="73e81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73e81-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="73e81-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="73e81-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="73e81-106">Cada pacote de acesso é referenciado por um único catálogo de pacotes do Access e tem links para os recursos desse catálogo por meio de escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="73e81-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="73e81-107">Um pacote do Access também é vinculado às diretivas de atribuição de pacote do Access, cada um deles define quem pode solicitar ou receber uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="73e81-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="73e81-108">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="73e81-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="73e81-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="73e81-109">Methods</span></span>

| <span data-ttu-id="73e81-110">Método</span><span class="sxs-lookup"><span data-stu-id="73e81-110">Method</span></span>       | <span data-ttu-id="73e81-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73e81-111">Return Type</span></span> | <span data-ttu-id="73e81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e81-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="73e81-113">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="73e81-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="73e81-114">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="73e81-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="73e81-115">Recupere uma lista de objetos **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="73e81-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="73e81-116">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="73e81-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="73e81-118">Criar um novo objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="73e81-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="73e81-119">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="73e81-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="73e81-121">Ler propriedades e relações de um objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="73e81-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="73e81-122">Atualizar accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="73e81-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73e81-123">None</span></span> | <span data-ttu-id="73e81-124">Atualiza as propriedades de um objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="73e81-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="73e81-125">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="73e81-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="73e81-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73e81-126">None</span></span> | <span data-ttu-id="73e81-127">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="73e81-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="73e81-128">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="73e81-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="73e81-129">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="73e81-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="73e81-130">Recupere uma lista de objetos **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="73e81-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="73e81-131">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="73e81-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="73e81-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73e81-132">None</span></span> | <span data-ttu-id="73e81-133">Crie um novo objeto **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="73e81-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="73e81-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73e81-134">Properties</span></span>

| <span data-ttu-id="73e81-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73e81-135">Property</span></span>     | <span data-ttu-id="73e81-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="73e81-136">Type</span></span>        | <span data-ttu-id="73e81-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e81-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73e81-138">catalogID</span><span class="sxs-lookup"><span data-stu-id="73e81-138">catalogId</span></span>|<span data-ttu-id="73e81-139">String</span><span class="sxs-lookup"><span data-stu-id="73e81-139">String</span></span>|<span data-ttu-id="73e81-140">ID do catálogo de pacotes do Access que faz referência a esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="73e81-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="73e81-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-141">Read-only.</span></span>|
|<span data-ttu-id="73e81-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="73e81-142">createdBy</span></span>|<span data-ttu-id="73e81-143">String</span><span class="sxs-lookup"><span data-stu-id="73e81-143">String</span></span>|<span data-ttu-id="73e81-144">O UPN do usuário ou a identidade do assunto que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="73e81-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="73e81-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-145">Read-only.</span></span>|
|<span data-ttu-id="73e81-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73e81-146">createdDateTime</span></span>|<span data-ttu-id="73e81-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73e81-147">DateTimeOffset</span></span>|<span data-ttu-id="73e81-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="73e81-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73e81-149">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="73e81-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="73e81-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-150">Read-only.</span></span>|
|<span data-ttu-id="73e81-151">description</span><span class="sxs-lookup"><span data-stu-id="73e81-151">description</span></span>|<span data-ttu-id="73e81-152">String</span><span class="sxs-lookup"><span data-stu-id="73e81-152">String</span></span>|<span data-ttu-id="73e81-153">A descrição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="73e81-153">The description of the access package.</span></span>|
|<span data-ttu-id="73e81-154">displayName</span><span class="sxs-lookup"><span data-stu-id="73e81-154">displayName</span></span>|<span data-ttu-id="73e81-155">String</span><span class="sxs-lookup"><span data-stu-id="73e81-155">String</span></span>|<span data-ttu-id="73e81-156">O nome de exibição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="73e81-156">The display name of the access package.</span></span>|
|<span data-ttu-id="73e81-157">id</span><span class="sxs-lookup"><span data-stu-id="73e81-157">id</span></span>|<span data-ttu-id="73e81-158">String</span><span class="sxs-lookup"><span data-stu-id="73e81-158">String</span></span>| <span data-ttu-id="73e81-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-159">Read-only.</span></span>|
|<span data-ttu-id="73e81-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="73e81-160">isHidden</span></span>|<span data-ttu-id="73e81-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="73e81-161">Boolean</span></span>|<span data-ttu-id="73e81-162">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="73e81-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="73e81-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="73e81-163">isRoleScopesVisible</span></span>|<span data-ttu-id="73e81-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="73e81-164">Boolean</span></span>|<span data-ttu-id="73e81-165">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="73e81-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="73e81-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="73e81-166">modifiedBy</span></span>|<span data-ttu-id="73e81-167">String</span><span class="sxs-lookup"><span data-stu-id="73e81-167">String</span></span>|<span data-ttu-id="73e81-168">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73e81-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="73e81-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-169">Read-only.</span></span>|
|<span data-ttu-id="73e81-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73e81-170">modifiedDateTime</span></span>|<span data-ttu-id="73e81-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73e81-171">DateTimeOffset</span></span>|<span data-ttu-id="73e81-172">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="73e81-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73e81-173">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="73e81-173">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="73e81-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="73e81-175">Relações</span><span class="sxs-lookup"><span data-stu-id="73e81-175">Relationships</span></span>

| <span data-ttu-id="73e81-176">Relação</span><span class="sxs-lookup"><span data-stu-id="73e81-176">Relationship</span></span> | <span data-ttu-id="73e81-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="73e81-177">Type</span></span>        | <span data-ttu-id="73e81-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e81-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73e81-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="73e81-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="73e81-180">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="73e81-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="73e81-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-181">Read-only.</span></span> <span data-ttu-id="73e81-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73e81-182">Nullable.</span></span>|
|<span data-ttu-id="73e81-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="73e81-183">accessPackageCatalog</span></span>|[<span data-ttu-id="73e81-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="73e81-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="73e81-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73e81-185">Read-only.</span></span> <span data-ttu-id="73e81-186">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73e81-186">Nullable.</span></span>|
|<span data-ttu-id="73e81-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="73e81-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="73e81-188">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="73e81-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="73e81-189">Anulável.</span><span class="sxs-lookup"><span data-stu-id="73e81-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73e81-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73e81-190">JSON representation</span></span>

<span data-ttu-id="73e81-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73e81-191">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


