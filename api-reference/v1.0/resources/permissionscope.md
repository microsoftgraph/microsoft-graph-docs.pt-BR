---
title: tipo de recurso permissionScope
description: Representa um escopo de permissão delegada do OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bdc022f82f2e0dc7a1277d2674f215b58d521679
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447210"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="d918e-103">tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="d918e-103">permissionScope resource type</span></span>

<span data-ttu-id="d918e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d918e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d918e-105">Representa um escopo de permissão delegada do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d918e-105">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="d918e-106">Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="d918e-106">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="d918e-107">A propriedade **oauth2Permissions**</span><span class="sxs-lookup"><span data-stu-id="d918e-107">The **oauth2Permissions** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="d918e-108">a entidade do [aplicativo](application.md) é uma coleção de **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="d918e-108">of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="d918e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d918e-109">Properties</span></span>

| <span data-ttu-id="d918e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d918e-110">Property</span></span> | <span data-ttu-id="d918e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d918e-111">Type</span></span> | <span data-ttu-id="d918e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d918e-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d918e-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="d918e-113">adminConsentDescription</span></span>|<span data-ttu-id="d918e-114">String</span><span class="sxs-lookup"><span data-stu-id="d918e-114">String</span></span>| <span data-ttu-id="d918e-115">Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="d918e-115">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="d918e-116">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="d918e-116">adminConsentDisplayName</span></span>|<span data-ttu-id="d918e-117">String</span><span class="sxs-lookup"><span data-stu-id="d918e-117">String</span></span>| <span data-ttu-id="d918e-118">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="d918e-118">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="d918e-119">id</span><span class="sxs-lookup"><span data-stu-id="d918e-119">id</span></span>|<span data-ttu-id="d918e-120">Guid</span><span class="sxs-lookup"><span data-stu-id="d918e-120">Guid</span></span>| <span data-ttu-id="d918e-121">Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="d918e-121">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="d918e-122">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d918e-122">isEnabled</span></span>|<span data-ttu-id="d918e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d918e-123">Boolean</span></span>| <span data-ttu-id="d918e-124">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="d918e-124">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="d918e-125">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="d918e-125">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="d918e-126">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="d918e-126">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="d918e-127">tenham</span><span class="sxs-lookup"><span data-stu-id="d918e-127">origin</span></span>|<span data-ttu-id="d918e-128">String</span><span class="sxs-lookup"><span data-stu-id="d918e-128">String</span></span>| <span data-ttu-id="d918e-129">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="d918e-129">For internal use.</span></span> |
|<span data-ttu-id="d918e-130">type</span><span class="sxs-lookup"><span data-stu-id="d918e-130">type</span></span>|<span data-ttu-id="d918e-131">String</span><span class="sxs-lookup"><span data-stu-id="d918e-131">String</span></span>| <span data-ttu-id="d918e-132">Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="d918e-132">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="d918e-133">Os valores possíveis são *User* ou *admin*.</span><span class="sxs-lookup"><span data-stu-id="d918e-133">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="d918e-134">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="d918e-134">userConsentDescription</span></span>|<span data-ttu-id="d918e-135">String</span><span class="sxs-lookup"><span data-stu-id="d918e-135">String</span></span>| <span data-ttu-id="d918e-136">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="d918e-136">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="d918e-137">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="d918e-137">userConsentDisplayName</span></span>|<span data-ttu-id="d918e-138">String</span><span class="sxs-lookup"><span data-stu-id="d918e-138">String</span></span>| <span data-ttu-id="d918e-139">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="d918e-139">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="d918e-140">value</span><span class="sxs-lookup"><span data-stu-id="d918e-140">value</span></span>|<span data-ttu-id="d918e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d918e-141">String</span></span>| <span data-ttu-id="d918e-142">O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="d918e-142">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d918e-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d918e-143">JSON representation</span></span>
<span data-ttu-id="d918e-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d918e-144">Here is a JSON representation of the resource.</span></span>

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
