---
title: Listar um userflowidentityproviders
description: Listar todos os provedores de identidade em um b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 04d45c4fc622b24f3d9a04410ec010e08c45e3ad
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439739"
---
# <a name="list-a-userflowidentityproviders"></a><span data-ttu-id="97b1d-103">Listar um userflowidentityproviders</span><span class="sxs-lookup"><span data-stu-id="97b1d-103">List a userflowidentityproviders</span></span>

<span data-ttu-id="97b1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97b1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97b1d-105">Obter os provedores de identidade em um [objeto b2cIdentityUserFlow.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="97b1d-105">Get the identity providers in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97b1d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="97b1d-106">Permissions</span></span>

<span data-ttu-id="97b1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97b1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97b1d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97b1d-109">Permission type</span></span>      | <span data-ttu-id="97b1d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97b1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97b1d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97b1d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97b1d-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b1d-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="97b1d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97b1d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="97b1d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97b1d-114">Not supported.</span></span>|
|<span data-ttu-id="97b1d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97b1d-115">Application</span></span>| <span data-ttu-id="97b1d-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97b1d-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="97b1d-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="97b1d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="97b1d-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="97b1d-118">Global administrator</span></span>
* <span data-ttu-id="97b1d-119">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="97b1d-119">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="97b1d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97b1d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{userflow-id}/userflowIdentityProviders
```

## <a name="request-headers"></a><span data-ttu-id="97b1d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97b1d-121">Request headers</span></span>

|<span data-ttu-id="97b1d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="97b1d-122">Name</span></span>|<span data-ttu-id="97b1d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="97b1d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="97b1d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="97b1d-124">Authorization</span></span>|<span data-ttu-id="97b1d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97b1d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97b1d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97b1d-127">Request body</span></span>

<span data-ttu-id="97b1d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97b1d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97b1d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b1d-129">Response</span></span>

<span data-ttu-id="97b1d-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` representação JSON dos [identityProviders](../resources/identityproviderbase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97b1d-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProviders](../resources/identityproviderbase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97b1d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97b1d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="97b1d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97b1d-132">Request</span></span>

<span data-ttu-id="97b1d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97b1d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="97b1d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="97b1d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlow_list_userflowidentityProviders"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders
```
# <a name="c"></a>[<span data-ttu-id="97b1d-135">C#</span><span class="sxs-lookup"><span data-stu-id="97b1d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflow-list-userflowidentityproviders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97b1d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97b1d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflow-list-userflowidentityproviders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97b1d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97b1d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflow-list-userflowidentityproviders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97b1d-138">Java</span><span class="sxs-lookup"><span data-stu-id="97b1d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflow-list-userflowidentityproviders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97b1d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="97b1d-139">Response</span></span>

<span data-ttu-id="97b1d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97b1d-140">The following is an example of the response.</span></span>
><span data-ttu-id="97b1d-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97b1d-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
