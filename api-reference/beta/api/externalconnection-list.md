---
title: Listar conexões
description: Recupere uma lista de externalConnections.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c47d2e58bed88748e6b05e3099bc1d2d930bbb9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422254"
---
# <a name="list-connections"></a><span data-ttu-id="37a11-103">Listar conexões</span><span class="sxs-lookup"><span data-stu-id="37a11-103">List connections</span></span>

<span data-ttu-id="37a11-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="37a11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a11-105">Recupere uma lista de [externalConnections](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="37a11-105">Retrieve a list of [externalConnections](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="37a11-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37a11-106">Permissions</span></span>

<span data-ttu-id="37a11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="37a11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37a11-109">Permission type</span></span>                        | <span data-ttu-id="37a11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37a11-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="37a11-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37a11-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="37a11-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a11-112">Not supported.</span></span> |
| <span data-ttu-id="37a11-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37a11-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37a11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37a11-114">Not supported.</span></span> |
| <span data-ttu-id="37a11-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37a11-115">Application</span></span>                            | <span data-ttu-id="37a11-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37a11-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37a11-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37a11-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37a11-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37a11-118">Optional query parameters</span></span>

<span data-ttu-id="37a11-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37a11-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37a11-120">Request headers</span></span>

| <span data-ttu-id="37a11-121">Nome</span><span class="sxs-lookup"><span data-stu-id="37a11-121">Name</span></span>          | <span data-ttu-id="37a11-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="37a11-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="37a11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="37a11-123">Authorization</span></span> | <span data-ttu-id="37a11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37a11-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37a11-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37a11-126">Request body</span></span>

<span data-ttu-id="37a11-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37a11-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a11-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a11-128">Response</span></span>

<span data-ttu-id="37a11-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [externalConnection](../resources/externalconnection.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37a11-129">If successful, this method returns a `200 OK` response code and a collection of [externalConnection](../resources/externalconnection.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a11-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37a11-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37a11-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37a11-131">Request</span></span>

<span data-ttu-id="37a11-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37a11-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37a11-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a11-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connections"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/external/connections
```
# <a name="c"></a>[<span data-ttu-id="37a11-134">C#</span><span class="sxs-lookup"><span data-stu-id="37a11-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a11-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a11-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a11-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a11-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="37a11-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="37a11-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="37a11-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37a11-138">The following is an example of the response.</span></span>

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
