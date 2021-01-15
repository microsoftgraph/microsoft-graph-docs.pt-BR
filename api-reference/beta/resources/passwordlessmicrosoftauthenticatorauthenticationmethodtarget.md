---
title: Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ef62b251d6c943bd6290a07fa2b018bddca81ab5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872265"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type-deprecated"></a><span data-ttu-id="ee098-103">Tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget (preterido)</span><span class="sxs-lookup"><span data-stu-id="ee098-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type (deprecated)</span></span>

<span data-ttu-id="ee098-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee098-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee098-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de Login de Telefone sem Senha do Microsoft Authenticator](.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee098-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!CAUTION]
> <span data-ttu-id="ee098-106">A API do método de autenticação de autenticação de telefone sem senha do Microsoft Authenticator foi preterida e parou de retornar resultados em 31 de dezembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="ee098-106">The Microsoft Authenticator Passwordless Phone Sign-in authentication method policy API is deprecated and stopped returning results on December 31, 2020.</span></span> <span data-ttu-id="ee098-107">Use a nova política [de método de autenticação do Microsoft Authenticator.](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ee098-107">Please use the new [Microsoft Authenticator authentication method policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ee098-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee098-108">Properties</span></span>
|<span data-ttu-id="ee098-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee098-109">Property</span></span>|<span data-ttu-id="ee098-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee098-110">Type</span></span>|<span data-ttu-id="ee098-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee098-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee098-112">id</span><span class="sxs-lookup"><span data-stu-id="ee098-112">id</span></span>|<span data-ttu-id="ee098-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee098-113">String</span></span>|<span data-ttu-id="ee098-114">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee098-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="ee098-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="ee098-115">isRegistrationRequired</span></span>|<span data-ttu-id="ee098-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee098-116">Boolean</span></span>|<span data-ttu-id="ee098-117">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="ee098-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="ee098-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="ee098-118">shownContext</span></span>|<span data-ttu-id="ee098-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="ee098-119">authenticatorAppContextType</span></span>|<span data-ttu-id="ee098-120">Os valores possíveis são: `location` e `app`.</span><span class="sxs-lookup"><span data-stu-id="ee098-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="ee098-121">targetType</span><span class="sxs-lookup"><span data-stu-id="ee098-121">targetType</span></span>|<span data-ttu-id="ee098-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="ee098-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="ee098-123">Os valores possíveis são: `user` e `group`.</span><span class="sxs-lookup"><span data-stu-id="ee098-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="ee098-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="ee098-124">useForSignIn</span></span>|<span data-ttu-id="ee098-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="ee098-125">Boolean</span></span>|<span data-ttu-id="ee098-126">Determina se o método de autenticação pode ser usado para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee098-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee098-127">Relações</span><span class="sxs-lookup"><span data-stu-id="ee098-127">Relationships</span></span>
<span data-ttu-id="ee098-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee098-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee098-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee098-129">JSON representation</span></span>
<span data-ttu-id="ee098-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee098-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String"
}
```
