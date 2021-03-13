---
title: claimsMapping tipo de recurso
description: Mapeie as declarações de um token para as declarações que o Azure Active Directory B2C reconhece e usa.
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1863c6bf6f28e0e8ae8a3d1133330337a7420c0a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761839"
---
# <a name="claimsmapping-resource-type"></a><span data-ttu-id="a1eb4-103">claimsMapping tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="a1eb4-103">claimsMapping resource type</span></span>

<span data-ttu-id="a1eb4-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a1eb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1eb4-105">Depois que o provedor de identidade personalizado envia um token de ID de volta ao Azure AD B2C, o Azure AD B2C mapeia as declarações de um token para as declarações que o Azure AD B2C reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-105">After the custom identity provider sends an ID token back to Azure AD B2C, Azure AD B2C maps the claims from a token to the claims that Azure AD B2C recognizes and uses.</span></span>

## <a name="properties"></a><span data-ttu-id="a1eb4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1eb4-106">Properties</span></span>
|<span data-ttu-id="a1eb4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1eb4-107">Property</span></span>|<span data-ttu-id="a1eb4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1eb4-108">Type</span></span>|<span data-ttu-id="a1eb4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1eb4-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="a1eb4-110">userId</span><span class="sxs-lookup"><span data-stu-id="a1eb4-110">userId</span></span>|<span data-ttu-id="a1eb4-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1eb4-111">String</span></span>|<span data-ttu-id="a1eb4-112">A declaração que fornece o identificador exclusivo para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-112">The claim that provides the unique identifier for the signed-in user.</span></span> <span data-ttu-id="a1eb4-113">É uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-113">It is a required propoerty.</span></span>|
|<span data-ttu-id="a1eb4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="a1eb4-114">displayName</span></span>|<span data-ttu-id="a1eb4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1eb4-115">String</span></span>|<span data-ttu-id="a1eb4-116">A declaração que fornece o nome para exibição ou nome completo do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-116">The claim that provides the display name or full name for the user.</span></span> <span data-ttu-id="a1eb4-117">É uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-117">It is a required propoerty.</span></span>|
|<span data-ttu-id="a1eb4-118">givenName</span><span class="sxs-lookup"><span data-stu-id="a1eb4-118">givenName</span></span>|<span data-ttu-id="a1eb4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1eb4-119">String</span></span>|<span data-ttu-id="a1eb4-120">A declaração que fornece o primeiro nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-120">The claim that provides the first name of the user.</span></span>|
|<span data-ttu-id="a1eb4-121">surname</span><span class="sxs-lookup"><span data-stu-id="a1eb4-121">surname</span></span>|<span data-ttu-id="a1eb4-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1eb4-122">String</span></span>|<span data-ttu-id="a1eb4-123">A declaração que fornece o sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-123">The claim that provides the last name of the user.</span></span>|
|<span data-ttu-id="a1eb4-124">email</span><span class="sxs-lookup"><span data-stu-id="a1eb4-124">email</span></span>|<span data-ttu-id="a1eb4-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1eb4-125">String</span></span>|<span data-ttu-id="a1eb4-126">A declaração que fornece o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-126">The claim that provides the email address of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1eb4-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a1eb4-127">Relationships</span></span>
<span data-ttu-id="a1eb4-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1eb4-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1eb4-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1eb4-129">JSON representation</span></span>
<span data-ttu-id="a1eb4-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1eb4-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```


