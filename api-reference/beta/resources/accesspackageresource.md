---
title: Tipo de recurso accessPackageResource
description: Um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo para as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e34b850b19836eeb19cc63232c7af822512bfee4
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934819"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="3d64a-103">Tipo de recurso accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="3d64a-103">accessPackageResource resource type</span></span>

<span data-ttu-id="3d64a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d64a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d64a-105">No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)um recurso de pacote de acesso é uma referência a um recurso associado a um catálogo de pacotes de acesso, as funções para as quais podem ser usadas em um ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="3d64a-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with an access package catalog, the roles for which can be used in one or more access packages.</span></span>  <span data-ttu-id="3d64a-106">Para solicitar a associação de um recurso a um catálogo de pacotes de acesso ou remover um recurso de um catálogo, crie um [accessPackageResourceRequest](accesspackageresourcerequest.md).</span><span class="sxs-lookup"><span data-stu-id="3d64a-106">To request to associate a resource with an access package catalog, or remove a resource from a catalog, create an [accessPackageResourceRequest](accesspackageresourcerequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3d64a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3d64a-107">Methods</span></span>

| <span data-ttu-id="3d64a-108">Método</span><span class="sxs-lookup"><span data-stu-id="3d64a-108">Method</span></span>       | <span data-ttu-id="3d64a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3d64a-109">Return Type</span></span> | <span data-ttu-id="3d64a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d64a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3d64a-111">Listar recursos accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3d64a-111">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="3d64a-112">[Coleção accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="3d64a-112">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="3d64a-113">Recupere uma lista de objetos accessPackageResource em um catálogo.</span><span class="sxs-lookup"><span data-stu-id="3d64a-113">Retrieve a list of accessPackageResource objects in a catalog.</span></span> |

## <a name="properties"></a><span data-ttu-id="3d64a-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d64a-114">Properties</span></span>

| <span data-ttu-id="3d64a-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d64a-115">Property</span></span>     | <span data-ttu-id="3d64a-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d64a-116">Type</span></span>        | <span data-ttu-id="3d64a-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d64a-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d64a-118">addedBy</span><span class="sxs-lookup"><span data-stu-id="3d64a-118">addedBy</span></span>|<span data-ttu-id="3d64a-119">String</span><span class="sxs-lookup"><span data-stu-id="3d64a-119">String</span></span>|<span data-ttu-id="3d64a-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d64a-120">Read-only.</span></span>|
|<span data-ttu-id="3d64a-121">addedOn</span><span class="sxs-lookup"><span data-stu-id="3d64a-121">addedOn</span></span>|<span data-ttu-id="3d64a-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d64a-122">DateTimeOffset</span></span>|<span data-ttu-id="3d64a-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3d64a-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3d64a-125">description</span><span class="sxs-lookup"><span data-stu-id="3d64a-125">description</span></span>|<span data-ttu-id="3d64a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-126">String</span></span>|<span data-ttu-id="3d64a-127">Uma descrição para o recurso.</span><span class="sxs-lookup"><span data-stu-id="3d64a-127">A description for the resource.</span></span>|
|<span data-ttu-id="3d64a-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3d64a-128">displayName</span></span>|<span data-ttu-id="3d64a-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-129">String</span></span>|<span data-ttu-id="3d64a-130">O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.</span><span class="sxs-lookup"><span data-stu-id="3d64a-130">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="3d64a-131">id</span><span class="sxs-lookup"><span data-stu-id="3d64a-131">id</span></span>|<span data-ttu-id="3d64a-132">String</span><span class="sxs-lookup"><span data-stu-id="3d64a-132">String</span></span>| <span data-ttu-id="3d64a-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d64a-133">Read-only.</span></span>|
|<span data-ttu-id="3d64a-134">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="3d64a-134">isPendingOnboarding</span></span>|<span data-ttu-id="3d64a-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="3d64a-135">Boolean</span></span>|<span data-ttu-id="3d64a-136">True se o recurso ainda não estiver disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="3d64a-136">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="3d64a-137">originId</span><span class="sxs-lookup"><span data-stu-id="3d64a-137">originId</span></span>|<span data-ttu-id="3d64a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-138">String</span></span>|<span data-ttu-id="3d64a-139">O identificador exclusivo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="3d64a-139">The unique identifier of the resource in the origin system.</span></span> <span data-ttu-id="3d64a-140">No caso de um grupo do Azure AD, esse é o identificador do grupo.</span><span class="sxs-lookup"><span data-stu-id="3d64a-140">In the case of an Azure AD group, this is the identifier of the group.</span></span> |
|<span data-ttu-id="3d64a-141">originSystem</span><span class="sxs-lookup"><span data-stu-id="3d64a-141">originSystem</span></span>|<span data-ttu-id="3d64a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-142">String</span></span>|<span data-ttu-id="3d64a-143">O tipo do recurso no sistema de origem, `SharePointOnline` como, `AadApplication` ou `AadGroup` .</span><span class="sxs-lookup"><span data-stu-id="3d64a-143">The type of the resource in the origin system, such as `SharePointOnline`, `AadApplication` or `AadGroup`.</span></span>|
|<span data-ttu-id="3d64a-144">resourceType</span><span class="sxs-lookup"><span data-stu-id="3d64a-144">resourceType</span></span>|<span data-ttu-id="3d64a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-145">String</span></span>|<span data-ttu-id="3d64a-146">O tipo do recurso, como se fosse um aplicativo conectado ao Azure AD ou para um `Application` `SharePoint Online Site` site do SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3d64a-146">The type of the resource, such as `Application` if it is an Azure AD connected application, or `SharePoint Online Site` for a SharePoint Online site.</span></span>|
|<span data-ttu-id="3d64a-147">url</span><span class="sxs-lookup"><span data-stu-id="3d64a-147">url</span></span>|<span data-ttu-id="3d64a-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d64a-148">String</span></span>|<span data-ttu-id="3d64a-149">Um localizador de recurso exclusivo para o recurso, como a URL para entrar um usuário em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3d64a-149">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d64a-150">Relações</span><span class="sxs-lookup"><span data-stu-id="3d64a-150">Relationships</span></span>

| <span data-ttu-id="3d64a-151">Relação</span><span class="sxs-lookup"><span data-stu-id="3d64a-151">Relationship</span></span> | <span data-ttu-id="3d64a-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d64a-152">Type</span></span>        | <span data-ttu-id="3d64a-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d64a-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d64a-154">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="3d64a-154">accessPackageResourceRoles</span></span>|<span data-ttu-id="3d64a-155">[Coleção accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="3d64a-155">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="3d64a-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3d64a-156">Read-only.</span></span> <span data-ttu-id="3d64a-157">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3d64a-157">Nullable.</span></span>|
|<span data-ttu-id="3d64a-158">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="3d64a-158">accessPackageResourceScopes</span></span>|<span data-ttu-id="3d64a-159">[Coleção accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="3d64a-159">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="3d64a-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3d64a-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3d64a-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d64a-162">JSON representation</span></span>

<span data-ttu-id="3d64a-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d64a-163">The following is a JSON representation of the resource.</span></span>

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


