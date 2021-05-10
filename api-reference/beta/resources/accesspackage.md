---
title: Tipo de recurso accessPackage
description: Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d288465b04986b98de7b67fa049657b8bcf0a58
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298528"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="8f27a-103">Tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-103">accessPackage resource type</span></span>

<span data-ttu-id="8f27a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f27a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f27a-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="8f27a-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  

<span data-ttu-id="8f27a-106">Cada pacote de acesso é referenciado por um catálogo de pacotes de acesso único e tem links para os recursos desse catálogo por meio dos escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="8f27a-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="8f27a-107">Um pacote de acesso também se vincula às políticas de atribuição de pacote de acesso, cada uma das quais define quem pode solicitar ou ser atribuído a uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="8f27a-108">Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="8f27a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8f27a-109">Methods</span></span>

| <span data-ttu-id="8f27a-110">Método</span><span class="sxs-lookup"><span data-stu-id="8f27a-110">Method</span></span>       | <span data-ttu-id="8f27a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8f27a-111">Return Type</span></span> | <span data-ttu-id="8f27a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f27a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8f27a-113">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="8f27a-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="8f27a-114">[Coleção accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8f27a-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="8f27a-115">Recupere uma lista de **objetos accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8f27a-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="8f27a-116">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="8f27a-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="8f27a-118">Crie um novo **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8f27a-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="8f27a-119">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="8f27a-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="8f27a-121">Ler propriedades e relações de um **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8f27a-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="8f27a-122">Atualizar accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="8f27a-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8f27a-123">None</span></span> | <span data-ttu-id="8f27a-124">Atualize as propriedades de um **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8f27a-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="8f27a-125">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="8f27a-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="8f27a-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8f27a-126">None</span></span> | <span data-ttu-id="8f27a-127">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="8f27a-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="8f27a-128">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="8f27a-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="8f27a-129">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="8f27a-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="8f27a-130">Recupere uma lista de **objetos accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="8f27a-131">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="8f27a-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="8f27a-132">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8f27a-132">None</span></span> | <span data-ttu-id="8f27a-133">Crie um novo **objeto accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |
|[<span data-ttu-id="8f27a-134">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="8f27a-134">filterByCurrentUser</span></span>](../api/accesspackage-filterbycurrentuser.md)|<span data-ttu-id="8f27a-135">[Coleção accessPackage](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8f27a-135">[accessPackage](../resources/accesspackage.md) collection</span></span>|<span data-ttu-id="8f27a-136">Recupere a lista de **objetos accessPackage** filtrados no usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="8f27a-136">Retrieve the list of **accessPackage** objects filtered on the signed-in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f27a-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f27a-137">Properties</span></span>

| <span data-ttu-id="8f27a-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f27a-138">Property</span></span>     | <span data-ttu-id="8f27a-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f27a-139">Type</span></span>        | <span data-ttu-id="8f27a-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f27a-140">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f27a-141">catalogId</span><span class="sxs-lookup"><span data-stu-id="8f27a-141">catalogId</span></span>|<span data-ttu-id="8f27a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f27a-142">String</span></span>|<span data-ttu-id="8f27a-143">ID do catálogo de pacotes de acesso referenciando este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-143">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="8f27a-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-144">Read-only.</span></span>|
|<span data-ttu-id="8f27a-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="8f27a-145">createdBy</span></span>|<span data-ttu-id="8f27a-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f27a-146">String</span></span>|<span data-ttu-id="8f27a-147">UPN do usuário ou identidade do assunto que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-147">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="8f27a-148">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-148">Read-only.</span></span>|
|<span data-ttu-id="8f27a-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f27a-149">createdDateTime</span></span>|<span data-ttu-id="8f27a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f27a-150">DateTimeOffset</span></span>|<span data-ttu-id="8f27a-151">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8f27a-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f27a-152">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8f27a-152">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8f27a-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-153">Read-only.</span></span>|
|<span data-ttu-id="8f27a-154">description</span><span class="sxs-lookup"><span data-stu-id="8f27a-154">description</span></span>|<span data-ttu-id="8f27a-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f27a-155">String</span></span>|<span data-ttu-id="8f27a-156">A descrição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-156">The description of the access package.</span></span>|
|<span data-ttu-id="8f27a-157">displayName</span><span class="sxs-lookup"><span data-stu-id="8f27a-157">displayName</span></span>|<span data-ttu-id="8f27a-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f27a-158">String</span></span>|<span data-ttu-id="8f27a-159">O nome de exibição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-159">The display name of the access package.</span></span>|
|<span data-ttu-id="8f27a-160">id</span><span class="sxs-lookup"><span data-stu-id="8f27a-160">id</span></span>|<span data-ttu-id="8f27a-161">String</span><span class="sxs-lookup"><span data-stu-id="8f27a-161">String</span></span>| <span data-ttu-id="8f27a-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-162">Read-only.</span></span>|
|<span data-ttu-id="8f27a-163">isHidden</span><span class="sxs-lookup"><span data-stu-id="8f27a-163">isHidden</span></span>|<span data-ttu-id="8f27a-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f27a-164">Boolean</span></span>|<span data-ttu-id="8f27a-165">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="8f27a-165">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="8f27a-166">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="8f27a-166">isRoleScopesVisible</span></span>|<span data-ttu-id="8f27a-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f27a-167">Boolean</span></span>|<span data-ttu-id="8f27a-168">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="8f27a-168">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="8f27a-169">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f27a-169">modifiedBy</span></span>|<span data-ttu-id="8f27a-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f27a-170">String</span></span>|<span data-ttu-id="8f27a-171">O UPN do usuário que modificou esse recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8f27a-171">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="8f27a-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-172">Read-only.</span></span>|
|<span data-ttu-id="8f27a-173">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f27a-173">modifiedDateTime</span></span>|<span data-ttu-id="8f27a-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f27a-174">DateTimeOffset</span></span>|<span data-ttu-id="8f27a-175">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8f27a-175">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f27a-176">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8f27a-176">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8f27a-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f27a-177">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f27a-178">Relações</span><span class="sxs-lookup"><span data-stu-id="8f27a-178">Relationships</span></span>

| <span data-ttu-id="8f27a-179">Relação</span><span class="sxs-lookup"><span data-stu-id="8f27a-179">Relationship</span></span> | <span data-ttu-id="8f27a-180">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f27a-180">Type</span></span>        | <span data-ttu-id="8f27a-181">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f27a-181">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f27a-182">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="8f27a-182">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="8f27a-183">[coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8f27a-183">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="8f27a-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8f27a-p107">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8f27a-186">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8f27a-186">accessPackageCatalog</span></span>|[<span data-ttu-id="8f27a-187">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8f27a-187">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="8f27a-p108">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="8f27a-p108">Read-only. Nullable.</span></span>|
|<span data-ttu-id="8f27a-190">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="8f27a-190">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="8f27a-191">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="8f27a-191">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="8f27a-192">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8f27a-192">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f27a-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f27a-193">JSON representation</span></span>

<span data-ttu-id="8f27a-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f27a-194">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackage",
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


