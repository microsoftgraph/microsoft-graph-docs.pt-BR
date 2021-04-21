---
title: Obter identityProvider
description: Recupere as propriedades e as relações de um objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 31ae4f9ffad6f85466af0adede65c683499e06bd
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921446"
---
# <a name="get-identityprovider"></a><span data-ttu-id="3f932-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="3f932-103">Get identityProvider</span></span>

<span data-ttu-id="3f932-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f932-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f932-105">Recupere as propriedades e as relações de [um socialIdentityProvider](../resources/socialidentityprovider.md) ou [um builtinIdentityProvider](../resources/builtinidentityprovider.md) no Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3f932-105">Retrieve the properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in Azure AD.</span></span>

<span data-ttu-id="3f932-106">Para o Azure AD B2C, ele pode recuperar propriedades e relações de [um socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou [um appleIdentityProvider](../resources/appleidentityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="3f932-106">For Azure AD B2C, it can retrieve properties and relationships of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3f932-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3f932-107">Permissions</span></span>

<span data-ttu-id="3f932-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f932-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3f932-110">Permission type</span></span>      | <span data-ttu-id="3f932-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3f932-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f932-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3f932-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f932-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f932-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3f932-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3f932-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3f932-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3f932-115">Not supported.</span></span>|
|<span data-ttu-id="3f932-116">Application</span><span class="sxs-lookup"><span data-stu-id="3f932-116">Application</span></span>|<span data-ttu-id="3f932-117">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f932-117">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="3f932-118">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="3f932-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3f932-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="3f932-119">Global Administrator</span></span>
* <span data-ttu-id="3f932-120">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="3f932-120">External Identity Provider Administrator</span></span>
* <span data-ttu-id="3f932-121">Administrador de fluxo de usuário de ID externa</span><span class="sxs-lookup"><span data-stu-id="3f932-121">External ID user flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3f932-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3f932-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3f932-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-123">Request headers</span></span>

|<span data-ttu-id="3f932-124">Nome</span><span class="sxs-lookup"><span data-stu-id="3f932-124">Name</span></span>|<span data-ttu-id="3f932-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f932-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3f932-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="3f932-126">Authorization</span></span>|<span data-ttu-id="3f932-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3f932-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f932-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-129">Request body</span></span>

<span data-ttu-id="3f932-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3f932-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f932-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f932-131">Response</span></span>

<span data-ttu-id="3f932-132">Se tiver êxito, este método retornará um código de resposta e uma representação JSON de `200 OK` [um socialIdentityProvider](../resources/socialidentityprovider.md) ou um [builtinIdentityProvider](../resources/builtinidentityprovider.md) no corpo da resposta para um locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3f932-132">If successful, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md) or a [builtinIdentityProvider](../resources/builtinidentityprovider.md) in the response body for an Azure AD tenant.</span></span>

<span data-ttu-id="3f932-133">Para um locatário do Azure AD B2C, este método retorna um código de resposta e uma representação JSON de `200 OK` [um socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) ou um [objeto appleIdentityProvider](../resources/appleidentityprovider.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3f932-133">For an Azure AD B2C tenant, this method returns a `200 OK` response code and a JSON representation of a [socialIdentityProvider](../resources/socialidentityprovider.md), [openIdConnectIdentityProvider](../resources/openidconnectidentityprovider.md) or an [appleIdentityProvider](../resources/appleidentityprovider.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3f932-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3f932-134">Examples</span></span>

### <a name="example-1-retrieve-a-specific-social-identity-provider-azure-ad-or-azure-ad-b2c"></a><span data-ttu-id="3f932-135">Exemplo 1: Recuperar um provedor de identidade **social** específico (Azure AD ou Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="3f932-135">Example 1: Retrieve a specific **social identity provider** (Azure AD or Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="3f932-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-136">Request</span></span>

<span data-ttu-id="3f932-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f932-137">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f932-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f932-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_socialidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Amazon-OAUTH
```
# <a name="c"></a>[<span data-ttu-id="3f932-139">C#</span><span class="sxs-lookup"><span data-stu-id="3f932-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-socialidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f932-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f932-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-socialidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f932-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f932-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-socialidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f932-142">Java</span><span class="sxs-lookup"><span data-stu-id="3f932-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-socialidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="3f932-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f932-143">Response</span></span>

<span data-ttu-id="3f932-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f932-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.socialIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "displayName": "Amazon",
    "identityProviderType": "Amazon",
    "clientId": "09876545678908765978678",
    "clientSecret": "******"
}
```

### <a name="example-2-retrieve-a-specific-built-in-identity-provider-only-for-azure-ad"></a><span data-ttu-id="3f932-145">Exemplo 2: Recuperar um provedor **de identidade integrado específico** (somente para o Azure AD)</span><span class="sxs-lookup"><span data-stu-id="3f932-145">Example 2: Retrieve a specific **built-in identity provider** (only for Azure AD)</span></span>

#### <a name="request"></a><span data-ttu-id="3f932-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-146">Request</span></span>

<span data-ttu-id="3f932-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f932-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f932-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f932-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_builtinidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/MSASignup-OAUTH
```
# <a name="c"></a>[<span data-ttu-id="3f932-149">C#</span><span class="sxs-lookup"><span data-stu-id="3f932-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-builtinidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f932-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f932-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-builtinidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f932-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f932-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-builtinidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f932-152">Java</span><span class="sxs-lookup"><span data-stu-id="3f932-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-builtinidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="3f932-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f932-153">Response</span></span>

<span data-ttu-id="3f932-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f932-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.builtInIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "MSASignup-OAUTH",
    "identityProviderType": "MicrosoftAccount",
    "displayName": "MicrosoftAccount"
}
```

### <a name="example-3-retrieve-a-specific-openid-connect-identity-provider-only-for-azure-ad-b2c"></a><span data-ttu-id="3f932-155">Exemplo 3: Recuperar um provedor de identidade **do OpenID Connect** específico (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="3f932-155">Example 3: Retrieve a specific **OpenID Connect identity provider** (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="3f932-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-156">Request</span></span>

<span data-ttu-id="3f932-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f932-157">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f932-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f932-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_openidconnectidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000
```
# <a name="c"></a>[<span data-ttu-id="3f932-159">C#</span><span class="sxs-lookup"><span data-stu-id="3f932-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-openidconnectidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f932-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f932-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-openidconnectidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f932-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f932-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-openidconnectidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f932-162">Java</span><span class="sxs-lookup"><span data-stu-id="3f932-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-openidconnectidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="3f932-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f932-163">Response</span></span>

<span data-ttu-id="3f932-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f932-164">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectIdentityProvider",
  "id": "OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000",
  "displayName": "Login with the Contoso identity provider",
  "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
  "clientSecret": "12345",
  "claimsMapping": {
      "userId": "myUserId",
      "givenName": "myGivenName",
      "surname": "mySurname",
      "email": "myEmail",
      "displayName": "myDisplayName"
  },
  "domainHint": "mycustomoidc",
  "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
  "responseMode": "form_post",
  "responseType": "code",
  "scope": "openid"
}
```

### <a name="example-4-retrieves-apple-identity-provideronly-for-azure-ad-b2c"></a><span data-ttu-id="3f932-165">Exemplo 4: recupera o provedor de identidade da Apple(somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="3f932-165">Example 4: Retrieves Apple identity provider(only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="3f932-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3f932-166">Request</span></span>

<span data-ttu-id="3f932-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3f932-167">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3f932-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f932-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applemanagedidentityprovider_from_identityproviderbase"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/identityProviders/Apple-Managed-OIDC
```
# <a name="c"></a>[<span data-ttu-id="3f932-169">C#</span><span class="sxs-lookup"><span data-stu-id="3f932-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applemanagedidentityprovider-from-identityproviderbase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f932-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f932-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applemanagedidentityprovider-from-identityproviderbase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f932-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f932-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applemanagedidentityprovider-from-identityproviderbase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f932-172">Java</span><span class="sxs-lookup"><span data-stu-id="3f932-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applemanagedidentityprovider-from-identityproviderbase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="3f932-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="3f932-173">Response</span></span>

<span data-ttu-id="3f932-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3f932-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleManagedIdentityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Apple-Managed-OIDC",
    "displayName": "Sign in with Apple",
    "developerId": "UBF8T346G9",
    "serviceId": "com.microsoft.rts.b2c.test.client",
    "keyId": "99P6D879C4",
    "certificateData": "******"
}
```
