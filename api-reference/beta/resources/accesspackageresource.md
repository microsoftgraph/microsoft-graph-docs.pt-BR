---
title: Tipo de recurso accessPackageResource
description: Um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo para o qual as funções podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9c7b5e91c191ceaa747393e42e278bf9146bdc3a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722193"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="248c6-103">Tipo de recurso accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="248c6-103">accessPackageResource resource type</span></span>

<span data-ttu-id="248c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="248c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="248c6-105">No [Azure AD Entitlement Management](entitlementmanagement-root.md), um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo de pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="248c6-105">In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog.</span></span> <span data-ttu-id="248c6-106">As funções do recurso de pacote de acesso podem ser usadas em um ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="248c6-106">The roles for the access package resource can be used in one or more access packages.</span></span>  <span data-ttu-id="248c6-107">Para solicitar a associação de um recurso a um catálogo de pacotes de acesso ou remover um recurso de um catálogo, crie [um accessPackageResourceRequest](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="248c6-107">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="248c6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="248c6-108">Methods</span></span>

| <span data-ttu-id="248c6-109">Método</span><span class="sxs-lookup"><span data-stu-id="248c6-109">Method</span></span>       | <span data-ttu-id="248c6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="248c6-110">Return Type</span></span> | <span data-ttu-id="248c6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="248c6-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="248c6-112">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="248c6-112">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="248c6-113">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="248c6-113">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="248c6-114">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="248c6-114">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="248c6-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="248c6-115">Properties</span></span>

| <span data-ttu-id="248c6-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="248c6-116">Property</span></span>     | <span data-ttu-id="248c6-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="248c6-117">Type</span></span>        | <span data-ttu-id="248c6-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="248c6-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="248c6-119">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="248c6-119">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="248c6-120">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="248c6-120">accessPackageResourceEnvironment</span></span>](../resources/accesspackageresourceenvironment.md)|<span data-ttu-id="248c6-121">Contém as informações de ambiente do recurso.</span><span class="sxs-lookup"><span data-stu-id="248c6-121">Contains the environment information for the resource.</span></span> <span data-ttu-id="248c6-122">Isso pode ser definido usando `@odata.bind` a anotação ou a *origem do ambienteId*.</span><span class="sxs-lookup"><span data-stu-id="248c6-122">This can be set using either the `@odata.bind` annotation or the environment's *originId*.</span></span>|
|<span data-ttu-id="248c6-123">addedBy</span><span class="sxs-lookup"><span data-stu-id="248c6-123">addedBy</span></span>|<span data-ttu-id="248c6-124">String</span><span class="sxs-lookup"><span data-stu-id="248c6-124">String</span></span>|<span data-ttu-id="248c6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="248c6-125">Read-only.</span></span>|
|<span data-ttu-id="248c6-126">addedOn</span><span class="sxs-lookup"><span data-stu-id="248c6-126">addedOn</span></span>|<span data-ttu-id="248c6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="248c6-127">DateTimeOffset</span></span>|<span data-ttu-id="248c6-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="248c6-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="248c6-129">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="248c6-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="248c6-130">description</span><span class="sxs-lookup"><span data-stu-id="248c6-130">description</span></span>|<span data-ttu-id="248c6-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-131">String</span></span>|<span data-ttu-id="248c6-132">Uma descrição do recurso.</span><span class="sxs-lookup"><span data-stu-id="248c6-132">A description for the resource.</span></span>|
|<span data-ttu-id="248c6-133">displayName</span><span class="sxs-lookup"><span data-stu-id="248c6-133">displayName</span></span>|<span data-ttu-id="248c6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-134">String</span></span>|<span data-ttu-id="248c6-135">O nome de exibição do recurso, como nome do aplicativo, nome do grupo ou nome do site.</span><span class="sxs-lookup"><span data-stu-id="248c6-135">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="248c6-136">id</span><span class="sxs-lookup"><span data-stu-id="248c6-136">id</span></span>|<span data-ttu-id="248c6-137">String</span><span class="sxs-lookup"><span data-stu-id="248c6-137">String</span></span>| <span data-ttu-id="248c6-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="248c6-138">Read-only.</span></span>|
|<span data-ttu-id="248c6-139">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="248c6-139">isPendingOnboarding</span></span>|<span data-ttu-id="248c6-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="248c6-140">Boolean</span></span>|<span data-ttu-id="248c6-141">True se o recurso ainda não estiver disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="248c6-141">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="248c6-142">originId</span><span class="sxs-lookup"><span data-stu-id="248c6-142">originId</span></span>|<span data-ttu-id="248c6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-143">String</span></span>|<span data-ttu-id="248c6-144">O identificador exclusivo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="248c6-144">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="248c6-145">No caso de um grupo do Azure AD, esse é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="248c6-145">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="248c6-146">originSystem</span><span class="sxs-lookup"><span data-stu-id="248c6-146">originSystem</span></span>|<span data-ttu-id="248c6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-147">String</span></span>|<span data-ttu-id="248c6-148">O tipo do recurso no sistema de origem, como `SharePointOnline` , `AadApplication` ou `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="248c6-148">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="248c6-149">resourceType</span><span class="sxs-lookup"><span data-stu-id="248c6-149">resourceType</span></span>|<span data-ttu-id="248c6-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-150">String</span></span>|<span data-ttu-id="248c6-151">O tipo do recurso, como se fosse um aplicativo conectado ao `Application` Azure AD ou `SharePoint Online Site` para um site do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="248c6-151">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="248c6-152">url</span><span class="sxs-lookup"><span data-stu-id="248c6-152">url</span></span>|<span data-ttu-id="248c6-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="248c6-153">String</span></span>|<span data-ttu-id="248c6-154">Um localizador de recurso exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="248c6-154">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="248c6-155">Relações</span><span class="sxs-lookup"><span data-stu-id="248c6-155">Relationships</span></span>

| <span data-ttu-id="248c6-156">Relação</span><span class="sxs-lookup"><span data-stu-id="248c6-156">Relationship</span></span> | <span data-ttu-id="248c6-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="248c6-157">Type</span></span>        | <span data-ttu-id="248c6-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="248c6-158">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="248c6-159">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="248c6-159">accessPackageResourceEnvironment</span></span>|[<span data-ttu-id="248c6-160">accessPackageResourceEnvironment</span><span class="sxs-lookup"><span data-stu-id="248c6-160">accessPackageResourceEnvironment</span></span>](accesspackageresourceenvironment.md)| <span data-ttu-id="248c6-161">Anulável.</span><span class="sxs-lookup"><span data-stu-id="248c6-161">Nullable.</span></span>|
|<span data-ttu-id="248c6-162">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="248c6-162">accessPackageResourceRoles</span></span>|<span data-ttu-id="248c6-163">[Coleção accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="248c6-163">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="248c6-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="248c6-164">Read-only.</span></span> <span data-ttu-id="248c6-165">Anulável.</span><span class="sxs-lookup"><span data-stu-id="248c6-165">Nullable.</span></span>|
|<span data-ttu-id="248c6-166">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="248c6-166">accessPackageResourceScopes</span></span>|<span data-ttu-id="248c6-167">[Coleção accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="248c6-167">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="248c6-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="248c6-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="248c6-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="248c6-170">JSON representation</span></span>

<span data-ttu-id="248c6-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="248c6-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
