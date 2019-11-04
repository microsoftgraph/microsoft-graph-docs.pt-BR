---
title: Obter trustFrameworkKeySet
description: Recupere as propriedades e os relacionamentos do objeto trustframeworkkeyset.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b5bbeee97ce2bf5c6d70dfb316b78737d3c7b70
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938243"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="9a513-103">Obter trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="9a513-103">Get trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a513-104">Recupere as propriedades e associações de um [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="9a513-104">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a513-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a513-105">Permissions</span></span>

<span data-ttu-id="9a513-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9a513-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a513-108">Permission type</span></span>                        | <span data-ttu-id="9a513-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a513-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9a513-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a513-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9a513-111">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9a513-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="9a513-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a513-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a513-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a513-113">Not supported.</span></span> |
| <span data-ttu-id="9a513-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a513-114">Application</span></span>                            | <span data-ttu-id="9a513-115">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9a513-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a513-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a513-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9a513-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a513-117">Request headers</span></span>

| <span data-ttu-id="9a513-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9a513-118">Name</span></span>      |<span data-ttu-id="9a513-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a513-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a513-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a513-120">Authorization</span></span> | <span data-ttu-id="9a513-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a513-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a513-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a513-123">Request body</span></span>

<span data-ttu-id="9a513-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a513-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a513-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a513-125">Response</span></span>

<span data-ttu-id="9a513-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a513-126">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9a513-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9a513-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9a513-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a513-128">Request</span></span>

<span data-ttu-id="9a513-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a513-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a513-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a513-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a513-131">C#</span><span class="sxs-lookup"><span data-stu-id="9a513-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a513-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a513-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a513-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a513-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9a513-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a513-134">Response</span></span>

<span data-ttu-id="9a513-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a513-135">The following is an example of the response.</span></span>

> <span data-ttu-id="9a513-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a513-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
