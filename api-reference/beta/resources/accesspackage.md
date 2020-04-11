---
title: tipo de recurso accessPackage
description: Um pacote do Access define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d49ddfcc0db9b55701f0b84a223efcec85aa8dfe
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228062"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="a6345-103">tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-103">accessPackage resource type</span></span>

<span data-ttu-id="a6345-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6345-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="a6345-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="a6345-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="a6345-106">Cada pacote de acesso é referenciado por um único catálogo de pacotes do Access e tem links para os recursos desse catálogo por meio de escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="a6345-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="a6345-107">Um pacote do Access também é vinculado às diretivas de atribuição de pacote do Access, cada um deles define quem pode solicitar ou receber uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="a6345-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="a6345-108">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="a6345-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="a6345-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a6345-109">Methods</span></span>

| <span data-ttu-id="a6345-110">Método</span><span class="sxs-lookup"><span data-stu-id="a6345-110">Method</span></span>       | <span data-ttu-id="a6345-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a6345-111">Return Type</span></span> | <span data-ttu-id="a6345-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6345-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a6345-113">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="a6345-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="a6345-114">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="a6345-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="a6345-115">Recupere uma lista de objetos **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="a6345-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="a6345-116">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="a6345-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="a6345-118">Criar um novo objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="a6345-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="a6345-119">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="a6345-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="a6345-121">Ler propriedades e relações de um objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="a6345-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="a6345-122">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="a6345-122">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="a6345-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6345-123">None</span></span> | <span data-ttu-id="a6345-124">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="a6345-124">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="a6345-125">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="a6345-125">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="a6345-126">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="a6345-126">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="a6345-127">Recupere uma lista de objetos **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6345-127">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="a6345-128">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="a6345-128">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="a6345-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6345-129">None</span></span> | <span data-ttu-id="a6345-130">Crie um novo objeto **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6345-130">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="a6345-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6345-131">Properties</span></span>

| <span data-ttu-id="a6345-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6345-132">Property</span></span>     | <span data-ttu-id="a6345-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6345-133">Type</span></span>        | <span data-ttu-id="a6345-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6345-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6345-135">catalogID</span><span class="sxs-lookup"><span data-stu-id="a6345-135">catalogId</span></span>|<span data-ttu-id="a6345-136">String</span><span class="sxs-lookup"><span data-stu-id="a6345-136">String</span></span>|<span data-ttu-id="a6345-137">ID do catálogo de pacotes do Access que faz referência a esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="a6345-137">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="a6345-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-138">Read-only.</span></span>|
|<span data-ttu-id="a6345-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="a6345-139">createdBy</span></span>|<span data-ttu-id="a6345-140">String</span><span class="sxs-lookup"><span data-stu-id="a6345-140">String</span></span>|<span data-ttu-id="a6345-141">O UPN do usuário ou a identidade do assunto que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="a6345-141">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="a6345-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-142">Read-only.</span></span>|
|<span data-ttu-id="a6345-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6345-143">createdDateTime</span></span>|<span data-ttu-id="a6345-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6345-144">DateTimeOffset</span></span>|<span data-ttu-id="a6345-145">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a6345-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6345-146">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a6345-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a6345-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-147">Read-only.</span></span>|
|<span data-ttu-id="a6345-148">description</span><span class="sxs-lookup"><span data-stu-id="a6345-148">description</span></span>|<span data-ttu-id="a6345-149">String</span><span class="sxs-lookup"><span data-stu-id="a6345-149">String</span></span>|<span data-ttu-id="a6345-150">A descrição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="a6345-150">The description of the access package.</span></span>|
|<span data-ttu-id="a6345-151">displayName</span><span class="sxs-lookup"><span data-stu-id="a6345-151">displayName</span></span>|<span data-ttu-id="a6345-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a6345-152">String</span></span>|<span data-ttu-id="a6345-153">O nome de exibição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="a6345-153">The display name of the access package.</span></span>|
|<span data-ttu-id="a6345-154">id</span><span class="sxs-lookup"><span data-stu-id="a6345-154">id</span></span>|<span data-ttu-id="a6345-155">String</span><span class="sxs-lookup"><span data-stu-id="a6345-155">String</span></span>| <span data-ttu-id="a6345-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-156">Read-only.</span></span>|
|<span data-ttu-id="a6345-157">isHidden</span><span class="sxs-lookup"><span data-stu-id="a6345-157">isHidden</span></span>|<span data-ttu-id="a6345-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6345-158">Boolean</span></span>|<span data-ttu-id="a6345-159">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="a6345-159">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="a6345-160">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="a6345-160">isRoleScopesVisible</span></span>|<span data-ttu-id="a6345-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6345-161">Boolean</span></span>|<span data-ttu-id="a6345-162">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="a6345-162">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="a6345-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="a6345-163">modifiedBy</span></span>|<span data-ttu-id="a6345-164">String</span><span class="sxs-lookup"><span data-stu-id="a6345-164">String</span></span>|<span data-ttu-id="a6345-165">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a6345-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="a6345-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-166">Read-only.</span></span>|
|<span data-ttu-id="a6345-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6345-167">modifiedDateTime</span></span>|<span data-ttu-id="a6345-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6345-168">DateTimeOffset</span></span>|<span data-ttu-id="a6345-169">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a6345-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6345-170">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a6345-170">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a6345-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-171">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a6345-172">Relações</span><span class="sxs-lookup"><span data-stu-id="a6345-172">Relationships</span></span>

| <span data-ttu-id="a6345-173">Relação</span><span class="sxs-lookup"><span data-stu-id="a6345-173">Relationship</span></span> | <span data-ttu-id="a6345-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6345-174">Type</span></span>        | <span data-ttu-id="a6345-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6345-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a6345-176">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="a6345-176">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="a6345-177">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a6345-177">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="a6345-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-178">Read-only.</span></span> <span data-ttu-id="a6345-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6345-179">Nullable.</span></span>|
|<span data-ttu-id="a6345-180">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a6345-180">accessPackageCatalog</span></span>|[<span data-ttu-id="a6345-181">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="a6345-181">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="a6345-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a6345-182">Read-only.</span></span> <span data-ttu-id="a6345-183">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6345-183">Nullable.</span></span>|
|<span data-ttu-id="a6345-184">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="a6345-184">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="a6345-185">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="a6345-185">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="a6345-186">Anulável.</span><span class="sxs-lookup"><span data-stu-id="a6345-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6345-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6345-187">JSON representation</span></span>

<span data-ttu-id="a6345-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6345-188">The following is a JSON representation of the resource.</span></span>

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
