---
title: Obter identityProvider
description: Recupere as propriedades e os relacionamentos de um objeto identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 69615bbe83d3d93f09120a39277f8c18415ca745
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953429"
---
# <a name="get-identityprovider"></a><span data-ttu-id="006a5-103">Obter identityProvider</span><span class="sxs-lookup"><span data-stu-id="006a5-103">Get identityProvider</span></span>

<span data-ttu-id="006a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="006a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="006a5-105">Recupere as propriedades e os relacionamentos de um [identityprovider](../resources/identityprovider.md).</span><span class="sxs-lookup"><span data-stu-id="006a5-105">Retrieve the properties and relationships of an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="006a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="006a5-106">Permissions</span></span>

<span data-ttu-id="006a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="006a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="006a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="006a5-109">Permission type</span></span>      | <span data-ttu-id="006a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="006a5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="006a5-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="006a5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="006a5-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="006a5-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="006a5-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="006a5-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="006a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="006a5-114">Not supported.</span></span>|
|<span data-ttu-id="006a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="006a5-115">Application</span></span>|<span data-ttu-id="006a5-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="006a5-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="006a5-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="006a5-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="006a5-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="006a5-118">Global administrator</span></span>
* <span data-ttu-id="006a5-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="006a5-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="006a5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="006a5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="006a5-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="006a5-121">Request headers</span></span>

|<span data-ttu-id="006a5-122">Nome</span><span class="sxs-lookup"><span data-stu-id="006a5-122">Name</span></span>|<span data-ttu-id="006a5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="006a5-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="006a5-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="006a5-124">Authorization</span></span>|<span data-ttu-id="006a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="006a5-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="006a5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="006a5-127">Request body</span></span>

<span data-ttu-id="006a5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="006a5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="006a5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="006a5-129">Response</span></span>

<span data-ttu-id="006a5-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [identityprovider](../resources/identityprovider.md) ou [openIdConnectProvider](../resources/openidconnectprovider.md) (somente para o Azure ad B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="006a5-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) or [openIdConnectProvider](../resources/openidconnectprovider.md) (only for Azure AD B2C) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="006a5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="006a5-131">Examples</span></span>

### <a name="example-1-retrieve-a-specific-identityprovider"></a><span data-ttu-id="006a5-132">Exemplo 1: recuperar um identityprovider específico</span><span class="sxs-lookup"><span data-stu-id="006a5-132">Example 1: Retrieve a specific identityProvider</span></span>

#### <a name="request"></a><span data-ttu-id="006a5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="006a5-133">Request</span></span>

<span data-ttu-id="006a5-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="006a5-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="006a5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="006a5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```
# <a name="c"></a>[<span data-ttu-id="006a5-136">C#</span><span class="sxs-lookup"><span data-stu-id="006a5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="006a5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="006a5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="006a5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="006a5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="006a5-139">Java</span><span class="sxs-lookup"><span data-stu-id="006a5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="006a5-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="006a5-140">Response</span></span>

<span data-ttu-id="006a5-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="006a5-141">The following is an example of the response.</span></span>

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
### <a name="example-2-retrieve-a-specific-openidconnectprovider-only-for-azure-ad-b2c"></a><span data-ttu-id="006a5-142">Exemplo 2: recuperar um determinado openIDConnectProvider (somente para o Azure AD B2C)</span><span class="sxs-lookup"><span data-stu-id="006a5-142">Example 2: Retrieve a specific openIDConnectProvider (only for Azure AD B2C)</span></span>

#### <a name="request"></a><span data-ttu-id="006a5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="006a5-143">Request</span></span>

<span data-ttu-id="006a5-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="006a5-144">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/{id}
```

#### <a name="response"></a><span data-ttu-id="006a5-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="006a5-145">Response</span></span>

<span data-ttu-id="006a5-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="006a5-146">The following is an example of the response.</span></span>
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


