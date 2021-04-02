---
title: Obter identityProvider
description: Recupere as propriedades e as relações de um objeto identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: fc51780f2f5ab9a783b431d49e19136c1f5e3fef
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508579"
---
# <a name="get-identityprovider-deprecated"></a><span data-ttu-id="bcbc4-103">Obter identityProvider (preterido)</span><span class="sxs-lookup"><span data-stu-id="bcbc4-103">Get identityProvider (deprecated)</span></span>

<span data-ttu-id="bcbc4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcbc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="bcbc4-105">Recupere as propriedades e as relações de [um identityProvider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="bcbc4-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bcbc4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bcbc4-106">Permissions</span></span>

<span data-ttu-id="bcbc4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcbc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcbc4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcbc4-109">Permission type</span></span>      | <span data-ttu-id="bcbc4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bcbc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bcbc4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcbc4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bcbc4-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbc4-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="bcbc4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcbc4-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="bcbc4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-114">Not supported.</span></span>|
|<span data-ttu-id="bcbc4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcbc4-115">Application</span></span>|<span data-ttu-id="bcbc4-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbc4-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="bcbc4-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="bcbc4-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="bcbc4-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bcbc4-118">Global administrator</span></span>
* <span data-ttu-id="bcbc4-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="bcbc4-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="bcbc4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbc4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bcbc4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbc4-121">Request headers</span></span>

|<span data-ttu-id="bcbc4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="bcbc4-122">Name</span></span>|<span data-ttu-id="bcbc4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcbc4-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="bcbc4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcbc4-124">Authorization</span></span>|<span data-ttu-id="bcbc4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcbc4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbc4-127">Request body</span></span>

<span data-ttu-id="bcbc4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcbc4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbc4-129">Response</span></span>

<span data-ttu-id="bcbc4-130">Se tiver êxito, este método retornará um código de resposta e uma representação JSON do `200 OK` [identityProvider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure AD B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bcbc4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bcbc4-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="bcbc4-132">Exemplo 1: Recuperar uma identidade específicaProvider</span><span class="sxs-lookup"><span data-stu-id="bcbc4-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="bcbc4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbc4-133">Request</span></span>

<span data-ttu-id="bcbc4-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcbc4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbc4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="bcbc4-136">C#</span><span class="sxs-lookup"><span data-stu-id="bcbc4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcbc4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcbc4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcbc4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcbc4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcbc4-139">Java</span><span class="sxs-lookup"><span data-stu-id="bcbc4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bcbc4-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbc4-140">Response</span></span>

<span data-ttu-id="bcbc4-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="bcbc4-142">Exemplo 2: Recuperar um openIDConnectProvider específico (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="bcbc4-142">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="bcbc4-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbc4-143">Request</span></span>

<span data-ttu-id="bcbc4-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bcbc4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbc4-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="bcbc4-146">C#</span><span class="sxs-lookup"><span data-stu-id="bcbc4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bcbc4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bcbc4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bcbc4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bcbc4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bcbc4-149">Java</span><span class="sxs-lookup"><span data-stu-id="bcbc4-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bcbc4-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbc4-150">Response</span></span>

<span data-ttu-id="bcbc4-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bcbc4-151">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openIdConnectProvider"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "microsoft.graph.openIdConnectProvider",
  "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
  "name": "Login with the Contoso identity provider",
  "type": "OpenIDConnect",
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
