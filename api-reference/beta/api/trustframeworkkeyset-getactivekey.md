---
title: 'trustFrameworkKeySet: getActiveKey'
description: Obtém a chave ativa no conjunto de chaves.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: db234801ed4f4a1f1599d249d95f17b92a1f8afb
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215886"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="bdf62-103">trustFrameworkKeySet: getActiveKey</span><span class="sxs-lookup"><span data-stu-id="bdf62-103">trustFrameworkKeySet: getActiveKey</span></span>

<span data-ttu-id="bdf62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf62-105">Obter o [trustFrameworkKey](../resources/trustframeworkkey.md) ativo no momento em um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="bdf62-105">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="bdf62-106">Somente uma chave está ativa no conjunto de chaves por vez.</span><span class="sxs-lookup"><span data-stu-id="bdf62-106">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="bdf62-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdf62-107">Permissions</span></span>

<span data-ttu-id="bdf62-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdf62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf62-110">Permission type</span></span>                        | <span data-ttu-id="bdf62-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdf62-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bdf62-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf62-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdf62-113">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="bdf62-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="bdf62-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf62-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf62-115">Not supported.</span></span> |
| <span data-ttu-id="bdf62-116">Application</span><span class="sxs-lookup"><span data-stu-id="bdf62-116">Application</span></span>                            | <span data-ttu-id="bdf62-117">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="bdf62-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdf62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf62-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="bdf62-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf62-119">Request headers</span></span>

| <span data-ttu-id="bdf62-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bdf62-120">Name</span></span>          | <span data-ttu-id="bdf62-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf62-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bdf62-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdf62-122">Authorization</span></span> | <span data-ttu-id="bdf62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdf62-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdf62-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf62-125">Request body</span></span>

<span data-ttu-id="bdf62-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bdf62-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf62-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf62-127">Response</span></span>

<span data-ttu-id="bdf62-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf62-128">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bdf62-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bdf62-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bdf62-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf62-130">Request</span></span>

<span data-ttu-id="bdf62-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf62-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdf62-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf62-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="c"></a>[<span data-ttu-id="bdf62-133">C#</span><span class="sxs-lookup"><span data-stu-id="bdf62-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdf62-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdf62-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdf62-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdf62-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bdf62-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf62-136">Response</span></span>

<span data-ttu-id="bdf62-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf62-137">The following is an example of the response.</span></span>

> <span data-ttu-id="bdf62-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdf62-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
