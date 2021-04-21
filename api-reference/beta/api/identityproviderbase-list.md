---
title: Lista identityProviders
description: Recupere uma lista de objetos identityProviderbase.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 47e136bc63cd7b95bdcf3778047eb77db58c8de0
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921375"
---
# <a name="list-identityproviders"></a><span data-ttu-id="0bca4-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="0bca4-103">List identityProviders</span></span>
<span data-ttu-id="0bca4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bca4-105">Recuperar uma lista de conjunto de objetos herdados  [de identityProviderBase](../resources/identityproviderbase.md).</span><span class="sxs-lookup"><span data-stu-id="0bca4-105">Retrieve a list of collection of object inherited from  [identityProviderBase](../resources/identityproviderbase.md).</span></span>

<span data-ttu-id="0bca4-106">Para um locatário do Azure AD, ele pode ser [socialIdentityProviders](../resources/socialidentityprovider.md) e/ou [objetos builtinIdentityProviders.](../resources/builtinidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="0bca4-106">For an Azure AD tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md) and/or [builtinIdentityProviders](../resources/builtinidentityprovider.md) objects.</span></span>

<span data-ttu-id="0bca4-107">Para um locatário do Azure AD B2C, pode ser [socialIdentityProviders,](../resources/socialidentityprovider.md) [objetos openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider.](../resources/appleidentityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="0bca4-107">For an Azure AD B2C tenant it can be [socialIdentityProviders](../resources/socialidentityprovider.md), [openIdConnectIdentityProviders](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0bca4-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0bca4-108">Permissions</span></span>

<span data-ttu-id="0bca4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0bca4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bca4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0bca4-111">Permission type</span></span>      | <span data-ttu-id="0bca4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0bca4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bca4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0bca4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bca4-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bca4-114">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="0bca4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0bca4-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0bca4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0bca4-116">Not supported.</span></span>|
|<span data-ttu-id="0bca4-117">Application</span><span class="sxs-lookup"><span data-stu-id="0bca4-117">Application</span></span>|<span data-ttu-id="0bca4-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bca4-118">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="0bca4-119">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="0bca4-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0bca4-120">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="0bca4-120">Global Administrator</span></span>
* <span data-ttu-id="0bca4-121">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="0bca4-121">External Identity Provider Administrator</span></span>
* <span data-ttu-id="0bca4-122">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="0bca4-122">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0bca4-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0bca4-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="0bca4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0bca4-124">Request headers</span></span>

|<span data-ttu-id="0bca4-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0bca4-125">Name</span></span>|<span data-ttu-id="0bca4-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0bca4-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0bca4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0bca4-127">Authorization</span></span>|<span data-ttu-id="0bca4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0bca4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bca4-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0bca4-130">Request body</span></span>

<span data-ttu-id="0bca4-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0bca4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bca4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bca4-132">Response</span></span>

<span data-ttu-id="0bca4-133">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md) e/ou [builtinIdentityProvider](../resources/builtinidentityprovider.md) no corpo da resposta para um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0bca4-133">If successful, this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md) and/or [builtinIdentityProvider](../resources/builtinidentityprovider.md) objects in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="0bca4-134">Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma coleção de objetos `200 OK` [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) e/ou [appleIdentityProvider](../resources/appleidentityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0bca4-134">For an Azure AD B2C tenant this method returns a `200 OK` response code and a collection of [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) and/or [appleIdentityProvider](../resources/appleidentityprovider.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bca4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0bca4-135">Example</span></span>

### <a name="example-1-list-all-identityprovider-configured-in-an-azure-ad-tenant"></a><span data-ttu-id="0bca4-136">Exemplo 1: listar **toda a identidadeProvider** configurada em um locatário do Azure AD</span><span class="sxs-lookup"><span data-stu-id="0bca4-136">Example 1: List all **identityProvider** configured in an Azure AD tenant</span></span>

### <a name="request"></a><span data-ttu-id="0bca4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bca4-137">Request</span></span>
<span data-ttu-id="0bca4-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bca4-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0bca4-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0bca4-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="0bca4-140">C#</span><span class="sxs-lookup"><span data-stu-id="0bca4-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0bca4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0bca4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0bca4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0bca4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0bca4-143">Java</span><span class="sxs-lookup"><span data-stu-id="0bca4-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0bca4-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bca4-144">Response</span></span>
<span data-ttu-id="0bca4-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0bca4-145">The following is an example of the response.</span></span>

<span data-ttu-id="0bca4-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0bca4-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
   "value":[
      {
         "@odata.type": "microsoft.graph.builtInIdentityProvider",
         "id": "MSASignup-OAUTH",
         "identityProviderType": "MicrosoftAccount",
         "displayName": "MicrosoftAccount"
      },
      {
         "@odata.type": "#microsoft.graph.socialIdentityProvider",
         "id": "Facebook-OAUTH",
         "displayName": "Facebook",
         "identityProviderType": "Facebook",
         "clientId": "test",
         "clientSecret": "******"
      }
   ]
}
```

### <a name="example-2-list-all-identityprovider-configured-in-an-azure-ad-b2c-tenant"></a><span data-ttu-id="0bca4-147">Exemplo 2: listar **toda a identidadeProvider** configurada em um locatário do Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="0bca4-147">Example 2: List all **identityProvider** configured in an Azure AD B2C tenant</span></span>

### <a name="request"></a><span data-ttu-id="0bca4-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0bca4-148">Request</span></span>
<span data-ttu-id="0bca4-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0bca4-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders
```

### <a name="response"></a><span data-ttu-id="0bca4-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="0bca4-150">Response</span></span>
<span data-ttu-id="0bca4-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0bca4-151">The following is an example of the response.</span></span>

<span data-ttu-id="0bca4-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0bca4-152">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProviderBase",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/identityProviders",
    "value": [
        {
            "@odata.type": "#microsoft.graph.socialIdentityProvider",
            "id": "LinkedIn-OAUTH",
            "displayName": "linkedin",
            "identityProviderType": "LinkedIn",
            "clientId": "866xc0qtyy00ih",
            "clientSecret": "******"
        },
        {
            "@odata.type": "#microsoft.graph.openIdConnectIdentityProvider",
            "id": "OIDC-V1-rtt_AD_Test-3e393390-ed2d-4794-97f6-5c1a1ccc61f7",
            "displayName": "OIDC AD Test",
            "clientId": "fe1b3476-rdca-4bef-b321-076fde19750b",
            "clientSecret": "******",
            "scope": "openid",
            "metadataUrl": "https://login.microsoftonline.com/sashawho.onmicrosoft.com/.well-known/openid-configuration",
            "domainHint": "",
            "responseType": "code",
            "responseMode": "form_post",
            "claimsMapping": {
                "userId": "oid",
                "displayName": "name",
                "givenName": "given_name",
                "surname": "family_name",
                "email": "unique_email"
            }
        },
        {
            "@odata.type": "#microsoft.graph.appleManagedIdentityProvider",
            "id": "Apple-Managed-OIDC",
            "displayName": "Sign in with Apple",
            "developerId": "UBF8T346G9",
            "serviceId": "com.microsoft.aad.b2c.iuyt.client",
            "keyId": "99P6DD87C4",
            "certificateData": "******"
        }
    ]
}

```
