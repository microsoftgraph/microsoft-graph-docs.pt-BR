---
title: tipo de recurso de permissionScope
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **oauth2Permissions** da entidade ServicePrincipal e da entidade do aplicativo é uma coleção de **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517075"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="50f1d-105">tipo de recurso de permissionScope</span><span class="sxs-lookup"><span data-stu-id="50f1d-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50f1d-106">Representa um OAuth 2.0 delegada escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="50f1d-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="50f1d-107">O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="50f1d-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="50f1d-108">A propriedade **oauth2Permissions** da entidade [ServicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="50f1d-108">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="50f1d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50f1d-109">Properties</span></span>

| <span data-ttu-id="50f1d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50f1d-110">Property</span></span> | <span data-ttu-id="50f1d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="50f1d-111">Type</span></span> | <span data-ttu-id="50f1d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="50f1d-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="50f1d-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="50f1d-113">adminConsentDescription</span></span>|<span data-ttu-id="50f1d-114">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-114">String</span></span>| <span data-ttu-id="50f1d-115">Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="50f1d-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="50f1d-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="50f1d-116">adminConsentDisplayName</span></span>|<span data-ttu-id="50f1d-117">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-117">String</span></span>| <span data-ttu-id="50f1d-118">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="50f1d-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="50f1d-119">id</span><span class="sxs-lookup"><span data-stu-id="50f1d-119">id</span></span>|<span data-ttu-id="50f1d-120">Guid</span><span class="sxs-lookup"><span data-stu-id="50f1d-120">Guid</span></span>| <span data-ttu-id="50f1d-121">Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="50f1d-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="50f1d-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="50f1d-122">isEnabled</span></span>|<span data-ttu-id="50f1d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f1d-123">Boolean</span></span>| <span data-ttu-id="50f1d-124">Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="50f1d-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="50f1d-125">Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="50f1d-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="50f1d-126">Nesse momento, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="50f1d-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="50f1d-127">Origin</span><span class="sxs-lookup"><span data-stu-id="50f1d-127">origin</span></span>|<span data-ttu-id="50f1d-128">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-128">String</span></span>| <span data-ttu-id="50f1d-129">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="50f1d-129">For internal use.</span></span> |
|<span data-ttu-id="50f1d-130">type</span><span class="sxs-lookup"><span data-stu-id="50f1d-130">type</span></span>|<span data-ttu-id="50f1d-131">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-131">String</span></span>| <span data-ttu-id="50f1d-132">Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="50f1d-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="50f1d-133">Valores possíveis são o *usuário* ou *administrador*.</span><span class="sxs-lookup"><span data-stu-id="50f1d-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="50f1d-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="50f1d-134">userConsentDescription</span></span>|<span data-ttu-id="50f1d-135">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-135">String</span></span>| <span data-ttu-id="50f1d-136">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="50f1d-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="50f1d-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="50f1d-137">userConsentDisplayName</span></span>|<span data-ttu-id="50f1d-138">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-138">String</span></span>| <span data-ttu-id="50f1d-139">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="50f1d-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="50f1d-140">valor</span><span class="sxs-lookup"><span data-stu-id="50f1d-140">value</span></span>|<span data-ttu-id="50f1d-141">String</span><span class="sxs-lookup"><span data-stu-id="50f1d-141">String</span></span>| <span data-ttu-id="50f1d-142">O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="50f1d-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50f1d-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50f1d-143">JSON representation</span></span>
<span data-ttu-id="50f1d-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50f1d-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
