---
title: tipo de recurso permissionScope
description: Representa um escopo de permissão delegada do OAuth 2,0. Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto Application) ao chamar um aplicativo de recurso. A propriedade **oauth2Permissions** da entidade servicePrincipalName e da entidade Application é uma coleção de **OAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 6f45d2eb0645991eb55db8ef3338e3b6fcf300a7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344950"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="c2e82-105">tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="c2e82-105">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2e82-106">Representa um escopo de permissão delegada do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="c2e82-106">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="c2e82-107">Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="c2e82-107">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="c2e82-108">A propriedade **oauth2Permissions** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="c2e82-108">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="c2e82-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2e82-109">Properties</span></span>

| <span data-ttu-id="c2e82-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2e82-110">Property</span></span> | <span data-ttu-id="c2e82-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2e82-111">Type</span></span> | <span data-ttu-id="c2e82-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2e82-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c2e82-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="c2e82-113">adminConsentDescription</span></span>|<span data-ttu-id="c2e82-114">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-114">String</span></span>| <span data-ttu-id="c2e82-115">Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="c2e82-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="c2e82-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2e82-116">adminConsentDisplayName</span></span>|<span data-ttu-id="c2e82-117">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-117">String</span></span>| <span data-ttu-id="c2e82-118">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="c2e82-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="c2e82-119">id</span><span class="sxs-lookup"><span data-stu-id="c2e82-119">id</span></span>|<span data-ttu-id="c2e82-120">Guid</span><span class="sxs-lookup"><span data-stu-id="c2e82-120">Guid</span></span>| <span data-ttu-id="c2e82-121">Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="c2e82-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="c2e82-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c2e82-122">isEnabled</span></span>|<span data-ttu-id="c2e82-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2e82-123">Boolean</span></span>| <span data-ttu-id="c2e82-124">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="c2e82-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="c2e82-125">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="c2e82-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="c2e82-126">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="c2e82-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="c2e82-127">tenham</span><span class="sxs-lookup"><span data-stu-id="c2e82-127">origin</span></span>|<span data-ttu-id="c2e82-128">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-128">String</span></span>| <span data-ttu-id="c2e82-129">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="c2e82-129">For internal use.</span></span> |
|<span data-ttu-id="c2e82-130">type</span><span class="sxs-lookup"><span data-stu-id="c2e82-130">type</span></span>|<span data-ttu-id="c2e82-131">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-131">String</span></span>| <span data-ttu-id="c2e82-132">Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="c2e82-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="c2e82-133">Os valores possíveis são *User* ou *admin*.</span><span class="sxs-lookup"><span data-stu-id="c2e82-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="c2e82-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="c2e82-134">userConsentDescription</span></span>|<span data-ttu-id="c2e82-135">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-135">String</span></span>| <span data-ttu-id="c2e82-136">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="c2e82-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="c2e82-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2e82-137">userConsentDisplayName</span></span>|<span data-ttu-id="c2e82-138">String</span><span class="sxs-lookup"><span data-stu-id="c2e82-138">String</span></span>| <span data-ttu-id="c2e82-139">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="c2e82-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="c2e82-140">value</span><span class="sxs-lookup"><span data-stu-id="c2e82-140">value</span></span>|<span data-ttu-id="c2e82-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2e82-141">String</span></span>| <span data-ttu-id="c2e82-142">O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="c2e82-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2e82-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2e82-143">JSON representation</span></span>
<span data-ttu-id="c2e82-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2e82-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
