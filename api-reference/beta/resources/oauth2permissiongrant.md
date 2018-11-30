---
title: tipo de recurso de oAuth2PermissionGrant
description: Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.
ms.openlocfilehash: 8fc5154ddba1b78976dc3e24c6712f9fc8944f43
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034344"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="5a041-103">tipo de recurso de oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-103">oAuth2PermissionGrant resource type</span></span>

> <span data-ttu-id="5a041-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a041-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a041-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a041-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a041-106">Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.</span><span class="sxs-lookup"><span data-stu-id="5a041-106">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a041-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a041-107">JSON representation</span></span>

<span data-ttu-id="5a041-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5a041-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
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
## <a name="properties"></a><span data-ttu-id="5a041-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a041-109">Properties</span></span>
| <span data-ttu-id="5a041-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a041-110">Property</span></span>     | <span data-ttu-id="5a041-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a041-111">Type</span></span>   |<span data-ttu-id="5a041-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a041-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a041-113">clientId</span><span class="sxs-lookup"><span data-stu-id="5a041-113">clientId</span></span>|<span data-ttu-id="5a041-114">String</span><span class="sxs-lookup"><span data-stu-id="5a041-114">String</span></span>| <span data-ttu-id="5a041-115">A id da entidade de segurança do serviço concedido consentimento para representar o usuário ao acessar o recurso (representado pela propriedade resourceId).</span><span class="sxs-lookup"><span data-stu-id="5a041-115">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="5a041-116">consentType</span><span class="sxs-lookup"><span data-stu-id="5a041-116">consentType</span></span>|<span data-ttu-id="5a041-117">String</span><span class="sxs-lookup"><span data-stu-id="5a041-117">String</span></span>| <span data-ttu-id="5a041-118">Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="5a041-118">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="5a041-119">Os valores possíveis são *AllPrincipals* ou *Principal*.</span><span class="sxs-lookup"><span data-stu-id="5a041-119">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="5a041-120">expiryTime</span><span class="sxs-lookup"><span data-stu-id="5a041-120">expiryTime</span></span>|<span data-ttu-id="5a041-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a041-121">DateTimeOffset</span></span>| <span data-ttu-id="5a041-122">Atualmente, o valor de tempo de expiração será ignorado.</span><span class="sxs-lookup"><span data-stu-id="5a041-122">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="5a041-123">id</span><span class="sxs-lookup"><span data-stu-id="5a041-123">id</span></span>|<span data-ttu-id="5a041-124">String</span><span class="sxs-lookup"><span data-stu-id="5a041-124">String</span></span>| <span data-ttu-id="5a041-125">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5a041-125">Unique identifier.</span></span> <span data-ttu-id="5a041-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a041-126">Read-only.</span></span>|
|<span data-ttu-id="5a041-127">principalId</span><span class="sxs-lookup"><span data-stu-id="5a041-127">principalId</span></span>|<span data-ttu-id="5a041-128">String</span><span class="sxs-lookup"><span data-stu-id="5a041-128">String</span></span>| <span data-ttu-id="5a041-129">Este valor é null se consentType for *AllPrincipals* e o consentimento se aplica a todos os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="5a041-129">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="5a041-130">Se consentType for *Principal*, essa propriedade especifica a id do usuário que concedidas consentimento e aplica-se somente para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5a041-130">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="5a041-131">resourceId</span><span class="sxs-lookup"><span data-stu-id="5a041-131">resourceId</span></span>|<span data-ttu-id="5a041-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a041-132">String</span></span>| <span data-ttu-id="5a041-133">Especifica a id da entidade de serviço recurso ao qual tem permissão para acesso.</span><span class="sxs-lookup"><span data-stu-id="5a041-133">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="5a041-134">scope</span><span class="sxs-lookup"><span data-stu-id="5a041-134">scope</span></span>|<span data-ttu-id="5a041-135">String</span><span class="sxs-lookup"><span data-stu-id="5a041-135">String</span></span>| <span data-ttu-id="5a041-136">Especifica o valor da declaração [escopo](/graph/permissions-reference) que o aplicativo de recurso deve esperar que no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="5a041-136">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="5a041-137">Por exemplo, *User.Read*</span><span class="sxs-lookup"><span data-stu-id="5a041-137">For example, *User.Read*</span></span> |
|<span data-ttu-id="5a041-138">startTime</span><span class="sxs-lookup"><span data-stu-id="5a041-138">startTime</span></span>|<span data-ttu-id="5a041-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a041-139">DateTimeOffset</span></span>| <span data-ttu-id="5a041-140">Atualmente, o valor de hora de início será ignorado.</span><span class="sxs-lookup"><span data-stu-id="5a041-140">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5a041-141">Relações</span><span class="sxs-lookup"><span data-stu-id="5a041-141">Relationships</span></span>
<span data-ttu-id="5a041-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a041-142">None</span></span>


## <a name="methods"></a><span data-ttu-id="5a041-143">Métodos</span><span class="sxs-lookup"><span data-stu-id="5a041-143">Methods</span></span>

| <span data-ttu-id="5a041-144">Método</span><span class="sxs-lookup"><span data-stu-id="5a041-144">Method</span></span>           | <span data-ttu-id="5a041-145">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5a041-145">Return Type</span></span>    |<span data-ttu-id="5a041-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a041-146">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a041-147">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-147">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="5a041-148">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-148">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="5a041-149">Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="5a041-149">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="5a041-150">Lista oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="5a041-150">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="5a041-151">coleção [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="5a041-151">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="5a041-152">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="5a041-152">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="5a041-153">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-153">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="5a041-154">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-154">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="5a041-155">Atualize o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="5a041-155">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="5a041-156">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5a041-156">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="5a041-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a041-157">None</span></span> |<span data-ttu-id="5a041-158">Exclua objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="5a041-158">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->