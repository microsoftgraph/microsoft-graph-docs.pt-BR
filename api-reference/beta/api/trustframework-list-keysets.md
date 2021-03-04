---
title: Listar keySets
description: Recupere uma lista de objetos trustframeworkkeyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f908c3c410eb99dac93717d14fa28db5efe65bb0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444978"
---
# <a name="list-keysets"></a><span data-ttu-id="7bf2a-103">Listar keySets</span><span class="sxs-lookup"><span data-stu-id="7bf2a-103">List keySets</span></span>

<span data-ttu-id="7bf2a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bf2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf2a-105">Recupere uma lista de [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="7bf2a-105">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf2a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bf2a-106">Permissions</span></span>

<span data-ttu-id="7bf2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7bf2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bf2a-109">Permission type</span></span>                        | <span data-ttu-id="7bf2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bf2a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7bf2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bf2a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7bf2a-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf2a-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="7bf2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bf2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bf2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-114">Not supported.</span></span> |
| <span data-ttu-id="7bf2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bf2a-115">Application</span></span>                            | <span data-ttu-id="7bf2a-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf2a-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf2a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="7bf2a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf2a-118">Request headers</span></span>

| <span data-ttu-id="7bf2a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7bf2a-119">Name</span></span>      |<span data-ttu-id="7bf2a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bf2a-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7bf2a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bf2a-121">Authorization</span></span> | <span data-ttu-id="7bf2a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bf2a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf2a-124">Request body</span></span>

<span data-ttu-id="7bf2a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7bf2a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf2a-126">Response</span></span>

<span data-ttu-id="7bf2a-127">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos trustFrameworkKeySet](../resources/trustframeworkkeyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-127">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7bf2a-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7bf2a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7bf2a-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf2a-129">Request</span></span>

<span data-ttu-id="7bf2a-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7bf2a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf2a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets
```
# <a name="c"></a>[<span data-ttu-id="7bf2a-132">C#</span><span class="sxs-lookup"><span data-stu-id="7bf2a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-keysets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bf2a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bf2a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-keysets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bf2a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bf2a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-keysets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bf2a-135">Java</span><span class="sxs-lookup"><span data-stu-id="7bf2a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-keysets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7bf2a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf2a-136">Response</span></span>

<span data-ttu-id="7bf2a-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="7bf2a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bf2a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "keys": [
        {
          "k": "k-value",
          "x5c": [
            "x5c-value"
          ],
          "x5t": "x5t-value",
          "kty": "kty-value",
          "use": "use-value",
          "exp": 99,
          "nbf": 99,
          "kid": "kid-value",
          "e": "e-value",
          "n": "n-value",
          "d": "d-value",
          "p": "p-value",
          "q": "q-value",
          "dp": "dp-value",
          "dq": "dq-value",
          "qi": "qi-value"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List keySets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


