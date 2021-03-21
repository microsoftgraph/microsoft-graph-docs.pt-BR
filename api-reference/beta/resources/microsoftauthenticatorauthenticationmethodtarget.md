---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: db612bd2ac7aec387574fe1e45c967e2525c2b12
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960380"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="dc556-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="dc556-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="dc556-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc556-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc556-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc556-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="dc556-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc556-106">Properties</span></span>
|<span data-ttu-id="dc556-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc556-107">Property</span></span>|<span data-ttu-id="dc556-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc556-108">Type</span></span>|<span data-ttu-id="dc556-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc556-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc556-110">id</span><span class="sxs-lookup"><span data-stu-id="dc556-110">id</span></span>|<span data-ttu-id="dc556-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc556-111">String</span></span>|<span data-ttu-id="dc556-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dc556-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="dc556-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="dc556-113">authenticationMode</span></span>|<span data-ttu-id="dc556-114">microsoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="dc556-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="dc556-115">Determina quais tipos de notificações podem ser usadas para entrar.</span><span class="sxs-lookup"><span data-stu-id="dc556-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="dc556-116">Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .</span><span class="sxs-lookup"><span data-stu-id="dc556-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="dc556-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="dc556-117">featureSettings</span></span>|<span data-ttu-id="dc556-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="dc556-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="dc556-119">Determina quais configurações adicionais devem ser aplicadas ao Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="dc556-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="dc556-120">Os valores possíveis são: `null` , `requireNumberMatching` (Requer correspondência de número para notificações MFA.</span><span class="sxs-lookup"><span data-stu-id="dc556-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="dc556-121">O valor é ignorado para notificações de login por telefone).</span><span class="sxs-lookup"><span data-stu-id="dc556-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="dc556-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="dc556-122">isRegistrationRequired</span></span>|<span data-ttu-id="dc556-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc556-123">Boolean</span></span>|<span data-ttu-id="dc556-124">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="dc556-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="dc556-125">*Não há suporte para*.</span><span class="sxs-lookup"><span data-stu-id="dc556-125">*Not supported*.</span></span> |
|<span data-ttu-id="dc556-126">shownContext (Private Preview)</span><span class="sxs-lookup"><span data-stu-id="dc556-126">shownContext (Private Preview)</span></span>|<span data-ttu-id="dc556-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="dc556-127">authenticatorAppContextType</span></span>|<span data-ttu-id="dc556-128">Determina quais tipos de contexto sobre a assinatura devem ser mostrados ao usuário no corpo da notificação.</span><span class="sxs-lookup"><span data-stu-id="dc556-128">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="dc556-129">Os valores possíveis são: `location` e `app`.</span><span class="sxs-lookup"><span data-stu-id="dc556-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="dc556-130">targetType</span><span class="sxs-lookup"><span data-stu-id="dc556-130">targetType</span></span>|<span data-ttu-id="dc556-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="dc556-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="dc556-132">Os valores possíveis são: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="dc556-132">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc556-133">Relações</span><span class="sxs-lookup"><span data-stu-id="dc556-133">Relationships</span></span>
<span data-ttu-id="dc556-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc556-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc556-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc556-135">JSON representation</span></span>
<span data-ttu-id="dc556-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc556-136">The following is a JSON representation of the resource.</span></span>
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
  "shownContext": "String",
  "featureSettings": "String"
}

```
