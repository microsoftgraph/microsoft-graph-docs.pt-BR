---
title: tipo de recurso accessPackageResource
description: Um recurso de pacote do Access é uma referência a um recurso associado a um catálogo as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0567ca9347b560b14ae96da4914a8801f9183019
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870971"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="9e232-103">tipo de recurso accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="9e232-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e232-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um recurso de pacote do Access é uma referência a um recurso associado a um catálogo de pacotes do Access, as funções para as quais podem ser usadas em um ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="9e232-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="9e232-105">Para solicitar a associação de um recurso a um catálogo de pacotes do Access, crie um [accessPackageResourceRequest](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="9e232-105">To request to associate a resource with an access package catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9e232-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9e232-106">Methods</span></span>

| <span data-ttu-id="9e232-107">Método</span><span class="sxs-lookup"><span data-stu-id="9e232-107">Method</span></span>       | <span data-ttu-id="9e232-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9e232-108">Return Type</span></span> | <span data-ttu-id="9e232-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e232-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e232-110">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="9e232-110">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="9e232-111">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="9e232-111">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="9e232-112">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="9e232-112">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e232-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9e232-113">Properties</span></span>

| <span data-ttu-id="9e232-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9e232-114">Property</span></span>     | <span data-ttu-id="9e232-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e232-115">Type</span></span>        | <span data-ttu-id="9e232-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e232-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e232-117">addedBy</span><span class="sxs-lookup"><span data-stu-id="9e232-117">addedBy</span></span>|<span data-ttu-id="9e232-118">String</span><span class="sxs-lookup"><span data-stu-id="9e232-118">String</span></span>|<span data-ttu-id="9e232-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e232-119">Read-only.</span></span>|
|<span data-ttu-id="9e232-120">adicionado</span><span class="sxs-lookup"><span data-stu-id="9e232-120">addedOn</span></span>|<span data-ttu-id="9e232-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e232-121">DateTimeOffset</span></span>|<span data-ttu-id="9e232-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9e232-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9e232-124">descrição</span><span class="sxs-lookup"><span data-stu-id="9e232-124">description</span></span>|<span data-ttu-id="9e232-125">String</span><span class="sxs-lookup"><span data-stu-id="9e232-125">String</span></span>|<span data-ttu-id="9e232-126">Uma descrição do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e232-126">A description for the resource.</span></span>|
|<span data-ttu-id="9e232-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9e232-127">displayName</span></span>|<span data-ttu-id="9e232-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e232-128">String</span></span>|<span data-ttu-id="9e232-129">O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.</span><span class="sxs-lookup"><span data-stu-id="9e232-129">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="9e232-130">id</span><span class="sxs-lookup"><span data-stu-id="9e232-130">id</span></span>|<span data-ttu-id="9e232-131">String</span><span class="sxs-lookup"><span data-stu-id="9e232-131">String</span></span>| <span data-ttu-id="9e232-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e232-132">Read-only.</span></span>|
|<span data-ttu-id="9e232-133">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="9e232-133">isPendingOnboarding</span></span>|<span data-ttu-id="9e232-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="9e232-134">Boolean</span></span>|<span data-ttu-id="9e232-135">True se o recurso ainda não está disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="9e232-135">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="9e232-136">originid</span><span class="sxs-lookup"><span data-stu-id="9e232-136">originId</span></span>|<span data-ttu-id="9e232-137">String</span><span class="sxs-lookup"><span data-stu-id="9e232-137">String</span></span>|<span data-ttu-id="9e232-138">O identificador exclusivo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="9e232-138">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="9e232-139">No caso de um grupo do Azure AD, esse é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="9e232-139">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="9e232-140">originSystem</span><span class="sxs-lookup"><span data-stu-id="9e232-140">originSystem</span></span>|<span data-ttu-id="9e232-141">String</span><span class="sxs-lookup"><span data-stu-id="9e232-141">String</span></span>|<span data-ttu-id="9e232-142">O tipo do recurso no sistema de origem, como `SharePointOnline` ou. `AadGroup`</span><span class="sxs-lookup"><span data-stu-id="9e232-142">The type of the resource in the origin system, such as `SharePointOnline` or `AadGroup`.</span></span>|
|<span data-ttu-id="9e232-143">resourceType</span><span class="sxs-lookup"><span data-stu-id="9e232-143">resourceType</span></span>|<span data-ttu-id="9e232-144">String</span><span class="sxs-lookup"><span data-stu-id="9e232-144">String</span></span>|<span data-ttu-id="9e232-145">O tipo do recurso, como `Application` se é um aplicativo conectado ao Azure ad ou `SharePoint Online Site` um site do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9e232-145">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="9e232-146">url</span><span class="sxs-lookup"><span data-stu-id="9e232-146">url</span></span>|<span data-ttu-id="9e232-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9e232-147">String</span></span>|<span data-ttu-id="9e232-148">Um localizador de recursos exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e232-148">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e232-149">Relações</span><span class="sxs-lookup"><span data-stu-id="9e232-149">Relationships</span></span>

| <span data-ttu-id="9e232-150">Relação</span><span class="sxs-lookup"><span data-stu-id="9e232-150">Relationship</span></span> | <span data-ttu-id="9e232-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e232-151">Type</span></span>        | <span data-ttu-id="9e232-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e232-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e232-153">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="9e232-153">accessPackageResourceRoles</span></span>|<span data-ttu-id="9e232-154">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="9e232-154">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="9e232-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e232-155">Read-only.</span></span> <span data-ttu-id="9e232-156">Anulável.</span><span class="sxs-lookup"><span data-stu-id="9e232-156">Nullable.</span></span>|
|<span data-ttu-id="9e232-157">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="9e232-157">accessPackageResourceScopes</span></span>|<span data-ttu-id="9e232-158">coleção [accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="9e232-158">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="9e232-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="9e232-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e232-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9e232-161">JSON representation</span></span>

<span data-ttu-id="9e232-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9e232-162">The following is a JSON representation of the resource.</span></span>

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
