---
title: Obter trustFrameworkKeySet
description: Recupere as propriedades e os relacionamentos do objeto trustframeworkkeyset.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e70f0cf3e7eaae0add9da7ded068b8c3517529bc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734514"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="92e5e-103">Obter trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="92e5e-103">Get trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92e5e-104">Recupere as propriedades e associações de um [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="92e5e-104">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92e5e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="92e5e-105">Permissions</span></span>

<span data-ttu-id="92e5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="92e5e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92e5e-108">Permission type</span></span>                        | <span data-ttu-id="92e5e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92e5e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="92e5e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92e5e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="92e5e-111">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92e5e-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="92e5e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92e5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92e5e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92e5e-113">Not supported.</span></span> |
| <span data-ttu-id="92e5e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92e5e-114">Application</span></span>                            | <span data-ttu-id="92e5e-115">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="92e5e-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="92e5e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92e5e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="92e5e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92e5e-117">Request headers</span></span>

| <span data-ttu-id="92e5e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="92e5e-118">Name</span></span>      |<span data-ttu-id="92e5e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="92e5e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92e5e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="92e5e-120">Authorization</span></span> | <span data-ttu-id="92e5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92e5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92e5e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92e5e-123">Request body</span></span>

<span data-ttu-id="92e5e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="92e5e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92e5e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e5e-125">Response</span></span>

<span data-ttu-id="92e5e-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92e5e-126">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="92e5e-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="92e5e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="92e5e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92e5e-128">Request</span></span>

<span data-ttu-id="92e5e-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="92e5e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="92e5e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="92e5e-130">Response</span></span>

<span data-ttu-id="92e5e-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="92e5e-131">The following is an example of the response.</span></span>

> <span data-ttu-id="92e5e-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92e5e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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