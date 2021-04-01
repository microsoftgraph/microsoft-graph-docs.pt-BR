---
title: Tipo de recurso builtInIdentityProvider
description: Representa provedores de identidade internos em um locatário do Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 5c806306e596a087a6c4006dc39b1804c130858a
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491066"
---
# <a name="builtinidentityprovider-resource-type"></a><span data-ttu-id="9a4fc-103">Tipo de recurso builtInIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="9a4fc-103">builtInIdentityProvider resource type</span></span>
<span data-ttu-id="9a4fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a4fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a4fc-105">Representa provedores de identidade integrados com [Identidades externas](/azure/active-directory/external-identities/)para um locatário do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-105">Represents built-in identity providers with [External Identities](/azure/active-directory/external-identities/) for an Azure Active Directory tenant.</span></span>

<span data-ttu-id="9a4fc-106">Para cenários do Azure AD B2B em um locatário do Azure AD, o tipo de provedor de identidade integrado pode ser um Azure Active Directory (AAD), conta Microsoft (MSA) ou senha única de email (EmailOTP).</span><span class="sxs-lookup"><span data-stu-id="9a4fc-106">For Azure AD B2B scenarios in an Azure AD tenant, the built in identity provider type can be an Azure Active Directory(AAD), Microsoft account(MSA) or email one-time passcode (EmailOTP).</span></span>

<span data-ttu-id="9a4fc-107">Este tipo herdará de [IdentityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="9a4fc-107">This type will inherit from [identityProviderBase](../resources/identityproviderbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9a4fc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9a4fc-108">Methods</span></span>

| <span data-ttu-id="9a4fc-109">Método</span><span class="sxs-lookup"><span data-stu-id="9a4fc-109">Method</span></span>       | <span data-ttu-id="9a4fc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9a4fc-110">Return Type</span></span>  |<span data-ttu-id="9a4fc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4fc-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a4fc-112">List</span><span class="sxs-lookup"><span data-stu-id="9a4fc-112">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="9a4fc-113">Coleção [identityProviderBase](../resources/identityproviderbase.md) </span><span class="sxs-lookup"><span data-stu-id="9a4fc-113">[identityProviderBase](../resources/identityproviderbase.md) collection</span></span>|<span data-ttu-id="9a4fc-114">Recuperar todos os provedores de identidade configurados em um locatário, incluindo os provedores de identidade integrados.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-114">Retrieve all identity providers configured in a tenant including the built-in identity providers.</span></span>|
|[<span data-ttu-id="9a4fc-115">Get</span><span class="sxs-lookup"><span data-stu-id="9a4fc-115">Get</span></span>](../api/identityproviderbase-get.md) |<span data-ttu-id="9a4fc-116">builtInIdentityProvider</span><span class="sxs-lookup"><span data-stu-id="9a4fc-116">builtInIdentityProvider</span></span>|<span data-ttu-id="9a4fc-117">Recuperar propriedades de um provedor de identidade integrado.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-117">Retrieve properties of an built-in identity provider.</span></span>|
|[<span data-ttu-id="9a4fc-118">Listar os tipos de provedor disponíveis</span><span class="sxs-lookup"><span data-stu-id="9a4fc-118">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="9a4fc-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a4fc-119">String collection</span></span>|<span data-ttu-id="9a4fc-120">Recuperar todos os tipos de provedor de identidade disponíveis no locatário.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-120">Retrieve all available identity provider types available in the tenant.</span></span>|

## <a name="properties"></a><span data-ttu-id="9a4fc-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a4fc-121">Properties</span></span>

|<span data-ttu-id="9a4fc-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a4fc-122">Property</span></span>|<span data-ttu-id="9a4fc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a4fc-123">Type</span></span>|<span data-ttu-id="9a4fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a4fc-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a4fc-125">id</span><span class="sxs-lookup"><span data-stu-id="9a4fc-125">id</span></span>|<span data-ttu-id="9a4fc-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a4fc-126">String</span></span>|<span data-ttu-id="9a4fc-127">O identificador do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-127">The identifier of the identity provider.</span></span> <span data-ttu-id="9a4fc-128">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="9a4fc-128">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span> <span data-ttu-id="9a4fc-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-129">Read-only.</span></span>|
|<span data-ttu-id="9a4fc-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9a4fc-130">displayName</span></span>|<span data-ttu-id="9a4fc-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a4fc-131">String</span></span>|<span data-ttu-id="9a4fc-132">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-132">The display name of the identity provider.</span></span> <span data-ttu-id="9a4fc-133">Herdado de [identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="9a4fc-133">Inherited from [identityProviderBase](../resources/identityproviderbase.md).</span></span>|
|<span data-ttu-id="9a4fc-134">identityProviderType</span><span class="sxs-lookup"><span data-stu-id="9a4fc-134">identityProviderType</span></span>|<span data-ttu-id="9a4fc-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a4fc-135">String</span></span>|<span data-ttu-id="9a4fc-136">A identidade do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-136">The identity provider type.</span></span> <span data-ttu-id="9a4fc-137">Para um cenário B2B, valores possíveis: `AADSignup`, `MicrosoftAccount`, `EmailOTP`.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-137">For a B2B scenario, possible values: `AADSignup`, `MicrosoftAccount`, `EmailOTP`.</span></span> <span data-ttu-id="9a4fc-138">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-138">Required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a4fc-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a4fc-139">JSON representation</span></span>

<span data-ttu-id="9a4fc-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a4fc-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```json
{
    "id": "String",
    "identityProviderType": "String",
    "displayName": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-03-30 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
 "description": "builtinIdentityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
