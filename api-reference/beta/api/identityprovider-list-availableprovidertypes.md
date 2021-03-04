---
title: Listar availableProviderTypes
description: Recupere todos os tipos de provedores de identidade disponíveis no diretório.
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: ef78aea89344c480e9a0bc9a89e19144b7726ea0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435466"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="35a06-103">Listar availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="35a06-103">List availableProviderTypes</span></span>

<span data-ttu-id="35a06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35a06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35a06-105">Recupera todos os tipos de provedor de identidade disponíveis em um diretório.</span><span class="sxs-lookup"><span data-stu-id="35a06-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="35a06-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35a06-106">Permissions</span></span>

<span data-ttu-id="35a06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35a06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35a06-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35a06-109">Permission type</span></span>      | <span data-ttu-id="35a06-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35a06-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35a06-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35a06-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35a06-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35a06-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="35a06-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35a06-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="35a06-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35a06-114">Not supported.</span></span>|
|<span data-ttu-id="35a06-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35a06-115">Application</span></span>|<span data-ttu-id="35a06-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35a06-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="35a06-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="35a06-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="35a06-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="35a06-118">Global administrator</span></span>
* <span data-ttu-id="35a06-119">Administrador do Provedor de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="35a06-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="35a06-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35a06-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="35a06-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35a06-121">Request headers</span></span>

|<span data-ttu-id="35a06-122">Nome</span><span class="sxs-lookup"><span data-stu-id="35a06-122">Name</span></span>|<span data-ttu-id="35a06-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="35a06-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="35a06-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="35a06-124">Authorization</span></span>|<span data-ttu-id="35a06-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35a06-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="35a06-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35a06-127">Request body</span></span>
<span data-ttu-id="35a06-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35a06-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35a06-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="35a06-129">Response</span></span>

<span data-ttu-id="35a06-130">Se tiver êxito, essa função retornará o código de resposta `200 OK` e a Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35a06-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35a06-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35a06-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="35a06-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35a06-132">Request</span></span>
<span data-ttu-id="35a06-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="35a06-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35a06-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="35a06-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identityProviders/availableProviderTypes
```
# <a name="c"></a>[<span data-ttu-id="35a06-135">C#</span><span class="sxs-lookup"><span data-stu-id="35a06-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityprovider-availableprovidertypes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35a06-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35a06-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityprovider-availableprovidertypes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35a06-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35a06-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityprovider-availableprovidertypes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35a06-138">Java</span><span class="sxs-lookup"><span data-stu-id="35a06-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityprovider-availableprovidertypes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35a06-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="35a06-139">Response</span></span>

<span data-ttu-id="35a06-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="35a06-140">The following is an example of the response.</span></span>

<span data-ttu-id="35a06-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35a06-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
      "Amazon",
      "OpenIDConnect",
      "Facebook",
      "GitHub",
      "Google",
      "LinkedIn",
      "Microsoft",
      "QQ",
      "Twitter",
      "WeChat",
      "Weibo"
  ]
}
```


