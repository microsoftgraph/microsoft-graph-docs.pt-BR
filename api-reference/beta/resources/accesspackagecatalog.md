---
title: tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes do Access é um contêiner para pacotes do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5e5066337ef88db6a036839ebcbfd454e7710f3a
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757199"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="d568e-103">tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="d568e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d568e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d568e-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um catálogo de pacotes do Access é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="d568e-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="d568e-106">Um catálogo de pacotes do Access também pode ter recursos vinculados que são usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="d568e-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="d568e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d568e-107">Methods</span></span>

| <span data-ttu-id="d568e-108">Método</span><span class="sxs-lookup"><span data-stu-id="d568e-108">Method</span></span>       | <span data-ttu-id="d568e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d568e-109">Return Type</span></span> | <span data-ttu-id="d568e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d568e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d568e-111">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="d568e-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="d568e-112">coleção [accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="d568e-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="d568e-113">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="d568e-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="d568e-114">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="d568e-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="d568e-116">Criar um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="d568e-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="d568e-117">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="d568e-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="d568e-119">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="d568e-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="d568e-120">Atualizar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="d568e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d568e-121">None</span></span> | <span data-ttu-id="d568e-122">Atualiza as propriedades de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="d568e-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="d568e-123">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="d568e-124">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="d568e-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="d568e-125">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="d568e-126">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="d568e-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="d568e-127">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="d568e-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="d568e-128">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="d568e-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="d568e-129">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="d568e-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="d568e-130">Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="d568e-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="d568e-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d568e-131">Properties</span></span>

| <span data-ttu-id="d568e-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d568e-132">Property</span></span>     | <span data-ttu-id="d568e-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="d568e-133">Type</span></span>        | <span data-ttu-id="d568e-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="d568e-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d568e-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="d568e-135">catalogStatus</span></span>|<span data-ttu-id="d568e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d568e-136">String</span></span>|<span data-ttu-id="d568e-137">Tem o valor `Published` se os pacotes de acesso estiverem disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d568e-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="d568e-138">CatalogType</span><span class="sxs-lookup"><span data-stu-id="d568e-138">catalogType</span></span>|<span data-ttu-id="d568e-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d568e-139">String</span></span>|<span data-ttu-id="d568e-140">Um `UserManaged` ou `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="d568e-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="d568e-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="d568e-141">createdBy</span></span>|<span data-ttu-id="d568e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d568e-142">String</span></span>|<span data-ttu-id="d568e-143">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="d568e-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="d568e-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-144">Read-only.</span></span>|
|<span data-ttu-id="d568e-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d568e-145">createdDateTime</span></span>|<span data-ttu-id="d568e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d568e-146">DateTimeOffset</span></span>|<span data-ttu-id="d568e-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d568e-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d568e-148">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d568e-148">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d568e-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-149">Read-only.</span></span>|
|<span data-ttu-id="d568e-150">description</span><span class="sxs-lookup"><span data-stu-id="d568e-150">description</span></span>|<span data-ttu-id="d568e-151">String</span><span class="sxs-lookup"><span data-stu-id="d568e-151">String</span></span>|<span data-ttu-id="d568e-152">A descrição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="d568e-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="d568e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d568e-153">displayName</span></span>|<span data-ttu-id="d568e-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d568e-154">String</span></span>|<span data-ttu-id="d568e-155">O nome de exibição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="d568e-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="d568e-156">id</span><span class="sxs-lookup"><span data-stu-id="d568e-156">id</span></span>|<span data-ttu-id="d568e-157">String</span><span class="sxs-lookup"><span data-stu-id="d568e-157">String</span></span>| <span data-ttu-id="d568e-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-158">Read-only.</span></span>|
|<span data-ttu-id="d568e-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="d568e-159">isExternallyVisible</span></span>|<span data-ttu-id="d568e-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="d568e-160">Boolean</span></span>|<span data-ttu-id="d568e-161">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="d568e-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="d568e-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="d568e-162">modifiedBy</span></span>|<span data-ttu-id="d568e-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d568e-163">String</span></span>|<span data-ttu-id="d568e-164">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d568e-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="d568e-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-165">Read-only.</span></span>|
|<span data-ttu-id="d568e-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d568e-166">modifiedDateTime</span></span>|<span data-ttu-id="d568e-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d568e-167">DateTimeOffset</span></span>|<span data-ttu-id="d568e-168">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="d568e-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d568e-169">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d568e-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d568e-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="d568e-171">Relações</span><span class="sxs-lookup"><span data-stu-id="d568e-171">Relationships</span></span>

| <span data-ttu-id="d568e-172">Relação</span><span class="sxs-lookup"><span data-stu-id="d568e-172">Relationship</span></span> | <span data-ttu-id="d568e-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="d568e-173">Type</span></span>        | <span data-ttu-id="d568e-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="d568e-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d568e-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="d568e-175">accessPackages</span></span>|<span data-ttu-id="d568e-176">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="d568e-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="d568e-177">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="d568e-177">The access packages in this catalog.</span></span> <span data-ttu-id="d568e-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d568e-178">Read-only.</span></span> <span data-ttu-id="d568e-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="d568e-179">Nullable.</span></span>|
|<span data-ttu-id="d568e-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="d568e-180">accessPackageResources</span></span>|<span data-ttu-id="d568e-181">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="d568e-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="d568e-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d568e-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d568e-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d568e-184">JSON representation</span></span>

<span data-ttu-id="d568e-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d568e-185">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "baseType": "",
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
