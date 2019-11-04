---
title: tipo de recurso permissionScope
description: Representa um escopo de permissão delegada do OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 53e777d3a545ed95c5a6010db7abc965d3b9cad5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939338"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="5d461-103">tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="5d461-103">permissionScope resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d461-104">Representa um escopo de permissão delegada do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="5d461-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="5d461-105">Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="5d461-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="5d461-106">A propriedade **oauth2Permissions** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="5d461-106">The **oauth2Permissions** property of the [servicePrincipal](serviceprincipal.md) entity and of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="5d461-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d461-107">Properties</span></span>

| <span data-ttu-id="5d461-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d461-108">Property</span></span> | <span data-ttu-id="5d461-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d461-109">Type</span></span> | <span data-ttu-id="5d461-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d461-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5d461-111">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="5d461-111">adminConsentDescription</span></span>|<span data-ttu-id="5d461-112">String</span><span class="sxs-lookup"><span data-stu-id="5d461-112">String</span></span>| <span data-ttu-id="5d461-113">Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="5d461-113">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="5d461-114">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="5d461-114">adminConsentDisplayName</span></span>|<span data-ttu-id="5d461-115">String</span><span class="sxs-lookup"><span data-stu-id="5d461-115">String</span></span>| <span data-ttu-id="5d461-116">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="5d461-116">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="5d461-117">id</span><span class="sxs-lookup"><span data-stu-id="5d461-117">id</span></span>|<span data-ttu-id="5d461-118">Guid</span><span class="sxs-lookup"><span data-stu-id="5d461-118">Guid</span></span>| <span data-ttu-id="5d461-119">Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="5d461-119">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="5d461-120">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5d461-120">isEnabled</span></span>|<span data-ttu-id="5d461-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d461-121">Boolean</span></span>| <span data-ttu-id="5d461-122">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="5d461-122">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="5d461-123">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="5d461-123">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="5d461-124">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="5d461-124">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="5d461-125">tenham</span><span class="sxs-lookup"><span data-stu-id="5d461-125">origin</span></span>|<span data-ttu-id="5d461-126">String</span><span class="sxs-lookup"><span data-stu-id="5d461-126">String</span></span>| <span data-ttu-id="5d461-127">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="5d461-127">For internal use.</span></span> |
|<span data-ttu-id="5d461-128">type</span><span class="sxs-lookup"><span data-stu-id="5d461-128">type</span></span>|<span data-ttu-id="5d461-129">String</span><span class="sxs-lookup"><span data-stu-id="5d461-129">String</span></span>| <span data-ttu-id="5d461-130">Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="5d461-130">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="5d461-131">Os valores possíveis são *User* ou *admin*.</span><span class="sxs-lookup"><span data-stu-id="5d461-131">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="5d461-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="5d461-132">userConsentDescription</span></span>|<span data-ttu-id="5d461-133">String</span><span class="sxs-lookup"><span data-stu-id="5d461-133">String</span></span>| <span data-ttu-id="5d461-134">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="5d461-134">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="5d461-135">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="5d461-135">userConsentDisplayName</span></span>|<span data-ttu-id="5d461-136">String</span><span class="sxs-lookup"><span data-stu-id="5d461-136">String</span></span>| <span data-ttu-id="5d461-137">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="5d461-137">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="5d461-138">value</span><span class="sxs-lookup"><span data-stu-id="5d461-138">value</span></span>|<span data-ttu-id="5d461-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d461-139">String</span></span>| <span data-ttu-id="5d461-140">O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="5d461-140">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d461-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d461-141">JSON representation</span></span>
<span data-ttu-id="5d461-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d461-142">Here is a JSON representation of the resource.</span></span>

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
