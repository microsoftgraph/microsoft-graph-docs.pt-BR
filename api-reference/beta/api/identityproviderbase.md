---
title: Tipo de recurso identityProviderBase
description: Representa provedores de identidade em um locatário do Azure Active Directory e um locatário do B2C do Azure AD
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 71c6d58e9ad70773df39adc7d2a91393d64cd460
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491045"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="18a46-103">Tipo de recurso identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="18a46-103">identityProviderBase resource type</span></span>
<span data-ttu-id="18a46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18a46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18a46-105">Representa provedores de identidade com [Identidades externas](/azure/active-directory/external-identities/) para locatário do Azure Active Directory e um locatário do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="18a46-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="18a46-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="18a46-106">Methods</span></span>

| <span data-ttu-id="18a46-107">Método</span><span class="sxs-lookup"><span data-stu-id="18a46-107">Method</span></span>       | <span data-ttu-id="18a46-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18a46-108">Return Type</span></span>  |<span data-ttu-id="18a46-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a46-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="18a46-110">List</span><span class="sxs-lookup"><span data-stu-id="18a46-110">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="18a46-111">Coleção identityProviderBase</span><span class="sxs-lookup"><span data-stu-id="18a46-111">identityProviderBase collection</span></span>|<span data-ttu-id="18a46-112">Recupere todos os provedores de identidade configurados em um locatário.</span><span class="sxs-lookup"><span data-stu-id="18a46-112">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="18a46-113">Listar os tipos de provedor disponíveis</span><span class="sxs-lookup"><span data-stu-id="18a46-113">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="18a46-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a46-114">String collection</span></span>|<span data-ttu-id="18a46-115">Recupere todos os tipos de provedor de identidade disponíveis.</span><span class="sxs-lookup"><span data-stu-id="18a46-115">Retrieve all available identity provider types.</span></span>|

## <a name="properties"></a><span data-ttu-id="18a46-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18a46-116">Properties</span></span>

|<span data-ttu-id="18a46-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18a46-117">Property</span></span>|<span data-ttu-id="18a46-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="18a46-118">Type</span></span>|<span data-ttu-id="18a46-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="18a46-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18a46-120">id</span><span class="sxs-lookup"><span data-stu-id="18a46-120">id</span></span>|<span data-ttu-id="18a46-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a46-121">String</span></span>|<span data-ttu-id="18a46-122">O ID do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="18a46-122">The ID of the identity provider.</span></span>|
|<span data-ttu-id="18a46-123">displayName</span><span class="sxs-lookup"><span data-stu-id="18a46-123">displayName</span></span>|<span data-ttu-id="18a46-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18a46-124">String</span></span>|<span data-ttu-id="18a46-125">O nome de exibição exclusivo do provedor de identidade.</span><span class="sxs-lookup"><span data-stu-id="18a46-125">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18a46-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18a46-126">JSON representation</span></span>

<span data-ttu-id="18a46-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18a46-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
