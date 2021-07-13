---
title: Listar um userflowidentityproviders
description: Listar todos os identityProviders em um b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 63bf686abbe51a9abd132e71d1e4472fc45c0849
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401039"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="beb72-103">Listar um userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="beb72-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="beb72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="beb72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beb72-105">Obter os provedores de identidade em um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="beb72-105">Get the identity providers in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="beb72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="beb72-106">Permissions</span></span>

<span data-ttu-id="beb72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="beb72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="beb72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="beb72-109">Permission type</span></span>      | <span data-ttu-id="beb72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="beb72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="beb72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="beb72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="beb72-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb72-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="beb72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="beb72-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="beb72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="beb72-114">Not supported.</span></span>|
|<span data-ttu-id="beb72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb72-115">Application</span></span>| <span data-ttu-id="beb72-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="beb72-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="beb72-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="beb72-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="beb72-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="beb72-118">Global administrator</span></span>
* <span data-ttu-id="beb72-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="beb72-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="beb72-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="beb72-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="beb72-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="beb72-121">Request headers</span></span>

|<span data-ttu-id="beb72-122">Nome</span><span class="sxs-lookup"><span data-stu-id="beb72-122">Name</span></span>|<span data-ttu-id="beb72-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="beb72-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="beb72-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="beb72-124">Authorization</span></span>|<span data-ttu-id="beb72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beb72-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="beb72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="beb72-127">Request body</span></span>

<span data-ttu-id="beb72-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="beb72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beb72-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb72-129">Response</span></span>

<span data-ttu-id="beb72-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityproviderbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="beb72-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="beb72-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="beb72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="beb72-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="beb72-132">Request</span></span>

<span data-ttu-id="beb72-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="beb72-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlow_list_userflowIdentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Test/userflowIdentityProviders
```

### <a name="response"></a><span data-ttu-id="beb72-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="beb72-134">Response</span></span>

<span data-ttu-id="beb72-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="beb72-135">The following is an example of the response.</span></span>

<span data-ttu-id="beb72-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="beb72-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.identityProviderBase)",
    "value": [
  {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "AADSignup-OAUTH",
            "displayName": "Azure Active Directory Sign up",
            "identityProviderType": "AADSignup"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "MSASignup-OAUTH",
            "displayName": "Microsoft Account (Preview)",
            "identityProviderType": "MicrosoftAccount"
        },
        {
            "@odata.type": "#microsoft.graph.builtInIdentityProvider",
            "id": "EmailOtpSignup-OAUTH",
            "displayName": "Email one-time passcode (Preview)",
            "identityProviderType": "EmailOTP"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "clientIdFromFacebook",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Google-OAuth",
            "type": "Google",
            "name": "Google",
            "clientId": "clientIdFromGoogle",
            "clientSecret": "*****"
        }
    ]
}

```
