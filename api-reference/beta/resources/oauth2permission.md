---
title: tipo de recurso de oAuth2Permission
description: Representa um OAuth 2.0 delegada escopo de permissão. O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de aplicativo) ao chamar um aplicativo de recurso. A propriedade **appRoles** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **oAuth2Permission**.
localization_priority: Normal
ms.openlocfilehash: 420a7b181aa2590d3c5bc8eaa7f104251915ae0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829705"
---
# <a name="oauth2permission-resource-type"></a><span data-ttu-id="51a66-105">tipo de recurso de oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="51a66-105">oAuth2Permission resource type</span></span>

> <span data-ttu-id="51a66-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51a66-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51a66-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51a66-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51a66-108">Representa um OAuth 2.0 delegada escopo de permissão.</span><span class="sxs-lookup"><span data-stu-id="51a66-108">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="51a66-109">O OAuth 2.0 especificado escopos permissão delegada podem ser solicitados por aplicativos do cliente (por meio da coleção **requiredResourceAccess** no objeto de [aplicativo](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="51a66-109">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="51a66-110">A propriedade **appRoles** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **oAuth2Permission**.</span><span class="sxs-lookup"><span data-stu-id="51a66-110">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **oAuth2Permission**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="51a66-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51a66-111">JSON representation</span></span>

<span data-ttu-id="51a66-112">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="51a66-112">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="51a66-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51a66-113">Properties</span></span>
| <span data-ttu-id="51a66-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51a66-114">Property</span></span>     | <span data-ttu-id="51a66-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="51a66-115">Type</span></span>   |<span data-ttu-id="51a66-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="51a66-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51a66-117">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="51a66-117">adminConsentDescription</span></span>|<span data-ttu-id="51a66-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-118">String</span></span>|<span data-ttu-id="51a66-119">Texto de ajuda de permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="51a66-119">Permission help text that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="51a66-120">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="51a66-120">adminConsentDisplayName</span></span>|<span data-ttu-id="51a66-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-121">String</span></span>|<span data-ttu-id="51a66-122">Nome para exibição da permissão que aparece nas experiências de atribuição de consentimento e app admin.</span><span class="sxs-lookup"><span data-stu-id="51a66-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="51a66-123">id</span><span class="sxs-lookup"><span data-stu-id="51a66-123">id</span></span>|<span data-ttu-id="51a66-124">Guid</span><span class="sxs-lookup"><span data-stu-id="51a66-124">Guid</span></span>|<span data-ttu-id="51a66-125">Identificador de permissão de escopo exclusiva dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="51a66-125">Unique scope permission identifier inside the oauth2Permissions collection.</span></span>|
|<span data-ttu-id="51a66-126">isEnabled</span><span class="sxs-lookup"><span data-stu-id="51a66-126">isEnabled</span></span>|<span data-ttu-id="51a66-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="51a66-127">Boolean</span></span>|<span data-ttu-id="51a66-128">Ao criar ou atualizar uma permissão, essa propriedade deverá ser definida como **true** (o que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="51a66-128">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="51a66-129">Para excluir uma permissão, essa propriedade primeiro deve ser definida como **false**.</span><span class="sxs-lookup"><span data-stu-id="51a66-129">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="51a66-130">Nesse momento, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="51a66-130">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="51a66-131">type</span><span class="sxs-lookup"><span data-stu-id="51a66-131">type</span></span>|<span data-ttu-id="51a66-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-132">String</span></span>|<span data-ttu-id="51a66-133">Especifica se esta permissão de escopo pode ser consentiu por um usuário final, ou se é uma permissão de todo o inquilino deve ser consentiu por um administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="51a66-133">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a Company Administrator.</span></span>  <span data-ttu-id="51a66-134">Valores possíveis são "Usuário" ou "Admin".</span><span class="sxs-lookup"><span data-stu-id="51a66-134">Possible values are "User" or "Admin".</span></span>|
|<span data-ttu-id="51a66-135">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="51a66-135">userConsentDescription</span></span>|<span data-ttu-id="51a66-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-136">String</span></span>|<span data-ttu-id="51a66-137">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="51a66-137">Permission help text that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="51a66-138">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="51a66-138">userConsentDisplayName</span></span>|<span data-ttu-id="51a66-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-139">String</span></span>|<span data-ttu-id="51a66-140">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="51a66-140">Display name for the permission that appears in the end user consent experience.</span></span>|
|<span data-ttu-id="51a66-141">valor</span><span class="sxs-lookup"><span data-stu-id="51a66-141">value</span></span>|<span data-ttu-id="51a66-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51a66-142">String</span></span>|<span data-ttu-id="51a66-143">O valor da declaração escopo que deve esperar que o aplicativo de recurso no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="51a66-143">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
