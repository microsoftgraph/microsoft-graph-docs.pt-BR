---
title: 'trustFrameworkKeySet: getActiveKey'
description: Obtém a chave ativa no conjunto de chaves.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ea4e1e31812bdbdb7a8e6619280367a5ed873fc9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937529"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="4d471-103">trustFrameworkKeySet: getActiveKey</span><span class="sxs-lookup"><span data-stu-id="4d471-103">trustFrameworkKeySet: getActiveKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d471-104">Obter o [trustFrameworkKey](../resources/trustframeworkkey.md) ativo no momento em um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="4d471-104">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="4d471-105">Somente uma chave está ativa no conjunto de chaves por vez.</span><span class="sxs-lookup"><span data-stu-id="4d471-105">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="4d471-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d471-106">Permissions</span></span>

<span data-ttu-id="4d471-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d471-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4d471-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d471-109">Permission type</span></span>                        | <span data-ttu-id="4d471-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d471-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4d471-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d471-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4d471-112">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="4d471-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="4d471-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d471-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d471-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d471-114">Not supported.</span></span> |
| <span data-ttu-id="4d471-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d471-115">Application</span></span>                            | <span data-ttu-id="4d471-116">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="4d471-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d471-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d471-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="4d471-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d471-118">Request headers</span></span>

| <span data-ttu-id="4d471-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4d471-119">Name</span></span>          | <span data-ttu-id="4d471-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d471-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4d471-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d471-121">Authorization</span></span> | <span data-ttu-id="4d471-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d471-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d471-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d471-124">Request body</span></span>

<span data-ttu-id="4d471-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d471-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d471-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d471-126">Response</span></span>

<span data-ttu-id="4d471-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [trustFrameworkKey](../resources/trustframeworkkey.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d471-127">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4d471-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4d471-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4d471-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d471-129">Request</span></span>

<span data-ttu-id="4d471-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d471-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d471-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d471-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d471-132">C#</span><span class="sxs-lookup"><span data-stu-id="4d471-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d471-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d471-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d471-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d471-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4d471-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d471-135">Response</span></span>

<span data-ttu-id="4d471-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4d471-136">The following is an example of the response.</span></span>

> <span data-ttu-id="4d471-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d471-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
