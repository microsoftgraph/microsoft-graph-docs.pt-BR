---
title: tipo de recurso accessPackage
description: Um pacote do Access define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a944309d59383b8c1501495c12d937acb13adbbb
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870978"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="12f73-103">tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-103">accessPackage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12f73-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="12f73-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="12f73-105">Cada pacote de acesso é referenciado por um único catálogo de pacotes do Access e tem links para os recursos desse catálogo por meio de escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="12f73-105">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="12f73-106">Um pacote do Access também é vinculado às diretivas de atribuição de pacote do Access, cada um deles define quem pode solicitar ou receber uma atribuição de pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="12f73-106">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="12f73-107">Para atribuir um usuário a um pacote do Access, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faça referência ao pacote do Access e à política de atribuição de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="12f73-107">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="12f73-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="12f73-108">Methods</span></span>

| <span data-ttu-id="12f73-109">Método</span><span class="sxs-lookup"><span data-stu-id="12f73-109">Method</span></span>       | <span data-ttu-id="12f73-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="12f73-110">Return Type</span></span> | <span data-ttu-id="12f73-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f73-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="12f73-112">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="12f73-112">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="12f73-113">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="12f73-113">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="12f73-114">Recupere uma lista de objetos **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="12f73-114">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="12f73-115">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-115">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="12f73-116">accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-116">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="12f73-117">Criar um novo objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="12f73-117">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="12f73-118">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-118">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="12f73-119">accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-119">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="12f73-120">Ler propriedades e relações de um objeto **accesspackage** .</span><span class="sxs-lookup"><span data-stu-id="12f73-120">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="12f73-121">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="12f73-121">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="12f73-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12f73-122">None</span></span> | <span data-ttu-id="12f73-123">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="12f73-123">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="12f73-124">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="12f73-124">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="12f73-125">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="12f73-125">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="12f73-126">Recupere uma lista de objetos **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="12f73-126">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="12f73-127">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="12f73-127">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="12f73-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12f73-128">None</span></span> | <span data-ttu-id="12f73-129">Crie um novo objeto **accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="12f73-129">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="12f73-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12f73-130">Properties</span></span>

| <span data-ttu-id="12f73-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12f73-131">Property</span></span>     | <span data-ttu-id="12f73-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="12f73-132">Type</span></span>        | <span data-ttu-id="12f73-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f73-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12f73-134">catalogID</span><span class="sxs-lookup"><span data-stu-id="12f73-134">catalogId</span></span>|<span data-ttu-id="12f73-135">String</span><span class="sxs-lookup"><span data-stu-id="12f73-135">String</span></span>|<span data-ttu-id="12f73-136">ID do catálogo de pacotes do Access que faz referência a esse pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="12f73-136">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="12f73-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-137">Read-only.</span></span>|
|<span data-ttu-id="12f73-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="12f73-138">createdBy</span></span>|<span data-ttu-id="12f73-139">String</span><span class="sxs-lookup"><span data-stu-id="12f73-139">String</span></span>|<span data-ttu-id="12f73-140">O UPN do usuário ou a identidade do assunto que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="12f73-140">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="12f73-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-141">Read-only.</span></span>|
|<span data-ttu-id="12f73-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="12f73-142">createdDateTime</span></span>|<span data-ttu-id="12f73-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f73-143">DateTimeOffset</span></span>|<span data-ttu-id="12f73-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12f73-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12f73-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12f73-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="12f73-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-146">Read-only.</span></span>|
|<span data-ttu-id="12f73-147">description</span><span class="sxs-lookup"><span data-stu-id="12f73-147">description</span></span>|<span data-ttu-id="12f73-148">String</span><span class="sxs-lookup"><span data-stu-id="12f73-148">String</span></span>|<span data-ttu-id="12f73-149">A descrição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="12f73-149">The description of the access package.</span></span>|
|<span data-ttu-id="12f73-150">displayName</span><span class="sxs-lookup"><span data-stu-id="12f73-150">displayName</span></span>|<span data-ttu-id="12f73-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="12f73-151">String</span></span>|<span data-ttu-id="12f73-152">O nome de exibição do pacote do Access.</span><span class="sxs-lookup"><span data-stu-id="12f73-152">The display name of the access package.</span></span>|
|<span data-ttu-id="12f73-153">id</span><span class="sxs-lookup"><span data-stu-id="12f73-153">id</span></span>|<span data-ttu-id="12f73-154">String</span><span class="sxs-lookup"><span data-stu-id="12f73-154">String</span></span>| <span data-ttu-id="12f73-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-155">Read-only.</span></span>|
|<span data-ttu-id="12f73-156">isHidden</span><span class="sxs-lookup"><span data-stu-id="12f73-156">isHidden</span></span>|<span data-ttu-id="12f73-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="12f73-157">Boolean</span></span>|<span data-ttu-id="12f73-158">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="12f73-158">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="12f73-159">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="12f73-159">isRoleScopesVisible</span></span>|<span data-ttu-id="12f73-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="12f73-160">Boolean</span></span>|<span data-ttu-id="12f73-161">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="12f73-161">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="12f73-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="12f73-162">modifiedBy</span></span>|<span data-ttu-id="12f73-163">String</span><span class="sxs-lookup"><span data-stu-id="12f73-163">String</span></span>|<span data-ttu-id="12f73-164">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="12f73-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="12f73-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-165">Read-only.</span></span>|
|<span data-ttu-id="12f73-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="12f73-166">modifiedDateTime</span></span>|<span data-ttu-id="12f73-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12f73-167">DateTimeOffset</span></span>|<span data-ttu-id="12f73-168">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="12f73-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="12f73-169">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="12f73-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="12f73-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-170">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="12f73-171">Relações</span><span class="sxs-lookup"><span data-stu-id="12f73-171">Relationships</span></span>

| <span data-ttu-id="12f73-172">Relação</span><span class="sxs-lookup"><span data-stu-id="12f73-172">Relationship</span></span> | <span data-ttu-id="12f73-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="12f73-173">Type</span></span>        | <span data-ttu-id="12f73-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="12f73-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="12f73-175">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="12f73-175">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="12f73-176">coleção [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="12f73-176">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="12f73-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-177">Read-only.</span></span> <span data-ttu-id="12f73-178">Anulável.</span><span class="sxs-lookup"><span data-stu-id="12f73-178">Nullable.</span></span>|
|<span data-ttu-id="12f73-179">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="12f73-179">accessPackageCatalog</span></span>|[<span data-ttu-id="12f73-180">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="12f73-180">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="12f73-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12f73-181">Read-only.</span></span> <span data-ttu-id="12f73-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="12f73-182">Nullable.</span></span>|
|<span data-ttu-id="12f73-183">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="12f73-183">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="12f73-184">coleção [accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="12f73-184">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="12f73-185">Anulável.</span><span class="sxs-lookup"><span data-stu-id="12f73-185">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12f73-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12f73-186">JSON representation</span></span>

<span data-ttu-id="12f73-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12f73-187">The following is a JSON representation of the resource.</span></span>

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
