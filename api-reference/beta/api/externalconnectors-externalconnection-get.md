---
title: Obter conexão
description: Recupere as propriedades e as relações de um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 5f545343bc67b20fab59d48cce21077769c2960a
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467555"
---
# <a name="get-connection"></a><span data-ttu-id="2271d-103">Obter conexão</span><span class="sxs-lookup"><span data-stu-id="2271d-103">Get connection</span></span>

<span data-ttu-id="2271d-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="2271d-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2271d-105">Recupere as propriedades e as relações de [um externalConnection](../resources/externalconnectors-externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="2271d-105">Retrieve the properties and relationships of an [externalConnection](../resources/externalconnectors-externalconnection.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2271d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2271d-106">Permissions</span></span>

<span data-ttu-id="2271d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2271d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2271d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2271d-109">Permission type</span></span>                        | <span data-ttu-id="2271d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2271d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2271d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2271d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2271d-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2271d-112">Not supported.</span></span> |
| <span data-ttu-id="2271d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2271d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2271d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2271d-114">Not supported.</span></span> |
| <span data-ttu-id="2271d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2271d-115">Application</span></span>                            | <span data-ttu-id="2271d-116">ExternalConnection.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2271d-116">ExternalConnection.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="2271d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2271d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2271d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2271d-118">Optional query parameters</span></span>

<span data-ttu-id="2271d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2271d-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2271d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2271d-120">Request headers</span></span>

| <span data-ttu-id="2271d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2271d-121">Name</span></span>          | <span data-ttu-id="2271d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2271d-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2271d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2271d-123">Authorization</span></span> | <span data-ttu-id="2271d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2271d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2271d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2271d-126">Request body</span></span>

<span data-ttu-id="2271d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2271d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2271d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2271d-128">Response</span></span>

<span data-ttu-id="2271d-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [externalConnection](../resources/externalconnectors-externalconnection.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2271d-129">If successful, this method returns a `200 OK` response code and the requested [externalConnection](../resources/externalconnectors-externalconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2271d-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2271d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2271d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2271d-131">Request</span></span>

<span data-ttu-id="2271d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2271d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2271d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2271d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connection"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="2271d-134">C#</span><span class="sxs-lookup"><span data-stu-id="2271d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2271d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2271d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2271d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2271d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2271d-137">Java</span><span class="sxs-lookup"><span data-stu-id="2271d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2271d-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2271d-138">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2271d-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2271d-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalConnection"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contosohr",
  "name": "Contoso HR",
  "description": "Connection to index Contoso HR system",
  "state": "ready",
  "configuration": {
    "authorizedAppIds": [
      "d310d35d-72ec-47dd-92f2-fb9c40936555"
    ]
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
