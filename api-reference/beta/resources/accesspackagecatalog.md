---
title: tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes do Access é um contêiner para pacotes do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c8fde3b6ead60cada5e663b2150ba463187b22b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870412"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="b3c29-103">tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3c29-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um catálogo de pacotes do Access é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="b3c29-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="b3c29-105">Um catálogo de pacotes do Access também pode ter recursos vinculados que são usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="b3c29-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="b3c29-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3c29-106">Methods</span></span>

| <span data-ttu-id="b3c29-107">Método</span><span class="sxs-lookup"><span data-stu-id="b3c29-107">Method</span></span>       | <span data-ttu-id="b3c29-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3c29-108">Return Type</span></span> | <span data-ttu-id="b3c29-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c29-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b3c29-110">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="b3c29-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="b3c29-111">coleção [accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="b3c29-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="b3c29-112">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="b3c29-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="b3c29-113">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="b3c29-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="b3c29-115">Criar um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="b3c29-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="b3c29-116">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="b3c29-117">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="b3c29-118">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="b3c29-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="b3c29-119">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="b3c29-120">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="b3c29-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="b3c29-121">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="b3c29-122">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="b3c29-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="b3c29-123">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="b3c29-123">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="b3c29-124">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="b3c29-124">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="b3c29-125">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="b3c29-125">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="b3c29-126">Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="b3c29-126">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3c29-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3c29-127">Properties</span></span>

| <span data-ttu-id="b3c29-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3c29-128">Property</span></span>     | <span data-ttu-id="b3c29-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3c29-129">Type</span></span>        | <span data-ttu-id="b3c29-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c29-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3c29-131">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="b3c29-131">catalogStatus</span></span>|<span data-ttu-id="b3c29-132">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-132">String</span></span>|<span data-ttu-id="b3c29-133">Tem o valor `Published` se os pacotes de acesso estiverem disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="b3c29-133">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="b3c29-134">CatalogType</span><span class="sxs-lookup"><span data-stu-id="b3c29-134">catalogType</span></span>|<span data-ttu-id="b3c29-135">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-135">String</span></span>|<span data-ttu-id="b3c29-136">Um `UserManaged` ou `ServiceDefault`.</span><span class="sxs-lookup"><span data-stu-id="b3c29-136">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="b3c29-137">createdBy</span><span class="sxs-lookup"><span data-stu-id="b3c29-137">createdBy</span></span>|<span data-ttu-id="b3c29-138">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-138">String</span></span>|<span data-ttu-id="b3c29-139">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="b3c29-139">UPN of the user who created this resource.</span></span> <span data-ttu-id="b3c29-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-140">Read-only.</span></span>|
|<span data-ttu-id="b3c29-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3c29-141">createdDateTime</span></span>|<span data-ttu-id="b3c29-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3c29-142">DateTimeOffset</span></span>|<span data-ttu-id="b3c29-143">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3c29-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3c29-144">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b3c29-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b3c29-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-145">Read-only.</span></span>|
|<span data-ttu-id="b3c29-146">description</span><span class="sxs-lookup"><span data-stu-id="b3c29-146">description</span></span>|<span data-ttu-id="b3c29-147">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-147">String</span></span>|<span data-ttu-id="b3c29-148">A descrição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="b3c29-148">The description of the access package catalog.</span></span>|
|<span data-ttu-id="b3c29-149">displayName</span><span class="sxs-lookup"><span data-stu-id="b3c29-149">displayName</span></span>|<span data-ttu-id="b3c29-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3c29-150">String</span></span>|<span data-ttu-id="b3c29-151">O nome de exibição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="b3c29-151">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="b3c29-152">id</span><span class="sxs-lookup"><span data-stu-id="b3c29-152">id</span></span>|<span data-ttu-id="b3c29-153">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-153">String</span></span>| <span data-ttu-id="b3c29-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-154">Read-only.</span></span>|
|<span data-ttu-id="b3c29-155">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="b3c29-155">isExternallyVisible</span></span>|<span data-ttu-id="b3c29-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="b3c29-156">Boolean</span></span>|<span data-ttu-id="b3c29-157">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="b3c29-157">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="b3c29-158">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="b3c29-158">modifiedBy</span></span>|<span data-ttu-id="b3c29-159">String</span><span class="sxs-lookup"><span data-stu-id="b3c29-159">String</span></span>|<span data-ttu-id="b3c29-160">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b3c29-160">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="b3c29-161">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-161">Read-only.</span></span>|
|<span data-ttu-id="b3c29-162">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3c29-162">modifiedDateTime</span></span>|<span data-ttu-id="b3c29-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3c29-163">DateTimeOffset</span></span>|<span data-ttu-id="b3c29-164">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b3c29-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3c29-165">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b3c29-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="b3c29-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-166">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="b3c29-167">Relações</span><span class="sxs-lookup"><span data-stu-id="b3c29-167">Relationships</span></span>

| <span data-ttu-id="b3c29-168">Relação</span><span class="sxs-lookup"><span data-stu-id="b3c29-168">Relationship</span></span> | <span data-ttu-id="b3c29-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3c29-169">Type</span></span>        | <span data-ttu-id="b3c29-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c29-170">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b3c29-171">accessPackages</span><span class="sxs-lookup"><span data-stu-id="b3c29-171">accessPackages</span></span>|<span data-ttu-id="b3c29-172">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="b3c29-172">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="b3c29-173">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="b3c29-173">The access packages in this catalog.</span></span> <span data-ttu-id="b3c29-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3c29-174">Read-only.</span></span> <span data-ttu-id="b3c29-175">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3c29-175">Nullable.</span></span>|
|<span data-ttu-id="b3c29-176">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="b3c29-176">accessPackageResources</span></span>|<span data-ttu-id="b3c29-177">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="b3c29-177">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="b3c29-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b3c29-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3c29-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3c29-180">JSON representation</span></span>

<span data-ttu-id="b3c29-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3c29-181">The following is a JSON representation of the resource.</span></span>

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
