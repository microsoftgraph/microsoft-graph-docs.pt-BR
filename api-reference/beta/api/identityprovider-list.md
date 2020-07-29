---
title: Lista identityProviders
description: Recupere uma lista de objetos identityprovider.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 640844dd4d1a60b5a4c5864c9ea7d34fe01faabb
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509719"
---
# <a name="list-identityproviders"></a><span data-ttu-id="e5085-103">Lista identityProviders</span><span class="sxs-lookup"><span data-stu-id="e5085-103">List identityProviders</span></span>

<span data-ttu-id="e5085-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5085-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5085-105">Recupere uma lista de objetos [identityProviders](../resources/identityprovider.md) .</span><span class="sxs-lookup"><span data-stu-id="e5085-105">Retrieve a list of [identityProviders](../resources/identityprovider.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5085-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5085-106">Permissions</span></span>

<span data-ttu-id="e5085-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5085-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5085-109">Permission type</span></span>      | <span data-ttu-id="e5085-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5085-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5085-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5085-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5085-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5085-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="e5085-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5085-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e5085-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5085-114">Not supported.</span></span>|
|<span data-ttu-id="e5085-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5085-115">Application</span></span>|<span data-ttu-id="e5085-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5085-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="e5085-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e5085-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="e5085-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e5085-118">Global administrator</span></span>
* <span data-ttu-id="e5085-119">Administrador do provedor de identidade externa</span><span class="sxs-lookup"><span data-stu-id="e5085-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e5085-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5085-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="e5085-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5085-121">Request headers</span></span>

|<span data-ttu-id="e5085-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e5085-122">Name</span></span>|<span data-ttu-id="e5085-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5085-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e5085-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5085-124">Authorization</span></span>|<span data-ttu-id="e5085-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5085-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5085-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5085-127">Request body</span></span>

<span data-ttu-id="e5085-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5085-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5085-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5085-129">Response</span></span>

<span data-ttu-id="e5085-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção de [identityprovider](../resources/identityprovider.md) e [openIdConnectProvider](../resources/openIdConnectProvider.md) (somente para objetos do Azure ad B2C) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5085-130">If successful, this method returns a `200 OK` response code and a collection of [identityProvider](../resources/identityprovider.md) and [openIdConnectProvider](../resources/openIdConnectProvider.md) (only for Azure AD B2C) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5085-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5085-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5085-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5085-132">Request</span></span>

<span data-ttu-id="e5085-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5085-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders
```

### <a name="response"></a><span data-ttu-id="e5085-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5085-134">Response</span></span>

<span data-ttu-id="e5085-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5085-135">The following is an example of the response.</span></span>

<span data-ttu-id="e5085-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5085-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
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
