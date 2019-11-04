---
title: tipo de recurso accessPackageResource
description: Um recurso de pacote do Access é uma referência a um recurso associado a um catálogo as funções para as quais podem ser usadas em um ou mais pacotes de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e964a8ce2e9bd4165a29037a56ec4f95fe969422
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938923"
---
# <a name="accesspackageresource-resource-type"></a><span data-ttu-id="74c8b-103">tipo de recurso accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="74c8b-103">accessPackageResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74c8b-104">No [Azure ad pretitulation Management](entitlementmanagement-root.md), um recurso de pacote do Access é uma referência a um recurso associado a um catálogo as funções para as quais podem ser usadas em um ou mais pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="74c8b-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource is a reference to a resource associated with a catalog the roles for which can be used in one or more access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="74c8b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="74c8b-105">Methods</span></span>

| <span data-ttu-id="74c8b-106">Método</span><span class="sxs-lookup"><span data-stu-id="74c8b-106">Method</span></span>       | <span data-ttu-id="74c8b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74c8b-107">Return Type</span></span> | <span data-ttu-id="74c8b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c8b-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="74c8b-109">Listar recursos do accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="74c8b-109">List accessPackageCatalog resources</span></span>](../api/accesspackagecatalog-list-accesspackageresources.md) | <span data-ttu-id="74c8b-110">coleção [accessPackageResource](accesspackageresource.md)</span><span class="sxs-lookup"><span data-stu-id="74c8b-110">[accessPackageResource](accesspackageresource.md) collection</span></span> | <span data-ttu-id="74c8b-111">Recupere uma lista de objetos accesspackageresource.</span><span class="sxs-lookup"><span data-stu-id="74c8b-111">Retrieve a list of accesspackageresource objects.</span></span> |

## <a name="properties"></a><span data-ttu-id="74c8b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74c8b-112">Properties</span></span>

| <span data-ttu-id="74c8b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74c8b-113">Property</span></span>     | <span data-ttu-id="74c8b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c8b-114">Type</span></span>        | <span data-ttu-id="74c8b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c8b-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74c8b-116">addedBy</span><span class="sxs-lookup"><span data-stu-id="74c8b-116">addedBy</span></span>|<span data-ttu-id="74c8b-117">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-117">String</span></span>|<span data-ttu-id="74c8b-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74c8b-118">Read-only.</span></span>|
|<span data-ttu-id="74c8b-119">adicionado</span><span class="sxs-lookup"><span data-stu-id="74c8b-119">addedOn</span></span>|<span data-ttu-id="74c8b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74c8b-120">DateTimeOffset</span></span>|<span data-ttu-id="74c8b-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="74c8b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="74c8b-123">description</span><span class="sxs-lookup"><span data-stu-id="74c8b-123">description</span></span>|<span data-ttu-id="74c8b-124">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-124">String</span></span>|<span data-ttu-id="74c8b-125">Uma descrição do recurso.</span><span class="sxs-lookup"><span data-stu-id="74c8b-125">A description for the resource.</span></span>|
|<span data-ttu-id="74c8b-126">displayName</span><span class="sxs-lookup"><span data-stu-id="74c8b-126">displayName</span></span>|<span data-ttu-id="74c8b-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c8b-127">String</span></span>|<span data-ttu-id="74c8b-128">O nome de exibição do recurso, como o nome do aplicativo, o nome do grupo ou o nome do site.</span><span class="sxs-lookup"><span data-stu-id="74c8b-128">The display name of the resource, such as the application name, group name or site name.</span></span>|
|<span data-ttu-id="74c8b-129">id</span><span class="sxs-lookup"><span data-stu-id="74c8b-129">id</span></span>|<span data-ttu-id="74c8b-130">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-130">String</span></span>| <span data-ttu-id="74c8b-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74c8b-131">Read-only.</span></span>|
|<span data-ttu-id="74c8b-132">isPendingOnboarding</span><span class="sxs-lookup"><span data-stu-id="74c8b-132">isPendingOnboarding</span></span>|<span data-ttu-id="74c8b-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="74c8b-133">Boolean</span></span>|<span data-ttu-id="74c8b-134">True se o recurso ainda não está disponível para atribuição.</span><span class="sxs-lookup"><span data-stu-id="74c8b-134">True if the resource is not yet available for assignment.</span></span>|
|<span data-ttu-id="74c8b-135">originid</span><span class="sxs-lookup"><span data-stu-id="74c8b-135">originId</span></span>|<span data-ttu-id="74c8b-136">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-136">String</span></span>|<span data-ttu-id="74c8b-137">O identificador exclusivo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="74c8b-137">The unique identifier of the resource in the origin system.</span></span> |
|<span data-ttu-id="74c8b-138">originSystem</span><span class="sxs-lookup"><span data-stu-id="74c8b-138">originSystem</span></span>|<span data-ttu-id="74c8b-139">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-139">String</span></span>|<span data-ttu-id="74c8b-140">O tipo do recurso no sistema de origem.</span><span class="sxs-lookup"><span data-stu-id="74c8b-140">The type of the resource in the origin system.</span></span>|
|<span data-ttu-id="74c8b-141">resourceType</span><span class="sxs-lookup"><span data-stu-id="74c8b-141">resourceType</span></span>|<span data-ttu-id="74c8b-142">String</span><span class="sxs-lookup"><span data-stu-id="74c8b-142">String</span></span>|<span data-ttu-id="74c8b-143">O tipo do recurso, como `Application` se ele é um aplicativo conectado ao Azure AD.</span><span class="sxs-lookup"><span data-stu-id="74c8b-143">The type of the resource, such as `Application` if it is an Azure AD connected application.</span></span>|
|<span data-ttu-id="74c8b-144">url</span><span class="sxs-lookup"><span data-stu-id="74c8b-144">url</span></span>|<span data-ttu-id="74c8b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="74c8b-145">String</span></span>|<span data-ttu-id="74c8b-146">Um localizador de recursos exclusivo para o recurso, como a URL para assinar um usuário em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="74c8b-146">A unique resource locator for the resource, such as the URL for signing a user into an application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74c8b-147">Relações</span><span class="sxs-lookup"><span data-stu-id="74c8b-147">Relationships</span></span>

| <span data-ttu-id="74c8b-148">Relação</span><span class="sxs-lookup"><span data-stu-id="74c8b-148">Relationship</span></span> | <span data-ttu-id="74c8b-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="74c8b-149">Type</span></span>        | <span data-ttu-id="74c8b-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="74c8b-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74c8b-151">accessPackageResourceRoles</span><span class="sxs-lookup"><span data-stu-id="74c8b-151">accessPackageResourceRoles</span></span>|<span data-ttu-id="74c8b-152">coleção [accessPackageResourceRole](accesspackageresourcerole.md)</span><span class="sxs-lookup"><span data-stu-id="74c8b-152">[accessPackageResourceRole](accesspackageresourcerole.md) collection</span></span>| <span data-ttu-id="74c8b-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74c8b-153">Read-only.</span></span> <span data-ttu-id="74c8b-154">Anulável.</span><span class="sxs-lookup"><span data-stu-id="74c8b-154">Nullable.</span></span>|
|<span data-ttu-id="74c8b-155">accessPackageResourceScopes</span><span class="sxs-lookup"><span data-stu-id="74c8b-155">accessPackageResourceScopes</span></span>|<span data-ttu-id="74c8b-156">coleção [accessPackageResourceScope](accesspackageresourcescope.md)</span><span class="sxs-lookup"><span data-stu-id="74c8b-156">[accessPackageResourceScope](accesspackageresourcescope.md) collection</span></span>| <span data-ttu-id="74c8b-p103">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="74c8b-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="74c8b-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74c8b-159">JSON representation</span></span>

<span data-ttu-id="74c8b-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74c8b-160">The following is a JSON representation of the resource.</span></span>

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
