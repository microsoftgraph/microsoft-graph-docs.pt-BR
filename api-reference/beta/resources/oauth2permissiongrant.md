---
title: tipo de recurso oAuth2PermissionGrant
description: Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f00d9aa79e6a18e5dddf6881e251b3cbf00172e6
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543412"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="a4926-103">tipo de recurso oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="a4926-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4926-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4926-105">Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.</span><span class="sxs-lookup"><span data-stu-id="a4926-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

<span data-ttu-id="a4926-106">Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/oauth2permissiongrant-delta.md).</span><span class="sxs-lookup"><span data-stu-id="a4926-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="a4926-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a4926-107">Methods</span></span>

| <span data-ttu-id="a4926-108">Método</span><span class="sxs-lookup"><span data-stu-id="a4926-108">Method</span></span>           | <span data-ttu-id="a4926-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a4926-109">Return Type</span></span>    |<span data-ttu-id="a4926-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4926-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4926-111">Listar oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="a4926-111">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="a4926-112">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span><span class="sxs-lookup"><span data-stu-id="a4926-112">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="a4926-113">Recupere uma lista de objetos **oauth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="a4926-113">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="a4926-114">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-114">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="a4926-115">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-115">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a4926-116">Leia as propriedades e os relacionamentos de um objeto **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="a4926-116">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="a4926-117">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-117">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="a4926-118">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-118">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a4926-119">Atualize um objeto **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="a4926-119">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="a4926-120">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-120">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="a4926-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4926-121">None</span></span> |<span data-ttu-id="a4926-122">Excluir um objeto **oAuth2PermissionGrant** .</span><span class="sxs-lookup"><span data-stu-id="a4926-122">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="a4926-123">Obter delta</span><span class="sxs-lookup"><span data-stu-id="a4926-123">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="a4926-124">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a4926-124">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="a4926-125">Obter objetos **oauth2permissiongrant** recém-criados, atualizados ou excluídos sem executar uma leitura completa de toda a coleção de recursos.</span><span class="sxs-lookup"><span data-stu-id="a4926-125">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4926-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a4926-126">Properties</span></span>
| <span data-ttu-id="a4926-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a4926-127">Property</span></span>     | <span data-ttu-id="a4926-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4926-128">Type</span></span>   |<span data-ttu-id="a4926-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4926-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4926-130">clientId</span><span class="sxs-lookup"><span data-stu-id="a4926-130">clientId</span></span>|<span data-ttu-id="a4926-131">String</span><span class="sxs-lookup"><span data-stu-id="a4926-131">String</span></span>| <span data-ttu-id="a4926-132">A ID da entidade de serviço que recebe o consentimento para representar o usuário ao acessar o recurso (representado pela Propriedade ResourceId).</span><span class="sxs-lookup"><span data-stu-id="a4926-132">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="a4926-133">consentType</span><span class="sxs-lookup"><span data-stu-id="a4926-133">consentType</span></span>|<span data-ttu-id="a4926-134">String</span><span class="sxs-lookup"><span data-stu-id="a4926-134">String</span></span>| <span data-ttu-id="a4926-135">Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="a4926-135">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="a4926-136">Os valores possíveis são *Userdirigetes* ou *entidade de segurança*.</span><span class="sxs-lookup"><span data-stu-id="a4926-136">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="a4926-137">expiryTime</span><span class="sxs-lookup"><span data-stu-id="a4926-137">expiryTime</span></span>|<span data-ttu-id="a4926-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4926-138">DateTimeOffset</span></span>| <span data-ttu-id="a4926-139">No momento, o valor de tempo de expiração é ignorado.</span><span class="sxs-lookup"><span data-stu-id="a4926-139">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="a4926-140">id</span><span class="sxs-lookup"><span data-stu-id="a4926-140">id</span></span>|<span data-ttu-id="a4926-141">String</span><span class="sxs-lookup"><span data-stu-id="a4926-141">String</span></span>| <span data-ttu-id="a4926-142">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a4926-142">Unique identifier.</span></span> <span data-ttu-id="a4926-143">Apenas leitura.</span><span class="sxs-lookup"><span data-stu-id="a4926-143">Read-only.</span></span>|
|<span data-ttu-id="a4926-144">principalId</span><span class="sxs-lookup"><span data-stu-id="a4926-144">principalId</span></span>|<span data-ttu-id="a4926-145">String</span><span class="sxs-lookup"><span data-stu-id="a4926-145">String</span></span>| <span data-ttu-id="a4926-146">Se consenttype for *servicePrincipalName* , esse valor será nulo e o consentimento se aplicará a todos os usuários da organização.</span><span class="sxs-lookup"><span data-stu-id="a4926-146">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="a4926-147">Se consenttype for *principal*, essa propriedade especificará a ID do usuário que receberá o consentimento e se aplicará somente para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="a4926-147">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="a4926-148">resourceId</span><span class="sxs-lookup"><span data-stu-id="a4926-148">resourceId</span></span>|<span data-ttu-id="a4926-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4926-149">String</span></span>| <span data-ttu-id="a4926-150">Especifica a ID da entidade de serviço de recurso para a qual o acesso foi concedido.</span><span class="sxs-lookup"><span data-stu-id="a4926-150">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="a4926-151">escopo</span><span class="sxs-lookup"><span data-stu-id="a4926-151">scope</span></span>|<span data-ttu-id="a4926-152">String</span><span class="sxs-lookup"><span data-stu-id="a4926-152">String</span></span>| <span data-ttu-id="a4926-153">Especifica o valor da declaração do [escopo](/graph/permissions-reference) que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="a4926-153">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="a4926-154">Por exemplo, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="a4926-154">For example, *User.Read*</span></span> |
|<span data-ttu-id="a4926-155">startTime</span><span class="sxs-lookup"><span data-stu-id="a4926-155">startTime</span></span>|<span data-ttu-id="a4926-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4926-156">DateTimeOffset</span></span>| <span data-ttu-id="a4926-157">No momento, o valor de hora de início é ignorado.</span><span class="sxs-lookup"><span data-stu-id="a4926-157">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a4926-158">Relações</span><span class="sxs-lookup"><span data-stu-id="a4926-158">Relationships</span></span>
<span data-ttu-id="a4926-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a4926-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4926-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a4926-160">JSON representation</span></span>

<span data-ttu-id="a4926-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a4926-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
