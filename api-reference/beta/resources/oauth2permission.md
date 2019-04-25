---
title: tipo de recurso oAuth2Permission
description: Representa um escopo de permissão delegada do OAuth 2,0. Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto Application) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade servicePrincipalName e da entidade Application é uma coleção de **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581664"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="0309f-105">tipo de recurso oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="0309f-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0309f-106">Representa um escopo de permissão delegada do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="0309f-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="0309f-107">Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="0309f-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="0309f-108">A propriedade **appRoles** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="0309f-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0309f-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0309f-109">JSON representation</span></span>

<span data-ttu-id="0309f-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0309f-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="0309f-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0309f-111">Properties</span></span>
| <span data-ttu-id="0309f-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0309f-112">Property</span></span>     | <span data-ttu-id="0309f-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="0309f-113">Type</span></span>   |<span data-ttu-id="0309f-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="0309f-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0309f-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="0309f-115">adminConsentDescription</span></span>|<span data-ttu-id="0309f-116">String</span><span class="sxs-lookup"><span data-stu-id="0309f-116">String</span></span>|<span data-ttu-id="0309f-117">Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="0309f-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="0309f-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="0309f-118">adminConsentDisplayName</span></span>|<span data-ttu-id="0309f-119">String</span><span class="sxs-lookup"><span data-stu-id="0309f-119">String</span></span>|<span data-ttu-id="0309f-120">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="0309f-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="0309f-121">id</span><span class="sxs-lookup"><span data-stu-id="0309f-121">id</span></span>|<span data-ttu-id="0309f-122">Guid</span><span class="sxs-lookup"><span data-stu-id="0309f-122">Guid</span></span>|<span data-ttu-id="0309f-123">Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="0309f-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="0309f-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0309f-124">isEnabled</span></span>|<span data-ttu-id="0309f-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0309f-125">Boolean</span></span>|<span data-ttu-id="0309f-126">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="0309f-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="0309f-127">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="0309f-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="0309f-128">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="0309f-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="0309f-129">type</span><span class="sxs-lookup"><span data-stu-id="0309f-129">type</span></span>|<span data-ttu-id="0309f-130">String</span><span class="sxs-lookup"><span data-stu-id="0309f-130">String</span></span>|<span data-ttu-id="0309f-131">Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="0309f-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="0309f-132">Os valores possíveis são "user" ou "admin".</span><span class="sxs-lookup"><span data-stu-id="0309f-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="0309f-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="0309f-133">userConsentDescription</span></span>|<span data-ttu-id="0309f-134">String</span><span class="sxs-lookup"><span data-stu-id="0309f-134">String</span></span>|<span data-ttu-id="0309f-135">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0309f-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="0309f-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="0309f-136">userConsentDisplayName</span></span>|<span data-ttu-id="0309f-137">String</span><span class="sxs-lookup"><span data-stu-id="0309f-137">String</span></span>|<span data-ttu-id="0309f-138">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="0309f-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="0309f-139">value</span><span class="sxs-lookup"><span data-stu-id="0309f-139">value</span></span>|<span data-ttu-id="0309f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0309f-140">String</span></span>|<span data-ttu-id="0309f-141">O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="0309f-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
