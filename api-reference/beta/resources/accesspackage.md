---
title: Tipo de recurso accessPackage
description: Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 98e9a22137f9f6faaa39fbbb010a32b40f8f0254
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720834"
---
# <a name="accesspackage-resource-type"></a><span data-ttu-id="8219e-103">Tipo de recurso accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-103">accessPackage resource type</span></span>

<span data-ttu-id="8219e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8219e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8219e-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.</span><span class="sxs-lookup"><span data-stu-id="8219e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package defines the collections of resource roles and the policies for how one or more users can get access to those resources.</span></span>  
<span data-ttu-id="8219e-106">Cada pacote de acesso é referenciado por um catálogo de pacotes de acesso único e tem links para os recursos desse catálogo por meio dos escopos de função específicos do recurso que definem o acesso que o pacote fornece.</span><span class="sxs-lookup"><span data-stu-id="8219e-106">Each access package is referenced by a single access package catalog, and has links to the resources from that catalog via the resource-specific role scopes that define the access the package provides.</span></span>  <span data-ttu-id="8219e-107">Um pacote de acesso também se vincula às políticas de atribuição de pacote de acesso, cada uma das quais define quem pode solicitar ou ser atribuído a uma atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-107">An access package also links to the access package assignment policies, each of which define who can request or be assigned an access package assignment.</span></span>

<span data-ttu-id="8219e-108">Para atribuir um usuário a um pacote de acesso, [crie um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) que faz referência ao pacote de acesso e à política de atribuição de pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-108">To assign a user to an access package, [create an accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md) that references the access package and access package assignment policy.</span></span>

## <a name="methods"></a><span data-ttu-id="8219e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="8219e-109">Methods</span></span>

| <span data-ttu-id="8219e-110">Método</span><span class="sxs-lookup"><span data-stu-id="8219e-110">Method</span></span>       | <span data-ttu-id="8219e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8219e-111">Return Type</span></span> | <span data-ttu-id="8219e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8219e-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8219e-113">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="8219e-113">List accessPackages</span></span>](../api/accesspackage-list.md) | <span data-ttu-id="8219e-114">[Coleção accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="8219e-114">[accessPackage](accesspackage.md) collection</span></span> | <span data-ttu-id="8219e-115">Recupere uma lista de **objetos accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8219e-115">Retrieve a list of **accesspackage** objects.</span></span> |
| [<span data-ttu-id="8219e-116">Criar accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-116">Create accessPackage</span></span>](../api/accesspackage-post.md) | [<span data-ttu-id="8219e-117">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-117">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="8219e-118">Crie um novo **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8219e-118">Create a new **accesspackage** object.</span></span> |
| [<span data-ttu-id="8219e-119">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-119">Get accessPackage</span></span>](../api/accesspackage-get.md) | [<span data-ttu-id="8219e-120">accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-120">accessPackage</span></span>](accesspackage.md) | <span data-ttu-id="8219e-121">Ler propriedades e relações de um **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8219e-121">Read properties and relationships of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="8219e-122">Atualizar accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-122">Update accessPackage</span></span>](../api/accesspackage-update.md)|<span data-ttu-id="8219e-123">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8219e-123">None</span></span> | <span data-ttu-id="8219e-124">Atualize as propriedades de um **objeto accesspackage.**</span><span class="sxs-lookup"><span data-stu-id="8219e-124">Update the properties of an **accesspackage** object.</span></span> |
| [<span data-ttu-id="8219e-125">Excluir accessPackage</span><span class="sxs-lookup"><span data-stu-id="8219e-125">Delete accessPackage</span></span>](../api/accesspackage-delete.md) |<span data-ttu-id="8219e-126">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8219e-126">None</span></span> | <span data-ttu-id="8219e-127">Excluir um **accesspackage**.</span><span class="sxs-lookup"><span data-stu-id="8219e-127">Delete an **accesspackage**.</span></span> |
| [<span data-ttu-id="8219e-128">Listar accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="8219e-128">List accessPackageResourceRoleScopes</span></span>](../api/accesspackage-list-accesspackageresourcerolescopes.md) | <span data-ttu-id="8219e-129">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="8219e-129">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span> | <span data-ttu-id="8219e-130">Recupere uma lista de **objetos accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-130">Retrieve a list of **accessPackageResourceRoleScope** objects for this access package.</span></span> |
| [<span data-ttu-id="8219e-131">Criar accessPackageResourceRoleScope</span><span class="sxs-lookup"><span data-stu-id="8219e-131">Create accessPackageResourceRoleScope</span></span>](../api/accesspackage-post-accesspackageresourcerolescopes.md) |<span data-ttu-id="8219e-132">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8219e-132">None</span></span> | <span data-ttu-id="8219e-133">Crie um novo **objeto accessPackageResourceRoleScope** para este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-133">Create a new **accessPackageResourceRoleScope** object for this access package.</span></span> |

## <a name="properties"></a><span data-ttu-id="8219e-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8219e-134">Properties</span></span>

| <span data-ttu-id="8219e-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8219e-135">Property</span></span>     | <span data-ttu-id="8219e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8219e-136">Type</span></span>        | <span data-ttu-id="8219e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8219e-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8219e-138">catalogId</span><span class="sxs-lookup"><span data-stu-id="8219e-138">catalogId</span></span>|<span data-ttu-id="8219e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8219e-139">String</span></span>|<span data-ttu-id="8219e-140">ID do catálogo de pacotes de acesso referenciando este pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-140">ID of the access package catalog referencing this access package.</span></span> <span data-ttu-id="8219e-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-141">Read-only.</span></span>|
|<span data-ttu-id="8219e-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="8219e-142">createdBy</span></span>|<span data-ttu-id="8219e-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8219e-143">String</span></span>|<span data-ttu-id="8219e-144">UPN do usuário ou identidade do assunto que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="8219e-144">UPN of the user or identity of the subject who created this resource.</span></span> <span data-ttu-id="8219e-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-145">Read-only.</span></span>|
|<span data-ttu-id="8219e-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8219e-146">createdDateTime</span></span>|<span data-ttu-id="8219e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8219e-147">DateTimeOffset</span></span>|<span data-ttu-id="8219e-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8219e-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8219e-149">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8219e-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8219e-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-150">Read-only.</span></span>|
|<span data-ttu-id="8219e-151">description</span><span class="sxs-lookup"><span data-stu-id="8219e-151">description</span></span>|<span data-ttu-id="8219e-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8219e-152">String</span></span>|<span data-ttu-id="8219e-153">A descrição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-153">The description of the access package.</span></span>|
|<span data-ttu-id="8219e-154">displayName</span><span class="sxs-lookup"><span data-stu-id="8219e-154">displayName</span></span>|<span data-ttu-id="8219e-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8219e-155">String</span></span>|<span data-ttu-id="8219e-156">O nome de exibição do pacote de acesso.</span><span class="sxs-lookup"><span data-stu-id="8219e-156">The display name of the access package.</span></span>|
|<span data-ttu-id="8219e-157">id</span><span class="sxs-lookup"><span data-stu-id="8219e-157">id</span></span>|<span data-ttu-id="8219e-158">String</span><span class="sxs-lookup"><span data-stu-id="8219e-158">String</span></span>| <span data-ttu-id="8219e-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-159">Read-only.</span></span>|
|<span data-ttu-id="8219e-160">isHidden</span><span class="sxs-lookup"><span data-stu-id="8219e-160">isHidden</span></span>|<span data-ttu-id="8219e-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="8219e-161">Boolean</span></span>|<span data-ttu-id="8219e-162">Se o pacote de acesso está oculto do solicitante.</span><span class="sxs-lookup"><span data-stu-id="8219e-162">Whether the access package is hidden from the requestor.</span></span>|
|<span data-ttu-id="8219e-163">isRoleScopesVisible</span><span class="sxs-lookup"><span data-stu-id="8219e-163">isRoleScopesVisible</span></span>|<span data-ttu-id="8219e-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="8219e-164">Boolean</span></span>|<span data-ttu-id="8219e-165">Indica se os escopos de função estão visíveis.</span><span class="sxs-lookup"><span data-stu-id="8219e-165">Indicates whether role scopes are visible.</span></span>|
|<span data-ttu-id="8219e-166">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="8219e-166">modifiedBy</span></span>|<span data-ttu-id="8219e-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8219e-167">String</span></span>|<span data-ttu-id="8219e-168">O UPN do usuário que modificou esse recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8219e-168">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="8219e-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-169">Read-only.</span></span>|
|<span data-ttu-id="8219e-170">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8219e-170">modifiedDateTime</span></span>|<span data-ttu-id="8219e-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8219e-171">DateTimeOffset</span></span>|<span data-ttu-id="8219e-172">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8219e-172">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8219e-173">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8219e-173">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="8219e-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-174">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8219e-175">Relações</span><span class="sxs-lookup"><span data-stu-id="8219e-175">Relationships</span></span>

| <span data-ttu-id="8219e-176">Relação</span><span class="sxs-lookup"><span data-stu-id="8219e-176">Relationship</span></span> | <span data-ttu-id="8219e-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="8219e-177">Type</span></span>        | <span data-ttu-id="8219e-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="8219e-178">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8219e-179">accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="8219e-179">accessPackageAssignmentPolicies</span></span>|<span data-ttu-id="8219e-180">[coleção accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="8219e-180">[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) collection</span></span>| <span data-ttu-id="8219e-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-181">Read-only.</span></span> <span data-ttu-id="8219e-182">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8219e-182">Nullable.</span></span>|
|<span data-ttu-id="8219e-183">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8219e-183">accessPackageCatalog</span></span>|[<span data-ttu-id="8219e-184">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="8219e-184">accessPackageCatalog</span></span>](accesspackagecatalog.md)| <span data-ttu-id="8219e-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8219e-185">Read-only.</span></span> <span data-ttu-id="8219e-186">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8219e-186">Nullable.</span></span>|
|<span data-ttu-id="8219e-187">accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="8219e-187">accessPackageResourceRoleScopes</span></span>|<span data-ttu-id="8219e-188">[Coleção accessPackageResourceRoleScope](accesspackageresourcerolescope.md)</span><span class="sxs-lookup"><span data-stu-id="8219e-188">[accessPackageResourceRoleScope](accesspackageresourcerolescope.md) collection</span></span>| <span data-ttu-id="8219e-189">Anulável.</span><span class="sxs-lookup"><span data-stu-id="8219e-189">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8219e-190">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8219e-190">JSON representation</span></span>

<span data-ttu-id="8219e-191">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8219e-191">The following is a JSON representation of the resource.</span></span>

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


