---
title: tipo de recurso permissionScope
description: Representa um escopo de permissão delegada do OAuth 2,0.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: be8d9a7d08334bd716cfcbf565225add790b65e3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939366"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="75031-103">tipo de recurso permissionScope</span><span class="sxs-lookup"><span data-stu-id="75031-103">permissionScope resource type</span></span>

<span data-ttu-id="75031-104">Representa um escopo de permissão delegada do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="75031-104">Represents an OAuth 2.0 delegated permission scope.</span></span> <span data-ttu-id="75031-105">Os escopos de permissão delegada do OAuth 2,0 especificado podem ser solicitados por aplicativos cliente (por meio da coleção **requiredResourceAccess** no objeto [Application](application.md) ) ao chamar um aplicativo de recurso.</span><span class="sxs-lookup"><span data-stu-id="75031-105">The specified OAuth 2.0 delegated permission scopes may be requested by client applications (through the **requiredResourceAccess** collection on the [application](application.md) object) when calling a resource application.</span></span> <span data-ttu-id="75031-106">A propriedade **oauth2Permissions**</span><span class="sxs-lookup"><span data-stu-id="75031-106">The **oauth2Permissions** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="75031-107">a entidade do [aplicativo](application.md) é uma coleção de **permissionScope**.</span><span class="sxs-lookup"><span data-stu-id="75031-107">of the [Application](application.md) entity is a collection of **permissionScope**.</span></span>

## <a name="properties"></a><span data-ttu-id="75031-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75031-108">Properties</span></span>

| <span data-ttu-id="75031-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75031-109">Property</span></span> | <span data-ttu-id="75031-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75031-110">Type</span></span> | <span data-ttu-id="75031-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75031-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="75031-112">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="75031-112">adminConsentDescription</span></span>|<span data-ttu-id="75031-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-113">String</span></span>| <span data-ttu-id="75031-114">Texto de ajuda de permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="75031-114">Permission help text that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="75031-115">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="75031-115">adminConsentDisplayName</span></span>|<span data-ttu-id="75031-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-116">String</span></span>| <span data-ttu-id="75031-117">Nome para exibição da permissão que aparece nas experiências de atribuição de aplicativo e consentimento de administrador.</span><span class="sxs-lookup"><span data-stu-id="75031-117">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span> |
|<span data-ttu-id="75031-118">id</span><span class="sxs-lookup"><span data-stu-id="75031-118">id</span></span>|<span data-ttu-id="75031-119">Guid</span><span class="sxs-lookup"><span data-stu-id="75031-119">Guid</span></span>| <span data-ttu-id="75031-120">Identificador de permissão de escopo exclusivo dentro da coleção oauth2Permissions.</span><span class="sxs-lookup"><span data-stu-id="75031-120">Unique scope permission identifier inside the oauth2Permissions collection.</span></span> |
|<span data-ttu-id="75031-121">isEnabled</span><span class="sxs-lookup"><span data-stu-id="75031-121">isEnabled</span></span>|<span data-ttu-id="75031-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="75031-122">Boolean</span></span>| <span data-ttu-id="75031-123">Ao criar ou atualizar uma permissão, essa propriedade deve ser definida como **true** (que é o padrão).</span><span class="sxs-lookup"><span data-stu-id="75031-123">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="75031-124">Para excluir uma permissão, essa propriedade deve ser definida primeiro como **false**.</span><span class="sxs-lookup"><span data-stu-id="75031-124">To delete a permission, this property must first be set to **false**.</span></span> <span data-ttu-id="75031-125">Nesse ponto, em uma chamada subsequente, a permissão pode ser removida.</span><span class="sxs-lookup"><span data-stu-id="75031-125">At that point, in a subsequent call, the permission may be removed.</span></span> |
|<span data-ttu-id="75031-126">tenham</span><span class="sxs-lookup"><span data-stu-id="75031-126">origin</span></span>|<span data-ttu-id="75031-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-127">String</span></span>| <span data-ttu-id="75031-128">Para uso interno.</span><span class="sxs-lookup"><span data-stu-id="75031-128">For internal use.</span></span> |
|<span data-ttu-id="75031-129">type</span><span class="sxs-lookup"><span data-stu-id="75031-129">type</span></span>|<span data-ttu-id="75031-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-130">String</span></span>| <span data-ttu-id="75031-131">Especifica se essa permissão de escopo pode ser consentida por um usuário final ou se é uma permissão em todo o locatário que deve ser consentida pelo administrador da empresa.</span><span class="sxs-lookup"><span data-stu-id="75031-131">Specifies whether this scope permission can be consented to by an end user, or whether it is a tenant-wide permission that must be consented to by a company administrator.</span></span> <span data-ttu-id="75031-132">Os valores possíveis são *User* ou *admin*.</span><span class="sxs-lookup"><span data-stu-id="75031-132">Possible values are *User* or *Admin*.</span></span> |
|<span data-ttu-id="75031-133">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="75031-133">userConsentDescription</span></span>|<span data-ttu-id="75031-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-134">String</span></span>| <span data-ttu-id="75031-135">Texto de ajuda de permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="75031-135">Permission help text that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="75031-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="75031-136">userConsentDisplayName</span></span>|<span data-ttu-id="75031-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-137">String</span></span>| <span data-ttu-id="75031-138">Nome para exibição da permissão que aparece na experiência de consentimento do usuário final.</span><span class="sxs-lookup"><span data-stu-id="75031-138">Display name for the permission that appears in the end-user consent experience.</span></span> |
|<span data-ttu-id="75031-139">value</span><span class="sxs-lookup"><span data-stu-id="75031-139">value</span></span>|<span data-ttu-id="75031-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75031-140">String</span></span>| <span data-ttu-id="75031-141">O valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="75031-141">The value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75031-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75031-142">JSON representation</span></span>
<span data-ttu-id="75031-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75031-143">Here is a JSON representation of the resource.</span></span>

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
