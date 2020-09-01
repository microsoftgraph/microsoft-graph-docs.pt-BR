---
title: Lista identityProviders
description: Recupere uma lista de objetos identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86eb1de0d222bc9b535df843e3a30dbd248505a1
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319552"
---
# <a name="list-identityproviders"></a><span data-ttu-id="e79ad-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="e79ad-103">List identityProviders</span></span>

<span data-ttu-id="e79ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e79ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e79ad-105">Recupere uma lista de objetos [identityProviders](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="e79ad-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e79ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e79ad-106">Permissions</span></span>

<span data-ttu-id="e79ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e79ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e79ad-109">Permission type</span></span>      | <span data-ttu-id="e79ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e79ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e79ad-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e79ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e79ad-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79ad-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e79ad-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e79ad-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e79ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e79ad-114">Not supported.</span></span>|
|<span data-ttu-id="e79ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e79ad-115">Application</span></span>|<span data-ttu-id="e79ad-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79ad-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="e79ad-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e79ad-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="e79ad-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e79ad-118">Global administrator</span></span>
* <span data-ttu-id="e79ad-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="e79ad-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e79ad-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e79ad-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e79ad-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e79ad-121">Request headers</span></span>

|<span data-ttu-id="e79ad-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e79ad-122">Name</span></span>|<span data-ttu-id="e79ad-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e79ad-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e79ad-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e79ad-124">Authorization</span></span>|<span data-ttu-id="e79ad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e79ad-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79ad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e79ad-127">Request body</span></span>

<span data-ttu-id="e79ad-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e79ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e79ad-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79ad-129">Response</span></span>

<span data-ttu-id="e79ad-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [identityprovider](../resources/identityprovider.md) e [openIdConnectProvider](../resources/openIdConnectProvider.md) (somente para objetos do Azure ad B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e79ad-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79ad-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e79ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e79ad-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e79ad-132">Request</span></span>

<span data-ttu-id="e79ad-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e79ad-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e79ad-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e79ad-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="e79ad-135">C#</span><span class="sxs-lookup"><span data-stu-id="e79ad-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e79ad-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e79ad-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e79ad-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e79ad-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e79ad-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e79ad-138">Response</span></span>

<span data-ttu-id="e79ad-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e79ad-139">The following is an example of the response.</span></span>

<span data-ttu-id="e79ad-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e79ad-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityProvider",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityProviders",
    "value": [
      {
          "@odata.type": "microsoft.graph.identityProvider",
          "id": "Amazon-OAUTH",
          "name": "Login with Amazon",
          "type": "Amazon",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****"
      },
      {
          "@odata.type": "microsoft.graph.openIdConnectProvider",
          "id": "OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a",
          "name": "Login with the Contoso identity provider",
          "type": "OpenIDConnect",
          "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
          "clientSecret": "*****",
          "claimsMapping": {
              "userId": "myUserId",
              "givenName": "myGivenName",
              "surname": "mySurname",
              "email": "myEmail",
              "displayName": "myDisplayName"
          },
          "domainHint": "contoso",
          "metadataUrl": "https://mycustomoidc.com/.well-known/openid-configuration",
          "responseMode": "form_post",
          "responseType": "code",
          "scope": "openid"
      },
    ]
}
```
