---
title: tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget
description: Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a26a8fe76da954d3dc44a238665954539df0fa72
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418204"
---
# <a name="passwordlessmicrosoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="b1fbe-103">tipo de recurso passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="b1fbe-103">passwordlessMicrosoftAuthenticatorAuthenticationMethodTarget resource type</span></span>

<span data-ttu-id="b1fbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1fbe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1fbe-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação de entrada de telefone sem senha do Microsoft Authenticator] (.. /resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-105">A collection of users or groups enabled to use Microsoft Authenticator Passwordless Phone Sign-in authentication methods policy](../resources/passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

> [!NOTE]
> <span data-ttu-id="b1fbe-106">Alterações substanciais de esquema são planejadas para APIs que gerenciam o aplicativo Microsoft Authenticator enquanto as APIs estão no Mirosoft Graph beta.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="b1fbe-107">Como os padrões de chamada serão alterados, recomendamos que você não faça uma dependência de produção nessas APIs.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="b1fbe-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1fbe-108">Properties</span></span>
|<span data-ttu-id="b1fbe-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1fbe-109">Property</span></span>|<span data-ttu-id="b1fbe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1fbe-110">Type</span></span>|<span data-ttu-id="b1fbe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1fbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1fbe-112">id</span><span class="sxs-lookup"><span data-stu-id="b1fbe-112">id</span></span>|<span data-ttu-id="b1fbe-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1fbe-113">String</span></span>|<span data-ttu-id="b1fbe-114">ID de objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-114">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="b1fbe-115">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="b1fbe-115">isRegistrationRequired</span></span>|<span data-ttu-id="b1fbe-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1fbe-116">Boolean</span></span>|<span data-ttu-id="b1fbe-117">Determina se o usuário é imposto para registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-117">Determines whether the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="b1fbe-118">shownContext</span><span class="sxs-lookup"><span data-stu-id="b1fbe-118">shownContext</span></span>|<span data-ttu-id="b1fbe-119">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="b1fbe-119">authenticatorAppContextType</span></span>|<span data-ttu-id="b1fbe-120">Os valores possíveis são: `location` e `app`.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-120">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="b1fbe-121">targetType</span><span class="sxs-lookup"><span data-stu-id="b1fbe-121">targetType</span></span>|<span data-ttu-id="b1fbe-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="b1fbe-122">authenticationMethodTargetType</span></span>|<span data-ttu-id="b1fbe-123">Os valores possíveis são: `user` e `group`.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-123">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="b1fbe-124">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="b1fbe-124">useForSignIn</span></span>|<span data-ttu-id="b1fbe-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1fbe-125">Boolean</span></span>|<span data-ttu-id="b1fbe-126">Determina se o método de autenticação pode ser usado para entrar no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-126">Determines whether the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1fbe-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b1fbe-127">Relationships</span></span>
<span data-ttu-id="b1fbe-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1fbe-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1fbe-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1fbe-129">JSON representation</span></span>
<span data-ttu-id="b1fbe-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1fbe-130">The following is a JSON representation of the resource.</span></span>
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
