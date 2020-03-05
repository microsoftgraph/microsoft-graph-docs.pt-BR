---
title: Obter trustFrameworkKeySet
description: Recupere as propriedades e os relacionamentos do objeto trustframeworkkeyset.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a6b9fd69b1de7ece70cd405b18c95c5cb3131d2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452160"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="06990-103">Obter trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="06990-103">Get trustFrameworkKeySet</span></span>

<span data-ttu-id="06990-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="06990-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06990-105">Recupere as propriedades e associações de um [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="06990-105">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06990-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="06990-106">Permissions</span></span>

<span data-ttu-id="06990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06990-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06990-109">Permission type</span></span>                        | <span data-ttu-id="06990-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06990-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06990-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06990-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06990-112">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="06990-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="06990-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06990-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06990-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="06990-114">Not supported.</span></span> |
| <span data-ttu-id="06990-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06990-115">Application</span></span>                            | <span data-ttu-id="06990-116">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="06990-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06990-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06990-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="06990-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06990-118">Request headers</span></span>

| <span data-ttu-id="06990-119">Nome</span><span class="sxs-lookup"><span data-stu-id="06990-119">Name</span></span>      |<span data-ttu-id="06990-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="06990-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06990-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="06990-121">Authorization</span></span> | <span data-ttu-id="06990-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06990-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06990-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06990-124">Request body</span></span>

<span data-ttu-id="06990-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06990-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06990-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="06990-126">Response</span></span>

<span data-ttu-id="06990-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06990-127">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06990-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="06990-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06990-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06990-129">Request</span></span>

<span data-ttu-id="06990-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="06990-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06990-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="06990-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="06990-132">C#</span><span class="sxs-lookup"><span data-stu-id="06990-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06990-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06990-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06990-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06990-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06990-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="06990-135">Response</span></span>

<span data-ttu-id="06990-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="06990-136">The following is an example of the response.</span></span>

> <span data-ttu-id="06990-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="06990-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
