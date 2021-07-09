---
title: Tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes de acesso é um contêiner para pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 051657b5c8c7edb51a4c2c5c3a15bf3740052b86
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351094"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="c5f40-103">Tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="c5f40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5f40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5f40-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um catálogo de pacotes de acesso é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span> <span data-ttu-id="c5f40-106">Um catálogo de pacotes de acesso também pode ter recursos vinculados usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span> <span data-ttu-id="c5f40-107">Para exibir ou alterar a associação de funções com escopo de catálogo, use a [API](unifiedroleassignment.md) de atribuições de função com o provedor RBAC de gerenciamento de direitos.</span><span class="sxs-lookup"><span data-stu-id="c5f40-107">To view or change the membership of catalog-scoped roles, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>



## <a name="methods"></a><span data-ttu-id="c5f40-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5f40-108">Methods</span></span>

| <span data-ttu-id="c5f40-109">Método</span><span class="sxs-lookup"><span data-stu-id="c5f40-109">Method</span></span>       | <span data-ttu-id="c5f40-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5f40-110">Return Type</span></span> | <span data-ttu-id="c5f40-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f40-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c5f40-112">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="c5f40-112">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="c5f40-113">[Coleção accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="c5f40-113">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="c5f40-114">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="c5f40-114">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="c5f40-115">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-115">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="c5f40-116">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-116">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="c5f40-117">Crie um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="c5f40-117">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="c5f40-118">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-118">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="c5f40-119">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-119">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="c5f40-120">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="c5f40-120">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="c5f40-121">Atualizar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-121">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="c5f40-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c5f40-122">None</span></span> | <span data-ttu-id="c5f40-123">Atualize as propriedades de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="c5f40-123">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="c5f40-124">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-124">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="c5f40-125">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="c5f40-125">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="c5f40-126">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-126">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="c5f40-127">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="c5f40-127">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="c5f40-128">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="c5f40-128">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="c5f40-129">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="c5f40-129">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="c5f40-130">[Coleção accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="c5f40-130">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="c5f40-131">Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="c5f40-131">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5f40-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5f40-132">Properties</span></span>

| <span data-ttu-id="c5f40-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5f40-133">Property</span></span>     | <span data-ttu-id="c5f40-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f40-134">Type</span></span>        | <span data-ttu-id="c5f40-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f40-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5f40-136">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="c5f40-136">catalogStatus</span></span>|<span data-ttu-id="c5f40-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-137">String</span></span>|<span data-ttu-id="c5f40-138">Tem o valor `Published` se os pacotes de acesso estão disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="c5f40-138">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="c5f40-139">catalogType</span><span class="sxs-lookup"><span data-stu-id="c5f40-139">catalogType</span></span>|<span data-ttu-id="c5f40-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-140">String</span></span>|<span data-ttu-id="c5f40-141">Um dos `UserManaged` ou `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="c5f40-141">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="c5f40-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="c5f40-142">createdBy</span></span>|<span data-ttu-id="c5f40-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-143">String</span></span>|<span data-ttu-id="c5f40-144">UPN do usuário que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-144">UPN of the user who created this resource.</span></span> <span data-ttu-id="c5f40-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-145">Read-only.</span></span>|
|<span data-ttu-id="c5f40-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f40-146">createdDateTime</span></span>|<span data-ttu-id="c5f40-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f40-147">DateTimeOffset</span></span>|<span data-ttu-id="c5f40-148">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c5f40-148">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5f40-149">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c5f40-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c5f40-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-150">Read-only.</span></span>|
|<span data-ttu-id="c5f40-151">description</span><span class="sxs-lookup"><span data-stu-id="c5f40-151">description</span></span>|<span data-ttu-id="c5f40-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-152">String</span></span>|<span data-ttu-id="c5f40-153">A descrição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-153">The description of the access package catalog.</span></span>|
|<span data-ttu-id="c5f40-154">displayName</span><span class="sxs-lookup"><span data-stu-id="c5f40-154">displayName</span></span>|<span data-ttu-id="c5f40-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-155">String</span></span>|<span data-ttu-id="c5f40-156">O nome de exibição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-156">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="c5f40-157">id</span><span class="sxs-lookup"><span data-stu-id="c5f40-157">id</span></span>|<span data-ttu-id="c5f40-158">String</span><span class="sxs-lookup"><span data-stu-id="c5f40-158">String</span></span>| <span data-ttu-id="c5f40-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-159">Read-only.</span></span>|
|<span data-ttu-id="c5f40-160">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="c5f40-160">isExternallyVisible</span></span>|<span data-ttu-id="c5f40-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="c5f40-161">Boolean</span></span>|<span data-ttu-id="c5f40-162">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="c5f40-162">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="c5f40-163">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="c5f40-163">modifiedBy</span></span>|<span data-ttu-id="c5f40-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5f40-164">String</span></span>|<span data-ttu-id="c5f40-165">O UPN do usuário que modificou esse recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="c5f40-165">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="c5f40-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-166">Read-only.</span></span>|
|<span data-ttu-id="c5f40-167">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5f40-167">modifiedDateTime</span></span>|<span data-ttu-id="c5f40-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5f40-168">DateTimeOffset</span></span>|<span data-ttu-id="c5f40-169">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="c5f40-169">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c5f40-170">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c5f40-170">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="c5f40-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-171">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="c5f40-172">Relações</span><span class="sxs-lookup"><span data-stu-id="c5f40-172">Relationships</span></span>

| <span data-ttu-id="c5f40-173">Relação</span><span class="sxs-lookup"><span data-stu-id="c5f40-173">Relationship</span></span> | <span data-ttu-id="c5f40-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5f40-174">Type</span></span>        | <span data-ttu-id="c5f40-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5f40-175">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c5f40-176">accessPackages</span><span class="sxs-lookup"><span data-stu-id="c5f40-176">accessPackages</span></span>|<span data-ttu-id="c5f40-177">[Coleção accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="c5f40-177">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="c5f40-178">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="c5f40-178">The access packages in this catalog.</span></span> <span data-ttu-id="c5f40-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5f40-179">Read-only.</span></span> <span data-ttu-id="c5f40-180">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c5f40-180">Nullable.</span></span>|
|<span data-ttu-id="c5f40-181">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="c5f40-181">accessPackageResources</span></span>|<span data-ttu-id="c5f40-182">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="c5f40-182">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="c5f40-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c5f40-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5f40-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5f40-185">JSON representation</span></span>

<span data-ttu-id="c5f40-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c5f40-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "keyProperty": "id"
}-->

```json
{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
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
  "description": "accessPackageCatalog resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

