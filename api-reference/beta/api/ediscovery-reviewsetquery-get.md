---
title: Obter reviewSetQuery
description: Recupere as propriedades e as relações de um objeto reviewsetquery de Descoberta eDiscovery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3ddc2c3e3c7231d0bdf8ec81a12e49b4c016a83a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445768"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="a0dc9-103">Obter reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="a0dc9-103">Get reviewSetQuery</span></span>

<span data-ttu-id="a0dc9-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a0dc9-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0dc9-105">Recupere as propriedades e as relações de um objeto [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) de Descobertas e Descobertas.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-105">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0dc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0dc9-106">Permissions</span></span>

<span data-ttu-id="a0dc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0dc9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0dc9-109">Permission type</span></span>|<span data-ttu-id="a0dc9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0dc9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0dc9-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0dc9-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="a0dc9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0dc9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0dc9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-114">Not supported.</span></span>|
|<span data-ttu-id="a0dc9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0dc9-115">Application</span></span>|<span data-ttu-id="a0dc9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0dc9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dc9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0dc9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0dc9-118">Optional query parameters</span></span>

<span data-ttu-id="a0dc9-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a0dc9-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0dc9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0dc9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-121">Request headers</span></span>

| <span data-ttu-id="a0dc9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a0dc9-122">Name</span></span>      |<span data-ttu-id="a0dc9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0dc9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a0dc9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0dc9-124">Authorization</span></span> | <span data-ttu-id="a0dc9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0dc9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-127">Request body</span></span>

<span data-ttu-id="a0dc9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0dc9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dc9-129">Response</span></span>

<span data-ttu-id="a0dc9-130">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0dc9-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0dc9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0dc9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0dc9-132">Request</span></span>

<span data-ttu-id="a0dc9-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0dc9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0dc9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="a0dc9-135">C#</span><span class="sxs-lookup"><span data-stu-id="a0dc9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0dc9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0dc9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0dc9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0dc9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0dc9-138">Java</span><span class="sxs-lookup"><span data-stu-id="a0dc9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a0dc9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0dc9-139">Response</span></span>

<span data-ttu-id="a0dc9-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-140">The following is an example of the response.</span></span>

> <span data-ttu-id="a0dc9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0dc9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases('2eef613a-ca2d-42f4-89fe-84d5198ddedf')/reviewSets('b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8')/queries/$entity",
    "id": "6b5358b0-2ce2-4369-b9cf-65392fe56807",
    "displayName": "My Query 1",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-03-09T09:05:12.3756813Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-03-09T09:05:12.3756813Z",
    "query": "subject:\"Quarterly Financials\""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


