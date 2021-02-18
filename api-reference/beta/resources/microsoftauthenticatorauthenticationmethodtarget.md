---
title: Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget
description: Um conjunto de usuários ou grupos habilitados para usar a política de métodos de autenticação do Microsoft Authenticator.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a8eb9959faaf5f4a6bcaecceb165384be737623d
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292270"
---
# <a name="microsoftauthenticatorauthenticationmethodtarget-resource-type"></a><span data-ttu-id="455bd-103">Tipo de recurso microsoftAuthenticatorAuthenticationMethodTarget</span><span class="sxs-lookup"><span data-stu-id="455bd-103">microsoftAuthenticatorAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="455bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="455bd-105">Uma coleção de usuários ou grupos habilitados para usar a política de métodos de autenticação [do Microsoft Authenticator](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="455bd-105">A collection of users or groups enabled to use [Microsoft Authenticator authentication methods policy](../resources/microsoftAuthenticatorAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="455bd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="455bd-106">Properties</span></span>
|<span data-ttu-id="455bd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="455bd-107">Property</span></span>|<span data-ttu-id="455bd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="455bd-108">Type</span></span>|<span data-ttu-id="455bd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="455bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455bd-110">id</span><span class="sxs-lookup"><span data-stu-id="455bd-110">id</span></span>|<span data-ttu-id="455bd-111">String</span><span class="sxs-lookup"><span data-stu-id="455bd-111">String</span></span>|<span data-ttu-id="455bd-112">ID do objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="455bd-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="455bd-113">isNumberMatchingRequired (Visualização Privada)</span><span class="sxs-lookup"><span data-stu-id="455bd-113">isNumberMatchingRequired (Private Preview)</span></span>|<span data-ttu-id="455bd-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="455bd-114">Boolean</span></span>|<span data-ttu-id="455bd-115">Exigir que o usuário corresponder ao número exibido na página de login para aprovar a notificação MFA.</span><span class="sxs-lookup"><span data-stu-id="455bd-115">Require the user to match the number displayed on the sign-in page to approve the MFA notification.</span></span>|
|<span data-ttu-id="455bd-116">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="455bd-116">isRegistrationRequired</span></span>|<span data-ttu-id="455bd-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="455bd-117">Boolean</span></span>|<span data-ttu-id="455bd-118">Determina se o usuário é imposto a registrar o método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="455bd-118">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="455bd-119">*Sem suporte.*</span><span class="sxs-lookup"><span data-stu-id="455bd-119">*Not supported*.</span></span> |
|<span data-ttu-id="455bd-120">shownContext (Visualização Privada)</span><span class="sxs-lookup"><span data-stu-id="455bd-120">shownContext (Private Preview)</span></span>|<span data-ttu-id="455bd-121">authenticatorAppContextType</span><span class="sxs-lookup"><span data-stu-id="455bd-121">authenticatorAppContextType</span></span>|<span data-ttu-id="455bd-122">Determina quais tipos de contexto sobre a entrar devem ser mostrados para o usuário no corpo da notificação.</span><span class="sxs-lookup"><span data-stu-id="455bd-122">Determines what types of context about the sign-in should be shown to the user in the body of the notification.</span></span> <span data-ttu-id="455bd-123">Os valores possíveis são: `location` e `app`.</span><span class="sxs-lookup"><span data-stu-id="455bd-123">Possible values are: `location`, `app`.</span></span>|
|<span data-ttu-id="455bd-124">targetType</span><span class="sxs-lookup"><span data-stu-id="455bd-124">targetType</span></span>|<span data-ttu-id="455bd-125">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="455bd-125">authenticationMethodTargetType</span></span>| <span data-ttu-id="455bd-126">Os valores possíveis são: `null`, `user`, `group`.</span><span class="sxs-lookup"><span data-stu-id="455bd-126">Possible values are: `null`, `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="455bd-127">Relações</span><span class="sxs-lookup"><span data-stu-id="455bd-127">Relationships</span></span>
<span data-ttu-id="455bd-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="455bd-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="455bd-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="455bd-129">JSON representation</span></span>
<span data-ttu-id="455bd-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="455bd-130">The following is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean",
  "shownContext": "String",
  "isNumberMatchingRequired": "Boolean"
}
```

