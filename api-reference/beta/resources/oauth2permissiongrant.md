---
title: tipo de recurso de oAuth2PermissionGrant
description: Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516921"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="d29af-103">tipo de recurso de oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d29af-104">Representa os escopos de OAuth 2.0 (permissões delegadas) que tiverem sido concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento do usuário ou administrador.</span><span class="sxs-lookup"><span data-stu-id="d29af-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d29af-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d29af-105">JSON representation</span></span>

<span data-ttu-id="d29af-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d29af-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d29af-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d29af-107">Properties</span></span>
| <span data-ttu-id="d29af-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d29af-108">Property</span></span>     | <span data-ttu-id="d29af-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d29af-109">Type</span></span>   |<span data-ttu-id="d29af-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d29af-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d29af-111">clientId</span><span class="sxs-lookup"><span data-stu-id="d29af-111">clientId</span></span>|<span data-ttu-id="d29af-112">String</span><span class="sxs-lookup"><span data-stu-id="d29af-112">String</span></span>| <span data-ttu-id="d29af-113">A id da entidade de segurança do serviço concedido consentimento para representar o usuário ao acessar o recurso (representado pela propriedade resourceId).</span><span class="sxs-lookup"><span data-stu-id="d29af-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="d29af-114">consentType</span><span class="sxs-lookup"><span data-stu-id="d29af-114">consentType</span></span>|<span data-ttu-id="d29af-115">String</span><span class="sxs-lookup"><span data-stu-id="d29af-115">String</span></span>| <span data-ttu-id="d29af-116">Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="d29af-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="d29af-117">Os valores possíveis são "AllPrincipals" ou "Principal".</span><span class="sxs-lookup"><span data-stu-id="d29af-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="d29af-118">ExpiryTime</span><span class="sxs-lookup"><span data-stu-id="d29af-118">expiryTime</span></span>|<span data-ttu-id="d29af-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d29af-119">DateTimeOffset</span></span>| <span data-ttu-id="d29af-120">Atualmente, o valor de tempo de expiração será ignorado.</span><span class="sxs-lookup"><span data-stu-id="d29af-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="d29af-121">id</span><span class="sxs-lookup"><span data-stu-id="d29af-121">id</span></span>|<span data-ttu-id="d29af-122">String</span><span class="sxs-lookup"><span data-stu-id="d29af-122">String</span></span>| <span data-ttu-id="d29af-123">Identificador exclusivo</span><span class="sxs-lookup"><span data-stu-id="d29af-123">Unique identifier.</span></span> <span data-ttu-id="d29af-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d29af-124">Read-only.</span></span>|
|<span data-ttu-id="d29af-125">principalId</span><span class="sxs-lookup"><span data-stu-id="d29af-125">principalId</span></span>|<span data-ttu-id="d29af-126">String</span><span class="sxs-lookup"><span data-stu-id="d29af-126">String</span></span>| <span data-ttu-id="d29af-127">Este valor é null se consentType for *AllPrincipals* e o consentimento se aplica a todos os usuários na organização.</span><span class="sxs-lookup"><span data-stu-id="d29af-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="d29af-128">Se consentType for *Principal*, essa propriedade especifica a id do usuário que concedidas consentimento e aplica-se somente para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="d29af-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="d29af-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="d29af-129">resourceId</span></span>|<span data-ttu-id="d29af-130">String</span><span class="sxs-lookup"><span data-stu-id="d29af-130">String</span></span>| <span data-ttu-id="d29af-131">Especifica a id da entidade de serviço recurso ao qual tem permissão para acesso.</span><span class="sxs-lookup"><span data-stu-id="d29af-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="d29af-132">scope</span><span class="sxs-lookup"><span data-stu-id="d29af-132">scope</span></span>|<span data-ttu-id="d29af-133">String</span><span class="sxs-lookup"><span data-stu-id="d29af-133">String</span></span>| <span data-ttu-id="d29af-134">Especifica o valor da declaração [escopo](/graph/permissions-reference) que o aplicativo de recurso deve esperar que no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="d29af-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="d29af-135">Por exemplo, *User.Read*</span><span class="sxs-lookup"><span data-stu-id="d29af-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="d29af-136">startTime</span><span class="sxs-lookup"><span data-stu-id="d29af-136">startTime</span></span>|<span data-ttu-id="d29af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d29af-137">DateTimeOffset</span></span>| <span data-ttu-id="d29af-138">Atualmente, o valor de hora de início será ignorado.</span><span class="sxs-lookup"><span data-stu-id="d29af-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d29af-139">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="d29af-139">Relationships</span></span>
<span data-ttu-id="d29af-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d29af-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="d29af-141">Métodos</span><span class="sxs-lookup"><span data-stu-id="d29af-141">Methods</span></span>

| <span data-ttu-id="d29af-142">Método</span><span class="sxs-lookup"><span data-stu-id="d29af-142">Method</span></span>           | <span data-ttu-id="d29af-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d29af-143">Return Type</span></span>    |<span data-ttu-id="d29af-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="d29af-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d29af-145">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="d29af-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="d29af-147">Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="d29af-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="d29af-148">Lista oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="d29af-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="d29af-149">coleção [oAuth2PermissionGrant](oauth2permissiongrant.md)</span><span class="sxs-lookup"><span data-stu-id="d29af-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="d29af-150">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="d29af-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="d29af-151">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="d29af-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="d29af-153">Atualize o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="d29af-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="d29af-154">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="d29af-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="d29af-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d29af-155">None</span></span> |<span data-ttu-id="d29af-156">Exclua objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="d29af-156">Delete oAuth2PermissionGrant object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
