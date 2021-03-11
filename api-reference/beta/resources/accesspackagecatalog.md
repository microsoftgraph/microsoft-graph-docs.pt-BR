---
title: Tipo de recurso accessPackageCatalog
description: Um catálogo de pacotes de acesso é um contêiner para pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 87c2541179cd94472eadab692544a40a1d8b81b7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720421"
---
# <a name="accesspackagecatalog-resource-type"></a><span data-ttu-id="2894a-103">Tipo de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-103">accessPackageCatalog resource type</span></span>

<span data-ttu-id="2894a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2894a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2894a-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um catálogo de pacotes de acesso é um contêiner para zero ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="2894a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package catalog is a container for zero or more access packages.</span></span>  <span data-ttu-id="2894a-106">Um catálogo de pacotes de acesso também pode ter recursos vinculados usados nesses pacotes de acesso para fornecer acesso.</span><span class="sxs-lookup"><span data-stu-id="2894a-106">An access package catalog might also have linked resources that are used in those access packages to provide access.</span></span>


## <a name="methods"></a><span data-ttu-id="2894a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2894a-107">Methods</span></span>

| <span data-ttu-id="2894a-108">Método</span><span class="sxs-lookup"><span data-stu-id="2894a-108">Method</span></span>       | <span data-ttu-id="2894a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2894a-109">Return Type</span></span> | <span data-ttu-id="2894a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2894a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2894a-111">Listar accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="2894a-111">List accessPackageCatalogs</span></span>](../api/accesspackagecatalog-list.md) | <span data-ttu-id="2894a-112">[Coleção accessPackageCatalog](accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="2894a-112">[accessPackageCatalog](accesspackagecatalog.md) collection</span></span> | <span data-ttu-id="2894a-113">Recupere uma lista de objetos accesspackagecatalog.</span><span class="sxs-lookup"><span data-stu-id="2894a-113">Retrieve a list of accesspackagecatalog objects.</span></span> |
| [<span data-ttu-id="2894a-114">Criar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-114">Create accessPackageCatalog</span></span>](../api/accesspackagecatalog-post.md) | [<span data-ttu-id="2894a-115">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-115">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="2894a-116">Crie um novo objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="2894a-116">Create a new accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="2894a-117">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-117">Get accessPackageCatalog</span></span>](../api/accesspackagecatalog-get.md) | [<span data-ttu-id="2894a-118">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-118">accessPackageCatalog</span></span>](accesspackagecatalog.md) | <span data-ttu-id="2894a-119">Ler propriedades e relações de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="2894a-119">Read properties and relationships of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="2894a-120">Atualizar accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-120">Update accessPackageCatalog</span></span>](../api/accesspackagecatalog-update.md)|<span data-ttu-id="2894a-121">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="2894a-121">None</span></span> | <span data-ttu-id="2894a-122">Atualize as propriedades de um objeto accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="2894a-122">Update the properties of an accessPackageCatalog object.</span></span> |
| [<span data-ttu-id="2894a-123">Excluir accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-123">Delete accessPackageCatalog</span></span>](../api/accesspackagecatalog-delete.md) | | <span data-ttu-id="2894a-124">Exclua accessPackageCatalog.</span><span class="sxs-lookup"><span data-stu-id="2894a-124">Delete accessPackageCatalog.</span></span> |
| [<span data-ttu-id="2894a-125">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-125">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="2894a-126">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="2894a-126">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="2894a-127">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="2894a-127">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |
| [<span data-ttu-id="2894a-128">Listar funções de recurso accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="2894a-128">List accessPackageCatalog resource roles</span></span>](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | <span data-ttu-id="2894a-129">[Coleção accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="2894a-129">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span> | <span data-ttu-id="2894a-130">Recupere uma lista de objetos accessPackageResourceRole para recursos em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="2894a-130">Retrieve a list of accessPackageResourceRole objects for resources in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="2894a-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2894a-131">Properties</span></span>

| <span data-ttu-id="2894a-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2894a-132">Property</span></span>     | <span data-ttu-id="2894a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="2894a-133">Type</span></span>        | <span data-ttu-id="2894a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2894a-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2894a-135">catalogStatus</span><span class="sxs-lookup"><span data-stu-id="2894a-135">catalogStatus</span></span>|<span data-ttu-id="2894a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-136">String</span></span>|<span data-ttu-id="2894a-137">Tem o valor `Published` se os pacotes de acesso estão disponíveis para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="2894a-137">Has the value `Published` if the access packages are available for management.</span></span>|
|<span data-ttu-id="2894a-138">catalogType</span><span class="sxs-lookup"><span data-stu-id="2894a-138">catalogType</span></span>|<span data-ttu-id="2894a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-139">String</span></span>|<span data-ttu-id="2894a-140">Um dos `UserManaged` ou `ServiceDefault` .</span><span class="sxs-lookup"><span data-stu-id="2894a-140">One of `UserManaged` or `ServiceDefault`.</span></span> |
|<span data-ttu-id="2894a-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="2894a-141">createdBy</span></span>|<span data-ttu-id="2894a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-142">String</span></span>|<span data-ttu-id="2894a-143">UPN do usuário que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="2894a-143">UPN of the user who created this resource.</span></span> <span data-ttu-id="2894a-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-144">Read-only.</span></span>|
|<span data-ttu-id="2894a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2894a-145">createdDateTime</span></span>|<span data-ttu-id="2894a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2894a-146">DateTimeOffset</span></span>|<span data-ttu-id="2894a-147">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2894a-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2894a-148">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2894a-148">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2894a-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-149">Read-only.</span></span>|
|<span data-ttu-id="2894a-150">description</span><span class="sxs-lookup"><span data-stu-id="2894a-150">description</span></span>|<span data-ttu-id="2894a-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-151">String</span></span>|<span data-ttu-id="2894a-152">A descrição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="2894a-152">The description of the access package catalog.</span></span>|
|<span data-ttu-id="2894a-153">displayName</span><span class="sxs-lookup"><span data-stu-id="2894a-153">displayName</span></span>|<span data-ttu-id="2894a-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-154">String</span></span>|<span data-ttu-id="2894a-155">O nome de exibição do catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="2894a-155">The display name of the access package catalog.</span></span>|
|<span data-ttu-id="2894a-156">id</span><span class="sxs-lookup"><span data-stu-id="2894a-156">id</span></span>|<span data-ttu-id="2894a-157">String</span><span class="sxs-lookup"><span data-stu-id="2894a-157">String</span></span>| <span data-ttu-id="2894a-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-158">Read-only.</span></span>|
|<span data-ttu-id="2894a-159">isExternallyVisible</span><span class="sxs-lookup"><span data-stu-id="2894a-159">isExternallyVisible</span></span>|<span data-ttu-id="2894a-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="2894a-160">Boolean</span></span>|<span data-ttu-id="2894a-161">Se os pacotes de acesso neste catálogo podem ser solicitados por usuários fora do locatário.</span><span class="sxs-lookup"><span data-stu-id="2894a-161">Whether the access packages in this catalog can be requested by users outside of the tenant.</span></span>|
|<span data-ttu-id="2894a-162">modifiedBy</span><span class="sxs-lookup"><span data-stu-id="2894a-162">modifiedBy</span></span>|<span data-ttu-id="2894a-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2894a-163">String</span></span>|<span data-ttu-id="2894a-164">O UPN do usuário que modificou esse recurso pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2894a-164">The UPN of the user who last modified this resource.</span></span> <span data-ttu-id="2894a-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-165">Read-only.</span></span>|
|<span data-ttu-id="2894a-166">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2894a-166">modifiedDateTime</span></span>|<span data-ttu-id="2894a-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2894a-167">DateTimeOffset</span></span>|<span data-ttu-id="2894a-168">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2894a-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2894a-169">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2894a-169">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2894a-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-170">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="2894a-171">Relações</span><span class="sxs-lookup"><span data-stu-id="2894a-171">Relationships</span></span>

| <span data-ttu-id="2894a-172">Relação</span><span class="sxs-lookup"><span data-stu-id="2894a-172">Relationship</span></span> | <span data-ttu-id="2894a-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="2894a-173">Type</span></span>        | <span data-ttu-id="2894a-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="2894a-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2894a-175">accessPackages</span><span class="sxs-lookup"><span data-stu-id="2894a-175">accessPackages</span></span>|<span data-ttu-id="2894a-176">[Coleção accessPackage](accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="2894a-176">[accessPackage](accesspackage.md) collection</span></span>| <span data-ttu-id="2894a-177">Os pacotes de acesso neste catálogo.</span><span class="sxs-lookup"><span data-stu-id="2894a-177">The access packages in this catalog.</span></span> <span data-ttu-id="2894a-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2894a-178">Read-only.</span></span> <span data-ttu-id="2894a-179">Anulável.</span><span class="sxs-lookup"><span data-stu-id="2894a-179">Nullable.</span></span>|
|<span data-ttu-id="2894a-180">accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="2894a-180">accessPackageResources</span></span>|<span data-ttu-id="2894a-181">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="2894a-181">[accessPackageResource](accesspackageresource.md) collection</span></span>| <span data-ttu-id="2894a-p107">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2894a-p107">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2894a-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2894a-184">JSON representation</span></span>

<span data-ttu-id="2894a-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2894a-185">The following is a JSON representation of the resource.</span></span>

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


