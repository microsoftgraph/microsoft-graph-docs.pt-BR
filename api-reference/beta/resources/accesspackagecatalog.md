---
title: tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes do Access é um contêiner para pacotes do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d95037bdf1e377f8981f99a06670957d838a2c92
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938930"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="71453-103">tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-103">accessPackageCatalog resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71453-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um catálogo de pacotes do Access é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="71453-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="71453-105">Um catálogo de pacotes do Access também pode ter recursos vinculados que são usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="71453-105">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="71453-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="71453-106">Methods</span></span>

| <span data-ttu-id="71453-107">Método</span><span class="sxs-lookup"><span data-stu-id="71453-107">Method</span></span>       | <span data-ttu-id="71453-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="71453-108">Return Type</span></span> | <span data-ttu-id="71453-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="71453-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="71453-110">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="71453-110">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="71453-111">coleção [accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="71453-111">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="71453-112">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="71453-112">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="71453-113">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-113">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="71453-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-114">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="71453-115">Criar um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="71453-115">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="71453-116">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-116">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="71453-117">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-117">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="71453-118">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="71453-118">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="71453-119">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-119">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="71453-120">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="71453-120">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="71453-121">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="71453-121">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="71453-122">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="71453-122">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="71453-123">Recupere uma lista de objetos accessPackageResource.</span><span class="sxs-lookup"><span data-stu-id="71453-123">Retrieve a list of accessPackageResource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="71453-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71453-124">Properties</span></span>

| <span data-ttu-id="71453-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71453-125">Property</span></span>     | <span data-ttu-id="71453-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="71453-126">Type</span></span>        | <span data-ttu-id="71453-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="71453-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71453-128">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="71453-128">catalogStatus</span></span>|<span data-ttu-id="71453-129">String</span><span class="sxs-lookup"><span data-stu-id="71453-129">String</span></span>|<span data-ttu-id="71453-130">Tem o valor `Published` se os pacotes de acesso estiverem disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="71453-130">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="71453-131">CatalogType</span><span class="sxs-lookup"><span data-stu-id="71453-131">catalogType</span></span>|<span data-ttu-id="71453-132">String</span><span class="sxs-lookup"><span data-stu-id="71453-132">String</span></span>|<span data-ttu-id="71453-133">Um `UserManaged` ou `ServiceDefault`.</span><span class="sxs-lookup"><span data-stu-id="71453-133">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="71453-134">createdBy</span><span class="sxs-lookup"><span data-stu-id="71453-134">createdBy</span></span>|<span data-ttu-id="71453-135">String</span><span class="sxs-lookup"><span data-stu-id="71453-135">String</span></span>|<span data-ttu-id="71453-136">UPN do usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="71453-136">UPN of the user who created this resource.</span></span> <span data-ttu-id="71453-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-137">Read-only.</span></span>|
|<span data-ttu-id="71453-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71453-138">createdDateTime</span></span>|<span data-ttu-id="71453-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71453-139">DateTimeOffset</span></span>|<span data-ttu-id="71453-140">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="71453-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71453-141">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="71453-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="71453-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-142">Read-only.</span></span>|
|<span data-ttu-id="71453-143">description</span><span class="sxs-lookup"><span data-stu-id="71453-143">description</span></span>|<span data-ttu-id="71453-144">String</span><span class="sxs-lookup"><span data-stu-id="71453-144">String</span></span>|<span data-ttu-id="71453-145">A descrição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="71453-145">The description of the access package catalog.</span></span>|
|<span data-ttu-id="71453-146">displayName</span><span class="sxs-lookup"><span data-stu-id="71453-146">displayName</span></span>|<span data-ttu-id="71453-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71453-147">String</span></span>|<span data-ttu-id="71453-148">O nome de exibição do catálogo de pacotes do Access.</span><span class="sxs-lookup"><span data-stu-id="71453-148">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="71453-149">id</span><span class="sxs-lookup"><span data-stu-id="71453-149">id</span></span>|<span data-ttu-id="71453-150">String</span><span class="sxs-lookup"><span data-stu-id="71453-150">String</span></span>| <span data-ttu-id="71453-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-151">Read-only.</span></span>|
|<span data-ttu-id="71453-152">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="71453-152">isExternallyVisible</span></span>|<span data-ttu-id="71453-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="71453-153">Boolean</span></span>|<span data-ttu-id="71453-154">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="71453-154">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="71453-155">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="71453-155">modifiedBy</span></span>|<span data-ttu-id="71453-156">String</span><span class="sxs-lookup"><span data-stu-id="71453-156">String</span></span>|<span data-ttu-id="71453-157">O UPN do usuário que modificou este recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="71453-157">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="71453-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-158">Read-only.</span></span>|
|<span data-ttu-id="71453-159">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71453-159">modifiedDateTime</span></span>|<span data-ttu-id="71453-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71453-160">DateTimeOffset</span></span>|<span data-ttu-id="71453-161">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="71453-161">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="71453-162">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="71453-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="71453-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-163">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="71453-164">Relações</span><span class="sxs-lookup"><span data-stu-id="71453-164">Relationships</span></span>

| <span data-ttu-id="71453-165">Relação</span><span class="sxs-lookup"><span data-stu-id="71453-165">Relationship</span></span> | <span data-ttu-id="71453-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="71453-166">Type</span></span>        | <span data-ttu-id="71453-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="71453-167">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="71453-168">accessPackages</span><span class="sxs-lookup"><span data-stu-id="71453-168">accessPackages</span></span>|<span data-ttu-id="71453-169">coleção [accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="71453-169">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="71453-170">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="71453-170">The access packages in this catalog.</span></span> <span data-ttu-id="71453-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="71453-171">Read-only.</span></span> <span data-ttu-id="71453-172">Anulável.</span><span class="sxs-lookup"><span data-stu-id="71453-172">Nullable.</span></span>|
|<span data-ttu-id="71453-173">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="71453-173">accessPackageResources</span></span>|<span data-ttu-id="71453-174">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="71453-174">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="71453-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="71453-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71453-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71453-177">JSON representation</span></span>

<span data-ttu-id="71453-178">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="71453-178">The following is a JSON representation of the resource.</span></span>

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
