---
title: Listar reviewSetQueries
description: Recupere uma lista de objetos reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 079448350236fda5febdea00cc850e4a185be030
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445767"
---
# <a name="list-reviewsetqueries"></a><span data-ttu-id="42ab1-103">Listar reviewSetQueries</span><span class="sxs-lookup"><span data-stu-id="42ab1-103">List reviewSetQueries</span></span>

<span data-ttu-id="42ab1-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="42ab1-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42ab1-105">Recupere uma lista de objetos eDiscovery [reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="42ab1-105">Retrieve a list of eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="42ab1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="42ab1-106">Permissions</span></span>

<span data-ttu-id="42ab1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42ab1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42ab1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42ab1-109">Permission type</span></span>|<span data-ttu-id="42ab1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42ab1-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42ab1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42ab1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="42ab1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42ab1-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="42ab1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42ab1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42ab1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42ab1-114">Not supported.</span></span>|
|<span data-ttu-id="42ab1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42ab1-115">Application</span></span>|<span data-ttu-id="42ab1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42ab1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42ab1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42ab1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="42ab1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="42ab1-118">Optional query parameters</span></span>

<span data-ttu-id="42ab1-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="42ab1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="42ab1-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="42ab1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="42ab1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42ab1-121">Request headers</span></span>

| <span data-ttu-id="42ab1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="42ab1-122">Name</span></span>      |<span data-ttu-id="42ab1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="42ab1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="42ab1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="42ab1-124">Authorization</span></span> | <span data-ttu-id="42ab1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42ab1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42ab1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42ab1-127">Request body</span></span>

<span data-ttu-id="42ab1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42ab1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42ab1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="42ab1-129">Response</span></span>

<span data-ttu-id="42ab1-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42ab1-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42ab1-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42ab1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42ab1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42ab1-132">Request</span></span>

<span data-ttu-id="42ab1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42ab1-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42ab1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="42ab1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
```
# <a name="c"></a>[<span data-ttu-id="42ab1-135">C#</span><span class="sxs-lookup"><span data-stu-id="42ab1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42ab1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42ab1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42ab1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42ab1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42ab1-138">Java</span><span class="sxs-lookup"><span data-stu-id="42ab1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42ab1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42ab1-139">Response</span></span>

<span data-ttu-id="42ab1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42ab1-140">The following is an example of the response.</span></span>

> <span data-ttu-id="42ab1-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42ab1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries",
    "@odata.nextLink": "https://graph.microsoft.com/beta/compliance/ediscovery/cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries?$skipToken=<encodedPageToken>",
    "value": [
        {
            "id": "f7859ebb-5546-4f96-937a-9cf5723e9809",
            "displayName": "Query 1",
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T12:07:52.6520503Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T12:07:52.6520503Z",
            "query": "(Cc:aa)"
        },
        {
            "id": "7c4b98e1-fe18-4887-be81-79f7a24b15c8",
            "displayName": "New query1",
            "description": null,
            "createdBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "createdDateTime": "2020-03-02T16:17:19.3564678Z",
            "lastModifiedBy": {
                "user": {
                    "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
                    "displayName": "eDiscovery admin"
                }
            },
            "lastModifiedDateTime": "2020-03-02T16:17:19.3564678Z",
            "query": "subject:\"Quarterly Financials\""
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List queries",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


