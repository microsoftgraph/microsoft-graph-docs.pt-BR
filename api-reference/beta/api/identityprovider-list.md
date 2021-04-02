---
title: Lista identityProviders
description: Recupere uma lista de objetos identityProvider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 099f77722e6f08a27dea01200246320cd8ae4eec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507817"
---
# <a name="list-identityproviders-deprecated"></a><span data-ttu-id="056b6-103">Listar identityProviders (preterido)</span><span class="sxs-lookup"><span data-stu-id="056b6-103">List identityProviders (deprecated)</span></span>
<span data-ttu-id="056b6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="056b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [identityprovider-deprecate](../../includes/identityprovider-deprecate.md)]

<span data-ttu-id="056b6-105">Recupere uma lista de [objetos identityProviders.](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="056b6-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="056b6-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="056b6-106">Permissions</span></span>

<span data-ttu-id="056b6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="056b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="056b6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="056b6-109">Permission type</span></span>      | <span data-ttu-id="056b6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="056b6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="056b6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="056b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="056b6-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="056b6-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="056b6-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="056b6-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="056b6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="056b6-114">Not supported.</span></span>|
|<span data-ttu-id="056b6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="056b6-115">Application</span></span>|<span data-ttu-id="056b6-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="056b6-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="056b6-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="056b6-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="056b6-118">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="056b6-118">Global Administrator</span></span>
* <span data-ttu-id="056b6-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="056b6-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="056b6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="056b6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="056b6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="056b6-121">Request headers</span></span>

|<span data-ttu-id="056b6-122">Nome</span><span class="sxs-lookup"><span data-stu-id="056b6-122">Name</span></span>|<span data-ttu-id="056b6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="056b6-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="056b6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="056b6-124">Authorization</span></span>|<span data-ttu-id="056b6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="056b6-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="056b6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="056b6-127">Request body</span></span>

<span data-ttu-id="056b6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="056b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="056b6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="056b6-129">Response</span></span>

<span data-ttu-id="056b6-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [identityProvider](../resources/identityprovider.md) e [openIdConnectProvider](../resources/openIdConnectProvider.md) (somente para objetos do Azure AD B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="056b6-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="056b6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="056b6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="056b6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="056b6-132">Request</span></span>

<span data-ttu-id="056b6-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="056b6-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="056b6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="056b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityprovider_3"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```
# <a name="c"></a>[<span data-ttu-id="056b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="056b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityprovider-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="056b6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="056b6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityprovider-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="056b6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="056b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityprovider-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="056b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="056b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityprovider-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="056b6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="056b6-139">Response</span></span>

<span data-ttu-id="056b6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="056b6-140">The following is an example of the response.</span></span>

<span data-ttu-id="056b6-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="056b6-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
