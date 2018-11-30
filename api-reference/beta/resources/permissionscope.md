---
title: tipo de recurso de permissionScope
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **oauth2Permissions** da entidade ServicePrincipal e da entidade do aplicativo é uma coleção de **OAuth2Permission**.
ms.openlocfilehash: b15ee9901632fca113d944000847c953e85be58c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038639"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="e48cd-105">tipo de recurso de permissionScope</span><span class="sxs-lookup"><span data-stu-id="e48cd-105">permissionScope resource type</span></span>

> <span data-ttu-id="e48cd-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e48cd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e48cd-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e48cd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e48cd-108">Representa um OAuth 2.0 delegada escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="e48cd-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="e48cd-109">O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="e48cd-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [Application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="e48cd-110">A propriedade **oauth2Permissions** da entidade [ServicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **OAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="e48cd-110">The **oauth2Permissions** property of the [ServicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **OAuth2Permission**.</span></span>

## <a name="properties"></a><span data-ttu-id="e48cd-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e48cd-111">Properties</span></span>

| <span data-ttu-id="e48cd-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e48cd-112">Property</span></span> | <span data-ttu-id="e48cd-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e48cd-113">Type</span></span> | <span data-ttu-id="e48cd-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e48cd-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e48cd-115">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e48cd-115">adminConsentDescription</span></span>|<span data-ttu-id="e48cd-116">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-116">String</span></span>| <span data-ttu-id="e48cd-117">Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="e48cd-117">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="e48cd-118">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e48cd-118">adminConsentDisplayName</span></span>|<span data-ttu-id="e48cd-119">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-119">String</span></span>| <span data-ttu-id="e48cd-120">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="e48cd-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="e48cd-121">id</span><span class="sxs-lookup"><span data-stu-id="e48cd-121">id</span></span>|<span data-ttu-id="e48cd-122">Guid</span><span class="sxs-lookup"><span data-stu-id="e48cd-122">Guid</span></span>| <span data-ttu-id="e48cd-123">Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="e48cd-123">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="e48cd-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e48cd-124">isEnabled</span></span>|<span data-ttu-id="e48cd-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e48cd-125">Boolean</span></span>| <span data-ttu-id="e48cd-126">Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="e48cd-126">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="e48cd-127">Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="e48cd-127">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="e48cd-128">Nesse momento, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="e48cd-128">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="e48cd-129">origem</span><span class="sxs-lookup"><span data-stu-id="e48cd-129">origin</span></span>|<span data-ttu-id="e48cd-130">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-130">String</span></span>| <span data-ttu-id="e48cd-131">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="e48cd-131">For internal use.</span></span> |
|<span data-ttu-id="e48cd-132">type</span><span class="sxs-lookup"><span data-stu-id="e48cd-132">type</span></span>|<span data-ttu-id="e48cd-133">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-133">String</span></span>| <span data-ttu-id="e48cd-134">Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="e48cd-134">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="e48cd-135">Valores possíveis são o *usuário* ou *administrador*.</span><span class="sxs-lookup"><span data-stu-id="e48cd-135">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="e48cd-136">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="e48cd-136">userConsentDescription</span></span>|<span data-ttu-id="e48cd-137">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-137">String</span></span>| <span data-ttu-id="e48cd-138">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="e48cd-138">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="e48cd-139">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="e48cd-139">userConsentDisplayName</span></span>|<span data-ttu-id="e48cd-140">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-140">String</span></span>| <span data-ttu-id="e48cd-141">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="e48cd-141">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="e48cd-142">valor</span><span class="sxs-lookup"><span data-stu-id="e48cd-142">value</span></span>|<span data-ttu-id="e48cd-143">String</span><span class="sxs-lookup"><span data-stu-id="e48cd-143">String</span></span>| <span data-ttu-id="e48cd-144">O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="e48cd-144">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e48cd-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e48cd-145">JSON representation</span></span>
<span data-ttu-id="e48cd-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e48cd-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->