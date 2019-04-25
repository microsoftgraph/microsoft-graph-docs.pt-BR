---
title: tipo de recurso oAuth2PermissionGrant
description: Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581524"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="33d53-103">tipo de recurso oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-103">oAuth2PermissionGrant resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33d53-104">Representa os escopos (permissões delegadas) do OAuth 2,0 que foram concedidos a um aplicativo (representado por uma entidade de serviço) como parte do processo de consentimento de administrador ou usuário.</span><span class="sxs-lookup"><span data-stu-id="33d53-104">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33d53-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33d53-105">JSON representation</span></span>

<span data-ttu-id="33d53-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="33d53-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="33d53-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33d53-107">Properties</span></span>
| <span data-ttu-id="33d53-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33d53-108">Property</span></span>     | <span data-ttu-id="33d53-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="33d53-109">Type</span></span>   |<span data-ttu-id="33d53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="33d53-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33d53-111">clientId</span><span class="sxs-lookup"><span data-stu-id="33d53-111">clientId</span></span>|<span data-ttu-id="33d53-112">String</span><span class="sxs-lookup"><span data-stu-id="33d53-112">String</span></span>| <span data-ttu-id="33d53-113">A ID da entidade de serviço que recebe o consentimento para representar o usuário ao acessar o recurso (representado pela propriedade reSourceid).</span><span class="sxs-lookup"><span data-stu-id="33d53-113">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="33d53-114">consentType</span><span class="sxs-lookup"><span data-stu-id="33d53-114">consentType</span></span>|<span data-ttu-id="33d53-115">String</span><span class="sxs-lookup"><span data-stu-id="33d53-115">String</span></span>| <span data-ttu-id="33d53-116">Indica se o consentimento foi fornecido pelo administrador (em nome da organização) ou por um indivíduo.</span><span class="sxs-lookup"><span data-stu-id="33d53-116">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="33d53-117">Os valores possíveis são \*\* userdirigetes ou *entidade de segurança*.</span><span class="sxs-lookup"><span data-stu-id="33d53-117">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="33d53-118">expiryTime</span><span class="sxs-lookup"><span data-stu-id="33d53-118">expiryTime</span></span>|<span data-ttu-id="33d53-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d53-119">DateTimeOffset</span></span>| <span data-ttu-id="33d53-120">No momento, o valor de tempo de expiração é ignorado.</span><span class="sxs-lookup"><span data-stu-id="33d53-120">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="33d53-121">id</span><span class="sxs-lookup"><span data-stu-id="33d53-121">id</span></span>|<span data-ttu-id="33d53-122">String</span><span class="sxs-lookup"><span data-stu-id="33d53-122">String</span></span>| <span data-ttu-id="33d53-123">Identificador exclusivo.</span><span class="sxs-lookup"><span data-stu-id="33d53-123">Unique identifier.</span></span> <span data-ttu-id="33d53-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="33d53-124">Read-only.</span></span>|
|<span data-ttu-id="33d53-125">principalId</span><span class="sxs-lookup"><span data-stu-id="33d53-125">principalId</span></span>|<span data-ttu-id="33d53-126">String</span><span class="sxs-lookup"><span data-stu-id="33d53-126">String</span></span>| <span data-ttu-id="33d53-127">Se consenttype for *servicePrincipalName* , esse valor será nulo e o consentimento se aplicará a todos os usuários da organização.</span><span class="sxs-lookup"><span data-stu-id="33d53-127">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="33d53-128">Se consenttype for *principal*, essa propriedade especificará a ID do usuário que receberá o consentimento e se aplicará somente para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="33d53-128">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="33d53-129">resourceId</span><span class="sxs-lookup"><span data-stu-id="33d53-129">resourceId</span></span>|<span data-ttu-id="33d53-130">String</span><span class="sxs-lookup"><span data-stu-id="33d53-130">String</span></span>| <span data-ttu-id="33d53-131">Especifica a ID da entidade de serviço de recurso para a qual o acesso foi concedido.</span><span class="sxs-lookup"><span data-stu-id="33d53-131">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="33d53-132">escopo</span><span class="sxs-lookup"><span data-stu-id="33d53-132">scope</span></span>|<span data-ttu-id="33d53-133">String</span><span class="sxs-lookup"><span data-stu-id="33d53-133">String</span></span>| <span data-ttu-id="33d53-134">Especifica o valor da declaração do [escopo](/graph/permissions-reference) que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="33d53-134">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="33d53-135">Por exemplo, *User. Read*</span><span class="sxs-lookup"><span data-stu-id="33d53-135">For example, *User.Read*</span></span> |
|<span data-ttu-id="33d53-136">startTime</span><span class="sxs-lookup"><span data-stu-id="33d53-136">startTime</span></span>|<span data-ttu-id="33d53-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d53-137">DateTimeOffset</span></span>| <span data-ttu-id="33d53-138">No momento, o valor de hora de início é ignorado.</span><span class="sxs-lookup"><span data-stu-id="33d53-138">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="33d53-139">Relações</span><span class="sxs-lookup"><span data-stu-id="33d53-139">Relationships</span></span>
<span data-ttu-id="33d53-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="33d53-140">None</span></span>


## <a name="methods"></a><span data-ttu-id="33d53-141">Métodos</span><span class="sxs-lookup"><span data-stu-id="33d53-141">Methods</span></span>

| <span data-ttu-id="33d53-142">Método</span><span class="sxs-lookup"><span data-stu-id="33d53-142">Method</span></span>           | <span data-ttu-id="33d53-143">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="33d53-143">Return Type</span></span>    |<span data-ttu-id="33d53-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="33d53-144">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="33d53-145">Obter oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-145">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="33d53-146">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-146">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="33d53-147">Leia as propriedades e os relacionamentos do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="33d53-147">Read properties and relationships of oAuth2PermissionGrant object.</span></span>|
|[<span data-ttu-id="33d53-148">Listar oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="33d53-148">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="33d53-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span><span class="sxs-lookup"><span data-stu-id="33d53-149">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="33d53-150">Recupere uma lista de objetos oauth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="33d53-150">Retrieve a list of oauth2PermissionGrant objects.</span></span> |
|[<span data-ttu-id="33d53-151">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-151">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="33d53-152">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-152">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="33d53-153">Atualize o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="33d53-153">Update oAuth2PermissionGrant object.</span></span> |
|[<span data-ttu-id="33d53-154">Excluir oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="33d53-154">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="33d53-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33d53-155">None</span></span> |<span data-ttu-id="33d53-156">Exclua o objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="33d53-156">Delete oAuth2PermissionGrant object.</span></span> |

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
