---
title: tipo de recurso de oAuth2Permission
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 8d8bb0bb5af17b7322bd6be37ac48ae9edbeba42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510810"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="9bdbd-105">tipo de recurso de oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="9bdbd-105">oAuth2Permission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bdbd-106">Representa um OAuth 2.0 delegada escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="9bdbd-107">O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="9bdbd-108">A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-108">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9bdbd-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bdbd-109">JSON representation</span></span>

<span data-ttu-id="9bdbd-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9bdbd-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9bdbd-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bdbd-111">Properties</span></span>
| <span data-ttu-id="9bdbd-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bdbd-112">Property</span></span>     | <span data-ttu-id="9bdbd-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bdbd-113">Type</span></span>   |<span data-ttu-id="9bdbd-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bdbd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9bdbd-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9bdbd-115">adminConsentDescription</span></span>|<span data-ttu-id="9bdbd-116">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-116">String</span></span>|<span data-ttu-id="9bdbd-117">Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="9bdbd-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9bdbd-118">adminConsentDisplayName</span></span>|<span data-ttu-id="9bdbd-119">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-119">String</span></span>|<span data-ttu-id="9bdbd-120">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="9bdbd-121">id</span><span class="sxs-lookup"><span data-stu-id="9bdbd-121">id</span></span>|<span data-ttu-id="9bdbd-122">Guid</span><span class="sxs-lookup"><span data-stu-id="9bdbd-122">Guid</span></span>|<span data-ttu-id="9bdbd-123">Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="9bdbd-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9bdbd-124">isEnabled</span></span>|<span data-ttu-id="9bdbd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bdbd-125">Boolean</span></span>|<span data-ttu-id="9bdbd-126">Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="9bdbd-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="9bdbd-127">Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-127">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="9bdbd-128">Nesse momento, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-128">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="9bdbd-129">type</span><span class="sxs-lookup"><span data-stu-id="9bdbd-129">type</span></span>|<span data-ttu-id="9bdbd-130">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-130">String</span></span>|<span data-ttu-id="9bdbd-131">Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="9bdbd-132">Valores possíveis são "Usuário" ou "Admin".</span><span class="sxs-lookup"><span data-stu-id="9bdbd-132">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="9bdbd-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="9bdbd-133">userConsentDescription</span></span>|<span data-ttu-id="9bdbd-134">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-134">String</span></span>|<span data-ttu-id="9bdbd-135">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-135">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="9bdbd-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="9bdbd-136">userConsentDisplayName</span></span>|<span data-ttu-id="9bdbd-137">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-137">String</span></span>|<span data-ttu-id="9bdbd-138">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-138">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="9bdbd-139">valor</span><span class="sxs-lookup"><span data-stu-id="9bdbd-139">value</span></span>|<span data-ttu-id="9bdbd-140">String</span><span class="sxs-lookup"><span data-stu-id="9bdbd-140">String</span></span>|<span data-ttu-id="9bdbd-141">O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="9bdbd-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

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
