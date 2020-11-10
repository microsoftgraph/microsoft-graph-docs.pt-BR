---
title: Listar conexões
description: Recupere uma lista de externalConnections.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b70e1fc69c5897e8209633e5b5ce0f35cb7fb41a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965626"
---
# <a name="list-connections"></a><span data-ttu-id="be1de-103">Listar conexões</span><span class="sxs-lookup"><span data-stu-id="be1de-103">List connections</span></span>

<span data-ttu-id="be1de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be1de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be1de-105">Recupere uma lista de [externalConnections](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="be1de-105">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="be1de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be1de-106">Permissions</span></span>

<span data-ttu-id="be1de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be1de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="be1de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be1de-109">Permission type</span></span>                        | <span data-ttu-id="be1de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be1de-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="be1de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be1de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="be1de-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be1de-112">Not supported.</span></span> |
| <span data-ttu-id="be1de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be1de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be1de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be1de-114">Not supported.</span></span> |
| <span data-ttu-id="be1de-115">Application</span><span class="sxs-lookup"><span data-stu-id="be1de-115">Application</span></span>                            | <span data-ttu-id="be1de-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be1de-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be1de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be1de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="be1de-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be1de-118">Optional query parameters</span></span>

<span data-ttu-id="be1de-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be1de-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be1de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be1de-120">Request headers</span></span>

| <span data-ttu-id="be1de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="be1de-121">Name</span></span>          | <span data-ttu-id="be1de-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="be1de-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="be1de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="be1de-123">Authorization</span></span> | <span data-ttu-id="be1de-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be1de-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be1de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be1de-126">Request body</span></span>

<span data-ttu-id="be1de-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be1de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be1de-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1de-128">Response</span></span>

<span data-ttu-id="be1de-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be1de-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="be1de-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="be1de-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="be1de-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be1de-131">Request</span></span>

<span data-ttu-id="be1de-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="be1de-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="be1de-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="be1de-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="be1de-134">C#</span><span class="sxs-lookup"><span data-stu-id="be1de-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="be1de-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="be1de-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="be1de-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="be1de-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="be1de-137">Java</span><span class="sxs-lookup"><span data-stu-id="be1de-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="be1de-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="be1de-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="be1de-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="be1de-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnection",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contosohr",
      "name": "Contoso HR",
      "description": "Connection to index Contoso HR system",
      "configuration": {
        "authorizedApps": [
          "d310d35d-72ec-47dd-92f2-fb9c40936555"
        ]
      }
    },
    {
      "id": "contosofinance",
      "name": "Contoso Finance",
      "description": "Connection to index Contoso Finance system",
      "configuration": {
        "authorizedApps": [
          "fbdc7d4e-07f4-4143-8258-e5a2fcebeadb"
        ]
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


