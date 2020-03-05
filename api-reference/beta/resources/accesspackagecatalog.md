---
title: tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes do Access é um contêiner para pacotes do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 66b7939541ba57dafc3be852c82c89781fc82381
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508531"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="0c1fd-103">tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="0c1fd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0c1fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c1fd-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um catálogo de pacotes do Access é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="0c1fd-106">Um catálogo de pacotes do Access também pode ter recursos vinculados que são usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="0c1fd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c1fd-107">Methods</span></span>

| <span data-ttu-id="0c1fd-108">Método</span><span class="sxs-lookup"><span data-stu-id="0c1fd-108">Method</span></span>       | <span data-ttu-id="0c1fd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c1fd-109">Return Type</span></span> | <span data-ttu-id="0c1fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c1fd-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0c1fd-111">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="0c1fd-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="0c1fd-112">coleção [accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="0c1fd-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="0c1fd-113">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="0c1fd-114">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="0c1fd-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="0c1fd-116">Criar um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="0c1fd-117">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="0c1fd-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="0c1fd-119">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="0c1fd-120">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-120">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="0c1fd-121">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-121">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="0c1fd-122">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-122">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="0c1fd-123">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="0c1fd-123">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="0c1fd-124">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-124">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="0c1fd-125">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="0c1fd-125">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="0c1fd-126">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="0c1fd-126">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="0c1fd-127">Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-127">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="0c1fd-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c1fd-128">Properties</span></span>

| <span data-ttu-id="0c1fd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c1fd-129">Property</span></span>     | <span data-ttu-id="0c1fd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c1fd-130">Type</span></span>        | <span data-ttu-id="0c1fd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c1fd-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c1fd-132">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="0c1fd-132">catalogStatus</span></span>|<span data-ttu-id="0c1fd-133">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-133">String</span></span>|<span data-ttu-id="0c1fd-134">Tem o valor `Published` se os pacotes de acesso estiverem disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-134">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="0c1fd-135">CatalogType</span><span class="sxs-lookup"><span data-stu-id="0c1fd-135">catalogType</span></span>|<span data-ttu-id="0c1fd-136">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-136">String</span></span>|<span data-ttu-id="0c1fd-137">Um `UserManaged` ou `ServiceDefault`.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-137">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="0c1fd-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="0c1fd-138">createdBy</span></span>|<span data-ttu-id="0c1fd-139">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-139">String</span></span>|<span data-ttu-id="0c1fd-140">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-140">UPN of the user who created this resource.</span></span> <span data-ttu-id="0c1fd-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-141">Read-only.</span></span>|
|<span data-ttu-id="0c1fd-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c1fd-142">createdDateTime</span></span>|<span data-ttu-id="0c1fd-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c1fd-143">DateTimeOffset</span></span>|<span data-ttu-id="0c1fd-144">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0c1fd-145">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0c1fd-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-146">Read-only.</span></span>|
|<span data-ttu-id="0c1fd-147">description</span><span class="sxs-lookup"><span data-stu-id="0c1fd-147">description</span></span>|<span data-ttu-id="0c1fd-148">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-148">String</span></span>|<span data-ttu-id="0c1fd-149">A descrição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-149">The description of the access package catalog.</span></span>|
|<span data-ttu-id="0c1fd-150">displayName</span><span class="sxs-lookup"><span data-stu-id="0c1fd-150">displayName</span></span>|<span data-ttu-id="0c1fd-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c1fd-151">String</span></span>|<span data-ttu-id="0c1fd-152">O nome de exibição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-152">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="0c1fd-153">id</span><span class="sxs-lookup"><span data-stu-id="0c1fd-153">id</span></span>|<span data-ttu-id="0c1fd-154">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-154">String</span></span>| <span data-ttu-id="0c1fd-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-155">Read-only.</span></span>|
|<span data-ttu-id="0c1fd-156">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="0c1fd-156">isExternallyVisible</span></span>|<span data-ttu-id="0c1fd-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c1fd-157">Boolean</span></span>|<span data-ttu-id="0c1fd-158">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-158">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="0c1fd-159">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="0c1fd-159">modifiedBy</span></span>|<span data-ttu-id="0c1fd-160">String</span><span class="sxs-lookup"><span data-stu-id="0c1fd-160">String</span></span>|<span data-ttu-id="0c1fd-161">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-161">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="0c1fd-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-162">Read-only.</span></span>|
|<span data-ttu-id="0c1fd-163">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c1fd-163">modifiedDateTime</span></span>|<span data-ttu-id="0c1fd-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c1fd-164">DateTimeOffset</span></span>|<span data-ttu-id="0c1fd-165">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-165">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0c1fd-166">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0c1fd-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-167">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="0c1fd-168">Relações</span><span class="sxs-lookup"><span data-stu-id="0c1fd-168">Relationships</span></span>

| <span data-ttu-id="0c1fd-169">Relação</span><span class="sxs-lookup"><span data-stu-id="0c1fd-169">Relationship</span></span> | <span data-ttu-id="0c1fd-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c1fd-170">Type</span></span>        | <span data-ttu-id="0c1fd-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c1fd-171">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0c1fd-172">accessPackages</span><span class="sxs-lookup"><span data-stu-id="0c1fd-172">accessPackages</span></span>|<span data-ttu-id="0c1fd-173">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="0c1fd-173">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="0c1fd-174">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-174">The access packages in this catalog.</span></span> <span data-ttu-id="0c1fd-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-175">Read-only.</span></span> <span data-ttu-id="0c1fd-176">Anulável.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-176">Nullable.</span></span>|
|<span data-ttu-id="0c1fd-177">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="0c1fd-177">accessPackageResources</span></span>|<span data-ttu-id="0c1fd-178">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="0c1fd-178">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="0c1fd-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c1fd-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c1fd-181">JSON representation</span></span>

<span data-ttu-id="0c1fd-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c1fd-182">The following is a JSON representation of the resource.</span></span>

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
