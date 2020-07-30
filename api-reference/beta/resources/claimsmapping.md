---
title: claimsMapping tipo de recurso
description: Mapeie as declarações de um token para as declarações que o Azure Active Directory B2C reconhece e usa.
author: namkedia
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fd47f751c71038158761b37721ad8a0d8831eb7d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509972"
---
# <a name="claimsmapping-resource-type"></a><span data-ttu-id="2d379-103">claimsMapping tipo de recurso</span><span class="sxs-lookup"><span data-stu-id="2d379-103">claimsMapping resource type</span></span>

<span data-ttu-id="2d379-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2d379-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d379-105">Depois que o provedor de identidade personalizado envia um token de ID de volta ao Azure AD B2C, o Azure AD B2C mapeia as declarações de um token para as declarações que o Azure AD B2C reconhece e usa.</span><span class="sxs-lookup"><span data-stu-id="2d379-105">After the custom identity provider sends an ID token back to Azure AD B2C, Azure AD B2C maps the claims from a token to the claims that Azure AD B2C recognizes and uses.</span></span>

## <a name="properties"></a><span data-ttu-id="2d379-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d379-106">Properties</span></span>
|<span data-ttu-id="2d379-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d379-107">Property</span></span>|<span data-ttu-id="2d379-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d379-108">Type</span></span>|<span data-ttu-id="2d379-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d379-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="2d379-110">userId</span><span class="sxs-lookup"><span data-stu-id="2d379-110">userId</span></span>|<span data-ttu-id="2d379-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d379-111">String</span></span>|<span data-ttu-id="2d379-112">A declaração que fornece o identificador exclusivo para o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2d379-112">The claim that provides the unique identifier for the signed-in user.</span></span> <span data-ttu-id="2d379-113">É uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="2d379-113">It is a required propoerty.</span></span>|
|<span data-ttu-id="2d379-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2d379-114">displayName</span></span>|<span data-ttu-id="2d379-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d379-115">String</span></span>|<span data-ttu-id="2d379-116">A declaração que fornece o nome para exibição ou nome completo do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d379-116">The claim that provides the display name or full name for the user.</span></span> <span data-ttu-id="2d379-117">É uma propriedade necessária.</span><span class="sxs-lookup"><span data-stu-id="2d379-117">It is a required propoerty.</span></span>|
|<span data-ttu-id="2d379-118">givenName</span><span class="sxs-lookup"><span data-stu-id="2d379-118">givenName</span></span>|<span data-ttu-id="2d379-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d379-119">String</span></span>|<span data-ttu-id="2d379-120">A declaração que fornece o primeiro nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d379-120">The claim that provides the first name of the user.</span></span>|
|<span data-ttu-id="2d379-121">surname</span><span class="sxs-lookup"><span data-stu-id="2d379-121">surname</span></span>|<span data-ttu-id="2d379-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d379-122">String</span></span>|<span data-ttu-id="2d379-123">A declaração que fornece o sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d379-123">The claim that provides the last name of the user.</span></span>|
|<span data-ttu-id="2d379-124">email</span><span class="sxs-lookup"><span data-stu-id="2d379-124">email</span></span>|<span data-ttu-id="2d379-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d379-125">String</span></span>|<span data-ttu-id="2d379-126">A declaração que fornece o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="2d379-126">The claim that provides the email address of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d379-127">Relações</span><span class="sxs-lookup"><span data-stu-id="2d379-127">Relationships</span></span>
<span data-ttu-id="2d379-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d379-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d379-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d379-129">JSON representation</span></span>
<span data-ttu-id="2d379-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d379-130">The following is a JSON representation of the resource.</span></span>
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
