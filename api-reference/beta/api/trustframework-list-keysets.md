---
title: Listar conjuntos de
description: Recupere uma lista de objetos trustframeworkkeyset.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 229ec09241de019910781a3bf37fe2c39db2c399
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734526"
---
# <a name="list-keysets"></a><span data-ttu-id="592da-103">Listar conjuntos de</span><span class="sxs-lookup"><span data-stu-id="592da-103">List keySets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="592da-104">Recupere uma lista de [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="592da-104">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="592da-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="592da-105">Permissions</span></span>

<span data-ttu-id="592da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="592da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="592da-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="592da-108">Permission type</span></span>                        | <span data-ttu-id="592da-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="592da-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="592da-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="592da-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="592da-111">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="592da-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="592da-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="592da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="592da-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="592da-113">Not supported.</span></span> |
| <span data-ttu-id="592da-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="592da-114">Application</span></span>                            | <span data-ttu-id="592da-115">TrustFrameworkKeySet. Read. All, TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="592da-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="592da-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="592da-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="592da-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="592da-117">Request headers</span></span>

| <span data-ttu-id="592da-118">Nome</span><span class="sxs-lookup"><span data-stu-id="592da-118">Name</span></span>      |<span data-ttu-id="592da-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="592da-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="592da-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="592da-120">Authorization</span></span> | <span data-ttu-id="592da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="592da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="592da-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="592da-123">Request body</span></span>

<span data-ttu-id="592da-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="592da-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="592da-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="592da-125">Response</span></span>

<span data-ttu-id="592da-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="592da-126">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="592da-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="592da-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="592da-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="592da-128">Request</span></span>

<span data-ttu-id="592da-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="592da-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```http
GET https://graph.microsoft.com/beta/trustFramework/keySets
```

### <a name="response"></a><span data-ttu-id="592da-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="592da-130">Response</span></span>

<span data-ttu-id="592da-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="592da-131">The following is an example of the response.</span></span>

> <span data-ttu-id="592da-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="592da-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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