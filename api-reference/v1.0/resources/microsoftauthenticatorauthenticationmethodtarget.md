---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 43c8e5a4ba92e838a64ec5f345ae82c744b53dee
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469245"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="5a2df-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="5a2df-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="5a2df-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a2df-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a2df-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a2df-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="5a2df-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a2df-106">Properties</span></span>
|<span data-ttu-id="5a2df-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a2df-107">Property</span></span>|<span data-ttu-id="5a2df-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a2df-108">Type</span></span>|<span data-ttu-id="5a2df-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2df-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2df-110">id</span><span class="sxs-lookup"><span data-stu-id="5a2df-110">id</span></span>|<span data-ttu-id="5a2df-111">String</span><span class="sxs-lookup"><span data-stu-id="5a2df-111">String</span></span>|<span data-ttu-id="5a2df-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5a2df-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="5a2df-113">authenticationMode</span><span class="sxs-lookup"><span data-stu-id="5a2df-113">authenticationMode</span></span>|<span data-ttu-id="5a2df-114">microsoftAuthenticatorAuthenticationMode</span><span class="sxs-lookup"><span data-stu-id="5a2df-114">microsoftAuthenticatorAuthenticationMode</span></span>|<span data-ttu-id="5a2df-115">Determina quais tipos de notificações podem ser usadas para entrar.</span><span class="sxs-lookup"><span data-stu-id="5a2df-115">Determines which types of notifications can be used for sign-in.</span></span> <span data-ttu-id="5a2df-116">Os valores possíveis são: `any` , ( somente sem `deviceBasedPush` senha), `push` .</span><span class="sxs-lookup"><span data-stu-id="5a2df-116">Possible values are: `any`, `deviceBasedPush` (passwordless only), `push`.</span></span>|
|<span data-ttu-id="5a2df-117">featureSettings</span><span class="sxs-lookup"><span data-stu-id="5a2df-117">featureSettings</span></span>|<span data-ttu-id="5a2df-118">authenticatorAppFeatureSettings</span><span class="sxs-lookup"><span data-stu-id="5a2df-118">authenticatorAppFeatureSettings</span></span>|<span data-ttu-id="5a2df-119">Determina quais configurações adicionais devem ser aplicadas ao Microsoft Authenticator.</span><span class="sxs-lookup"><span data-stu-id="5a2df-119">Determines what additional settings should be applied to Microsoft Authenticator.</span></span> <span data-ttu-id="5a2df-120">Os valores possíveis são: `null` , `requireNumberMatching` (Requer correspondência de número para notificações MFA.</span><span class="sxs-lookup"><span data-stu-id="5a2df-120">Possible values are: `null`, `requireNumberMatching` (Requires number matching for MFA notifications.</span></span> <span data-ttu-id="5a2df-121">O valor é ignorado para notificações de login por telefone).</span><span class="sxs-lookup"><span data-stu-id="5a2df-121">Value is ignored for phone sign-in notifications).</span></span>|
|<span data-ttu-id="5a2df-122">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="5a2df-122">isRegistrationRequired</span></span>|<span data-ttu-id="5a2df-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a2df-123">Boolean</span></span>|<span data-ttu-id="5a2df-124">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="5a2df-124">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="5a2df-125">*Não há suporte para*.</span><span class="sxs-lookup"><span data-stu-id="5a2df-125">*Not supported*.</span></span> |
|<span data-ttu-id="5a2df-126">shownContext</span><span class="sxs-lookup"><span data-stu-id="5a2df-126">shownContext</span></span>|<span data-ttu-id="5a2df-127">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="5a2df-127">authenticatorAppContextType</span></span>|<span data-ttu-id="5a2df-128">(Visualização Privada) Determina quais tipos de contexto sobre a assinatura devem ser mostrados ao usuário no corpo da notificação.</span><span class="sxs-lookup"><span data-stu-id="5a2df-128">(Private Preview) Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="5a2df-129">Os valores possíveis são: `location` e `app`.</span><span class="sxs-lookup"><span data-stu-id="5a2df-129">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="5a2df-130">targetType</span><span class="sxs-lookup"><span data-stu-id="5a2df-130">targetType</span></span>|<span data-ttu-id="5a2df-131">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="5a2df-131">authenticationMethodTargetType</span></span>| <span data-ttu-id="5a2df-132">Os valores possíveis são: `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="5a2df-132">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a2df-133">Relações</span><span class="sxs-lookup"><span data-stu-id="5a2df-133">Relationships</span></span>
<span data-ttu-id="5a2df-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a2df-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a2df-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a2df-135">JSON representation</span></span>
<span data-ttu-id="5a2df-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a2df-136">The following is a JSON representation of the resource.</span></span>
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
