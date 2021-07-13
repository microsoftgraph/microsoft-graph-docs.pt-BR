---
title: Listar um userflowidentityproviders
description: Listar todos os provedores de identidade em um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 618d9c0c1c7a27e015e45192f72b8c1455e0522c
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401041"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="02313-103">Listar um userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="02313-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="02313-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02313-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02313-105">Obter os provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="02313-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02313-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02313-106">Permissions</span></span>

<span data-ttu-id="02313-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02313-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02313-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02313-109">Permission type</span></span>      | <span data-ttu-id="02313-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02313-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02313-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02313-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02313-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02313-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="02313-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02313-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="02313-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02313-114">Not supported.</span></span>|
|<span data-ttu-id="02313-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02313-115">Application</span></span>| <span data-ttu-id="02313-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02313-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="02313-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="02313-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="02313-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="02313-118">Global administrator</span></span>
* <span data-ttu-id="02313-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="02313-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="02313-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02313-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="02313-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02313-121">Request headers</span></span>

|<span data-ttu-id="02313-122">Nome</span><span class="sxs-lookup"><span data-stu-id="02313-122">Name</span></span>|<span data-ttu-id="02313-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="02313-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="02313-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="02313-124">Authorization</span></span>|<span data-ttu-id="02313-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02313-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02313-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02313-127">Request body</span></span>

<span data-ttu-id="02313-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02313-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02313-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="02313-129">Response</span></span>

<span data-ttu-id="02313-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityproviderbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02313-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02313-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02313-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="02313-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02313-132">Request</span></span>

<span data-ttu-id="02313-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02313-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_userflowidentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders
```

### <a name="response"></a><span data-ttu-id="02313-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="02313-134">Response</span></span>

<span data-ttu-id="02313-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02313-135">The following is an example of the response.</span></span>
><span data-ttu-id="02313-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02313-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b1576-adca-4bef-b321-076fde19950b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/contoso.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "samuel",
                "givenName": "samuel",
                "surname": "emmense",
                "email": "sam.e@contoso.com"
            }
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "identityProviderType": "AppleManaged",
            "clientId": "com.contoso.client",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "MSA-OIDC",
            "displayName": "Microsoft Account",
            "identityProviderType": "Microsoft",
            "clientId": "1e02ac8a-0c37-4046-abe4-35098a840090",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "Facebook-OAUTH",
            "displayName": "Facebook",
            "identityProviderType": "Facebook",
            "clientId": "576628889930009",
            "clientSecret": "******"
        }
    ]
}
```
