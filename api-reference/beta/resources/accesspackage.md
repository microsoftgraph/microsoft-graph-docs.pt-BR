---
title: tipo de recurso accessPackage
description: Um pacote do Access define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e4d7565cdb16eb2a6a0abb7a33344c70490e2616
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939219"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="859fa-103">tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-103">accessPackage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="859fa-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="859fa-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="859fa-105">Cada pacote de acesso é referenciado por um único catálogo de pacotes do Access e tem links para os recursos desse catálogo por meio de escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="859fa-105">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="859fa-106">Um pacote do Access também é vinculado às diretivas de atribuição de pacote do Access, cada um deles define quem pode solicitar ou receber uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="859fa-106">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="859fa-107">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="859fa-107">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="859fa-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="859fa-108">Methods</span></span>

| <span data-ttu-id="859fa-109">Método</span><span class="sxs-lookup"><span data-stu-id="859fa-109">Method</span></span>       | <span data-ttu-id="859fa-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="859fa-110">Return Type</span></span> | <span data-ttu-id="859fa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="859fa-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="859fa-112">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="859fa-112">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="859fa-113">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="859fa-113">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="859fa-114">Recupere uma lista de objetos **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="859fa-114">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="859fa-115">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-115">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="859fa-116">accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-116">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="859fa-117">Criar um novo objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="859fa-117">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="859fa-118">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-118">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="859fa-119">accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-119">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="859fa-120">Ler propriedades e relações de um objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="859fa-120">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="859fa-121">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="859fa-121">Delete accessPackage</span></span>](../api/accesspackage-delete.md) | | <span data-ttu-id="859fa-122">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="859fa-122">Delete an **accesspackage**.</span></span> |

## <a name="properties"></a><span data-ttu-id="859fa-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="859fa-123">Properties</span></span>

| <span data-ttu-id="859fa-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="859fa-124">Property</span></span>     | <span data-ttu-id="859fa-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="859fa-125">Type</span></span>        | <span data-ttu-id="859fa-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="859fa-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="859fa-127">catalogID</span><span class="sxs-lookup"><span data-stu-id="859fa-127">catalogId</span></span>|<span data-ttu-id="859fa-128">String</span><span class="sxs-lookup"><span data-stu-id="859fa-128">String</span></span>|<span data-ttu-id="859fa-129">ID do catálogo de pacotes do Access que faz referência a esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="859fa-129">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="859fa-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-130">Read-only.</span></span>|
|<span data-ttu-id="859fa-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="859fa-131">createdBy</span></span>|<span data-ttu-id="859fa-132">String</span><span class="sxs-lookup"><span data-stu-id="859fa-132">String</span></span>|<span data-ttu-id="859fa-133">O UPN do usuário ou a identidade do assunto que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="859fa-133">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="859fa-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-134">Read-only.</span></span>|
|<span data-ttu-id="859fa-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="859fa-135">createdDateTime</span></span>|<span data-ttu-id="859fa-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="859fa-136">DateTimeOffset</span></span>|<span data-ttu-id="859fa-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="859fa-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="859fa-138">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="859fa-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="859fa-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-139">Read-only.</span></span>|
|<span data-ttu-id="859fa-140">description</span><span class="sxs-lookup"><span data-stu-id="859fa-140">description</span></span>|<span data-ttu-id="859fa-141">String</span><span class="sxs-lookup"><span data-stu-id="859fa-141">String</span></span>|<span data-ttu-id="859fa-142">A descrição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="859fa-142">The description of the access package.</span></span>|
|<span data-ttu-id="859fa-143">displayName</span><span class="sxs-lookup"><span data-stu-id="859fa-143">displayName</span></span>|<span data-ttu-id="859fa-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="859fa-144">String</span></span>|<span data-ttu-id="859fa-145">O nome de exibição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="859fa-145">The display name of the access package.</span></span>|
|<span data-ttu-id="859fa-146">id</span><span class="sxs-lookup"><span data-stu-id="859fa-146">id</span></span>|<span data-ttu-id="859fa-147">String</span><span class="sxs-lookup"><span data-stu-id="859fa-147">String</span></span>| <span data-ttu-id="859fa-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-148">Read-only.</span></span>|
|<span data-ttu-id="859fa-149">isHidden</span><span class="sxs-lookup"><span data-stu-id="859fa-149">isHidden</span></span>|<span data-ttu-id="859fa-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="859fa-150">Boolean</span></span>|<span data-ttu-id="859fa-151">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="859fa-151">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="859fa-152">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="859fa-152">isRoleScopesVisible</span></span>|<span data-ttu-id="859fa-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="859fa-153">Boolean</span></span>|<span data-ttu-id="859fa-154">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="859fa-154">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="859fa-155">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="859fa-155">modifiedBy</span></span>|<span data-ttu-id="859fa-156">String</span><span class="sxs-lookup"><span data-stu-id="859fa-156">String</span></span>|<span data-ttu-id="859fa-157">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="859fa-157">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="859fa-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-158">Read-only.</span></span>|
|<span data-ttu-id="859fa-159">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="859fa-159">modifiedDateTime</span></span>|<span data-ttu-id="859fa-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="859fa-160">DateTimeOffset</span></span>|<span data-ttu-id="859fa-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="859fa-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="859fa-162">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="859fa-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="859fa-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-163">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="859fa-164">Relações</span><span class="sxs-lookup"><span data-stu-id="859fa-164">Relationships</span></span>

| <span data-ttu-id="859fa-165">Relação</span><span class="sxs-lookup"><span data-stu-id="859fa-165">Relationship</span></span> | <span data-ttu-id="859fa-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="859fa-166">Type</span></span>        | <span data-ttu-id="859fa-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="859fa-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="859fa-168">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="859fa-168">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="859fa-169">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="859fa-169">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="859fa-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-170">Read-only.</span></span> <span data-ttu-id="859fa-171">Anulável.</span><span class="sxs-lookup"><span data-stu-id="859fa-171">Nullable.</span></span>|
|<span data-ttu-id="859fa-172">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="859fa-172">accessPackageCatalog</span></span>|[<span data-ttu-id="859fa-173">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="859fa-173">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="859fa-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="859fa-174">Read-only.</span></span> <span data-ttu-id="859fa-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="859fa-175">Nullable.</span></span>|
|<span data-ttu-id="859fa-176">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="859fa-176">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="859fa-177">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="859fa-177">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="859fa-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="859fa-178">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="859fa-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="859fa-179">JSON representation</span></span>

<span data-ttu-id="859fa-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="859fa-180">The following is a JSON representation of the resource.</span></span>

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
