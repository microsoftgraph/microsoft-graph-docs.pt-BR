---
title: 'trustFrameworkKeySet: getActiveKey'
description: Obter a chave ativa no keyset.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e0d94153e675e5c5c8da58b61eaf4f7166e5e239
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433639"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="a606a-103">trustFrameworkKeySet: getActiveKey</span><span class="sxs-lookup"><span data-stu-id="a606a-103">trustFrameworkKeySet: getActiveKey</span></span>

<span data-ttu-id="a606a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a606a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a606a-105">Obter o [trustFrameworkKey ativo](../resources/trustframeworkkey.md) no momento em [um trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="a606a-105">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="a606a-106">Somente uma chave está ativa no keyset de cada vez.</span><span class="sxs-lookup"><span data-stu-id="a606a-106">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="a606a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a606a-107">Permissions</span></span>

<span data-ttu-id="a606a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a606a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a606a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a606a-110">Permission type</span></span>                        | <span data-ttu-id="a606a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a606a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a606a-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a606a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a606a-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a606a-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="a606a-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a606a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a606a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a606a-115">Not supported.</span></span> |
| <span data-ttu-id="a606a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a606a-116">Application</span></span>                            | <span data-ttu-id="a606a-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a606a-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a606a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a606a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="a606a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a606a-119">Request headers</span></span>

| <span data-ttu-id="a606a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a606a-120">Name</span></span>          | <span data-ttu-id="a606a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a606a-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a606a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a606a-122">Authorization</span></span> | <span data-ttu-id="a606a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a606a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a606a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a606a-125">Request body</span></span>

<span data-ttu-id="a606a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a606a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a606a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a606a-127">Response</span></span>

<span data-ttu-id="a606a-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a606a-128">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a606a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a606a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a606a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a606a-130">Request</span></span>

<span data-ttu-id="a606a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a606a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a606a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a606a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="c"></a>[<span data-ttu-id="a606a-133">C#</span><span class="sxs-lookup"><span data-stu-id="a606a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a606a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a606a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a606a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a606a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a606a-136">Java</span><span class="sxs-lookup"><span data-stu-id="a606a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-getactivekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a606a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a606a-137">Response</span></span>

<span data-ttu-id="a606a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a606a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="a606a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a606a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "k": "k-value",
  "x5c": [
    "x5c-value"
  ],
  "x5t": "x5t-value",
  "kty": "kty-value",
  "use": "use-value",
  "exp": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: getActiveKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


