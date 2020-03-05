---
title: tipo de recurso oAuth2PermissionGrant
description: Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e43866c73b8ad92e56a6e907c5ef8c660ef56e22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522530"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="8a060-103">tipo de recurso oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="8a060-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8a060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a060-105">Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.</span><span class="sxs-lookup"><span data-stu-id="8a060-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a060-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a060-106">JSON representation</span></span>

<span data-ttu-id="8a060-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8a060-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8a060-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a060-108">Properties</span></span>
| <span data-ttu-id="8a060-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a060-109">Property</span></span>     | <span data-ttu-id="8a060-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a060-110">Type</span></span>   |<span data-ttu-id="8a060-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a060-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a060-112">clientId</span><span class="sxs-lookup"><span data-stu-id="8a060-112">clientId</span></span>|<span data-ttu-id="8a060-113">String</span><span class="sxs-lookup"><span data-stu-id="8a060-113">String</span></span>| <span data-ttu-id="8a060-114">A ID da entidade de serviço que recebe o consentimento para representar o usuário ao acessar o recurso (representado pela Propriedade ResourceId).</span><span class="sxs-lookup"><span data-stu-id="8a060-114">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="8a060-115">consentType</span><span class="sxs-lookup"><span data-stu-id="8a060-115">consentType</span></span>|<span data-ttu-id="8a060-116">String</span><span class="sxs-lookup"><span data-stu-id="8a060-116">String</span></span>| <span data-ttu-id="8a060-117">Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="8a060-117">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="8a060-118">Os valores possíveis são *Userdirigetes* ou *entidade de segurança*.</span><span class="sxs-lookup"><span data-stu-id="8a060-118">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="8a060-119">expiryTime</span><span class="sxs-lookup"><span data-stu-id="8a060-119">expiryTime</span></span>|<span data-ttu-id="8a060-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a060-120">DateTimeOffset</span></span>| <span data-ttu-id="8a060-121">No momento, o valor de tempo de expiração é ignorado.</span><span class="sxs-lookup"><span data-stu-id="8a060-121">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="8a060-122">id</span><span class="sxs-lookup"><span data-stu-id="8a060-122">id</span></span>|<span data-ttu-id="8a060-123">String</span><span class="sxs-lookup"><span data-stu-id="8a060-123">String</span></span>| <span data-ttu-id="8a060-124">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8a060-124">Unique identifier.</span></span> <span data-ttu-id="8a060-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8a060-125">Read-only.</span></span>|
|<span data-ttu-id="8a060-126">principalId</span><span class="sxs-lookup"><span data-stu-id="8a060-126">principalId</span></span>|<span data-ttu-id="8a060-127">String</span><span class="sxs-lookup"><span data-stu-id="8a060-127">String</span></span>| <span data-ttu-id="8a060-128">Se consenttype for *servicePrincipalName* , esse valor será nulo e o consentimento se aplicará a todos os usuários da organização.</span><span class="sxs-lookup"><span data-stu-id="8a060-128">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="8a060-129">Se consenttype for *principal*, essa propriedade especificará a ID do usuário que receberá o consentimento e se aplicará somente para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="8a060-129">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="8a060-130">resourceId</span><span class="sxs-lookup"><span data-stu-id="8a060-130">resourceId</span></span>|<span data-ttu-id="8a060-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a060-131">String</span></span>| <span data-ttu-id="8a060-132">Especifica a ID da entidade de serviço de recurso para a qual o acesso foi concedido.</span><span class="sxs-lookup"><span data-stu-id="8a060-132">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="8a060-133">escopo</span><span class="sxs-lookup"><span data-stu-id="8a060-133">scope</span></span>|<span data-ttu-id="8a060-134">String</span><span class="sxs-lookup"><span data-stu-id="8a060-134">String</span></span>| <span data-ttu-id="8a060-135">Especifica o valor da declaração do [escopo](/graph/permissions-reference) que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="8a060-135">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="8a060-136">Por exemplo, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="8a060-136">For example, *User.Read*</span></span> |
|<span data-ttu-id="8a060-137">startTime</span><span class="sxs-lookup"><span data-stu-id="8a060-137">startTime</span></span>|<span data-ttu-id="8a060-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a060-138">DateTimeOffset</span></span>| <span data-ttu-id="8a060-139">No momento, o valor de hora de início é ignorado.</span><span class="sxs-lookup"><span data-stu-id="8a060-139">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a060-140">Relações</span><span class="sxs-lookup"><span data-stu-id="8a060-140">Relationships</span></span>
<span data-ttu-id="8a060-141">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8a060-141">None</span></span>


## <a name="methods"></a><span data-ttu-id="8a060-142">Métodos</span><span class="sxs-lookup"><span data-stu-id="8a060-142">Methods</span></span>

| <span data-ttu-id="8a060-143">Método</span><span class="sxs-lookup"><span data-stu-id="8a060-143">Method</span></span>           | <span data-ttu-id="8a060-144">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8a060-144">Return Type</span></span>    |<span data-ttu-id="8a060-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a060-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a060-146">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-146">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="8a060-147">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-147">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="8a060-148">Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="8a060-148">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="8a060-149">Listar oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="8a060-149">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="8a060-150">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span><span class="sxs-lookup"><span data-stu-id="8a060-150">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="8a060-151">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="8a060-151">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="8a060-152">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-152">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="8a060-153">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-153">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="8a060-154">Atualize o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="8a060-154">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="8a060-155">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="8a060-155">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="8a060-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a060-156">None</span></span> |<span data-ttu-id="8a060-157">Exclua o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="8a060-157">Delete oAuth2PermissionGrant object.</span></span> |

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
