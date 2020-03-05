---
title: tipo de recurso accessPackageResource
description: Um recurso de pacote do Access é uma referência a um recurso associado a um catálogo as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8f862972b1c061d2c95267af19b26da300978288
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508524"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="742ae-103">tipo de recurso accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="742ae-103">accessPackageResource resource type</span></span>

<span data-ttu-id="742ae-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="742ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="742ae-105">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um recurso de pacote do Access é uma referência a um recurso associado a um catálogo de pacotes do Access, as funções para as quais podem ser usadas em um ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="742ae-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="742ae-106">Para solicitar a associação de um recurso a um catálogo de pacotes do Access, crie um [accessPackageResourceRequest](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="742ae-106">To request to associate a resource with an access package catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="742ae-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="742ae-107">Methods</span></span>

| <span data-ttu-id="742ae-108">Método</span><span class="sxs-lookup"><span data-stu-id="742ae-108">Method</span></span>       | <span data-ttu-id="742ae-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="742ae-109">Return Type</span></span> | <span data-ttu-id="742ae-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="742ae-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="742ae-111">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="742ae-111">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="742ae-112">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="742ae-112">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="742ae-113">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="742ae-113">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="742ae-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="742ae-114">Properties</span></span>

| <span data-ttu-id="742ae-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="742ae-115">Property</span></span>     | <span data-ttu-id="742ae-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="742ae-116">Type</span></span>        | <span data-ttu-id="742ae-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="742ae-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="742ae-118">addedBy</span><span class="sxs-lookup"><span data-stu-id="742ae-118">addedBy</span></span>|<span data-ttu-id="742ae-119">String</span><span class="sxs-lookup"><span data-stu-id="742ae-119">String</span></span>|<span data-ttu-id="742ae-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="742ae-120">Read-only.</span></span>|
|<span data-ttu-id="742ae-121">adicionado</span><span class="sxs-lookup"><span data-stu-id="742ae-121">addedOn</span></span>|<span data-ttu-id="742ae-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="742ae-122">DateTimeOffset</span></span>|<span data-ttu-id="742ae-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="742ae-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="742ae-125">description</span><span class="sxs-lookup"><span data-stu-id="742ae-125">description</span></span>|<span data-ttu-id="742ae-126">String</span><span class="sxs-lookup"><span data-stu-id="742ae-126">String</span></span>|<span data-ttu-id="742ae-127">Uma descrição do recurso.</span><span class="sxs-lookup"><span data-stu-id="742ae-127">A description for the resource.</span></span>|
|<span data-ttu-id="742ae-128">displayName</span><span class="sxs-lookup"><span data-stu-id="742ae-128">displayName</span></span>|<span data-ttu-id="742ae-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="742ae-129">String</span></span>|<span data-ttu-id="742ae-130">O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.</span><span class="sxs-lookup"><span data-stu-id="742ae-130">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="742ae-131">id</span><span class="sxs-lookup"><span data-stu-id="742ae-131">id</span></span>|<span data-ttu-id="742ae-132">String</span><span class="sxs-lookup"><span data-stu-id="742ae-132">String</span></span>| <span data-ttu-id="742ae-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="742ae-133">Read-only.</span></span>|
|<span data-ttu-id="742ae-134">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="742ae-134">isPendingOnboarding</span></span>|<span data-ttu-id="742ae-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="742ae-135">Boolean</span></span>|<span data-ttu-id="742ae-136">True se o recurso ainda não está disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="742ae-136">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="742ae-137">originid</span><span class="sxs-lookup"><span data-stu-id="742ae-137">originId</span></span>|<span data-ttu-id="742ae-138">String</span><span class="sxs-lookup"><span data-stu-id="742ae-138">String</span></span>|<span data-ttu-id="742ae-139">O identificador exclusivo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="742ae-139">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="742ae-140">No caso de um grupo do Azure AD, esse é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="742ae-140">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="742ae-141">originSystem</span><span class="sxs-lookup"><span data-stu-id="742ae-141">originSystem</span></span>|<span data-ttu-id="742ae-142">String</span><span class="sxs-lookup"><span data-stu-id="742ae-142">String</span></span>|<span data-ttu-id="742ae-143">O tipo do recurso no sistema de origem, como `SharePointOnline` ou. `AadGroup`</span><span class="sxs-lookup"><span data-stu-id="742ae-143">The type of the resource in the origin system, such as `SharePointOnline` or `AadGroup`.</span></span>|
|<span data-ttu-id="742ae-144">resourceType</span><span class="sxs-lookup"><span data-stu-id="742ae-144">resourceType</span></span>|<span data-ttu-id="742ae-145">String</span><span class="sxs-lookup"><span data-stu-id="742ae-145">String</span></span>|<span data-ttu-id="742ae-146">O tipo do recurso, como `Application` se é um aplicativo conectado ao Azure ad ou `SharePoint Online Site` um site do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="742ae-146">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="742ae-147">url</span><span class="sxs-lookup"><span data-stu-id="742ae-147">url</span></span>|<span data-ttu-id="742ae-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="742ae-148">String</span></span>|<span data-ttu-id="742ae-149">Um localizador de recursos exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="742ae-149">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="742ae-150">Relações</span><span class="sxs-lookup"><span data-stu-id="742ae-150">Relationships</span></span>

| <span data-ttu-id="742ae-151">Relação</span><span class="sxs-lookup"><span data-stu-id="742ae-151">Relationship</span></span> | <span data-ttu-id="742ae-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="742ae-152">Type</span></span>        | <span data-ttu-id="742ae-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="742ae-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="742ae-154">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="742ae-154">accessPackageResourceRoles</span></span>|<span data-ttu-id="742ae-155">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="742ae-155">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="742ae-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="742ae-156">Read-only.</span></span> <span data-ttu-id="742ae-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="742ae-157">Nullable.</span></span>|
|<span data-ttu-id="742ae-158">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="742ae-158">accessPackageResourceScopes</span></span>|<span data-ttu-id="742ae-159">coleção [accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="742ae-159">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="742ae-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="742ae-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="742ae-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="742ae-162">JSON representation</span></span>

<span data-ttu-id="742ae-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="742ae-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
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
