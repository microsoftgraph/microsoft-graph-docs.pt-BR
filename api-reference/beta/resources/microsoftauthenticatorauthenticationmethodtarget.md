---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar Microsoft Authenticator de autenticação.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db534dfb13e288b82b49005b2b1a923b8bfd5112
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896638"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="28e22-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="28e22-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="28e22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28e22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28e22-105">Uma coleção de usuários ou grupos habilitados para [usar](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) Microsoft Authenticator de autenticação no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28e22-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="28e22-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e22-106">Properties</span></span>
|<span data-ttu-id="28e22-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e22-107">Property</span></span>|<span data-ttu-id="28e22-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e22-108">Type</span></span>|<span data-ttu-id="28e22-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28e22-110">id</span><span class="sxs-lookup"><span data-stu-id="28e22-110">id</span></span>|<span data-ttu-id="28e22-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e22-111">String</span></span>|<span data-ttu-id="28e22-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="28e22-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="28e22-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="28e22-113">authenticationMode</span></span>|<span data-ttu-id="28e22-114">microsoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="28e22-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="28e22-115">Determina quais tipos de notificações podem ser usadas para entrar.</span><span class="sxs-lookup"><span data-stu-id="28e22-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="28e22-116">Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .</span><span class="sxs-lookup"><span data-stu-id="28e22-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="28e22-117">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="28e22-117">isRegistrationRequired</span></span>|<span data-ttu-id="28e22-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="28e22-118">Boolean</span></span>|<span data-ttu-id="28e22-119">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="28e22-119">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="28e22-120">*Não há suporte para*.</span><span class="sxs-lookup"><span data-stu-id="28e22-120">*Not supported*.</span></span> |
|<span data-ttu-id="28e22-121">numberMatchingRequiredState</span><span class="sxs-lookup"><span data-stu-id="28e22-121">numberMatchingRequiredState</span></span>|<span data-ttu-id="28e22-122">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="28e22-122">advancedConfigState</span></span>|<span data-ttu-id="28e22-123">Requer correspondência de números para notificações MFA.</span><span class="sxs-lookup"><span data-stu-id="28e22-123">Requires number matching for MFA notifications.</span></span> <span data-ttu-id="28e22-124">O valor é ignorado para notificações de login por telefone.</span><span class="sxs-lookup"><span data-stu-id="28e22-124">Value is ignored for phone sign-in notifications.</span></span> <span data-ttu-id="28e22-125">Os valores possíveis são: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="28e22-125">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="28e22-126">displayLocationInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="28e22-126">displayLocationInformationRequiredState</span></span>|<span data-ttu-id="28e22-127">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="28e22-127">advancedConfigState</span></span>|<span data-ttu-id="28e22-128">Determina se o local da assinatura deve ser mostrado ao usuário no corpo da notificação.</span><span class="sxs-lookup"><span data-stu-id="28e22-128">Determines whether the location of the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="28e22-129">Os valores possíveis são: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="28e22-129">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="28e22-130">displayAppInformationRequiredState</span><span class="sxs-lookup"><span data-stu-id="28e22-130">displayAppInformationRequiredState</span></span>|<span data-ttu-id="28e22-131">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="28e22-131">advancedConfigState</span></span>|<span data-ttu-id="28e22-132">Determina se o aplicativo no qual o usuário está entrando deve ser mostrado ao usuário no corpo da notificação.</span><span class="sxs-lookup"><span data-stu-id="28e22-132">Determines whether the app the user is signing into should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="28e22-133">Os valores possíveis são: `enabled`, `disabled`, `default`.</span><span class="sxs-lookup"><span data-stu-id="28e22-133">Possible values are: `enabled`, `disabled`, `default`.</span></span>|
|<span data-ttu-id="28e22-134">targetType</span><span class="sxs-lookup"><span data-stu-id="28e22-134">targetType</span></span>|<span data-ttu-id="28e22-135">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="28e22-135">authenticationMethodTargetType</span></span>| <span data-ttu-id="28e22-136">Os valores possíveis são: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="28e22-136">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28e22-137">Relações</span><span class="sxs-lookup"><span data-stu-id="28e22-137">Relationships</span></span>
<span data-ttu-id="28e22-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28e22-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28e22-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e22-139">JSON representation</span></span>
<span data-ttu-id="28e22-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e22-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "authenticationMode": "String",
  "numberMatchingRequiredState": "String",
  "displayLocationInformationRequiredState": "String",
  "displayAppInformationRequiredState": "String"
}

```
