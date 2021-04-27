---
title: Obter reviewSetQuery
description: Recupere as propriedades e as relações de um objeto reviewsetquery de Descoberta eDiscovery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 0fa68102401e4d556da708d0bd1e5263eaf33062
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044659"
---
# <a name="get-reviewsetquery"></a><span data-ttu-id="e8d16-103">Obter reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="e8d16-103">Get reviewSetQuery</span></span>

<span data-ttu-id="e8d16-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="e8d16-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8d16-105">Recupere as propriedades e as relações de um objeto [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) de Descobertas e Descobertas.</span><span class="sxs-lookup"><span data-stu-id="e8d16-105">Retrieve the properties and relationships of an eDiscovery [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d16-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8d16-106">Permissions</span></span>

<span data-ttu-id="e8d16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d16-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8d16-109">Permission type</span></span>|<span data-ttu-id="e8d16-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8d16-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8d16-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8d16-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8d16-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8d16-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="e8d16-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8d16-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8d16-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d16-114">Not supported.</span></span>|
|<span data-ttu-id="e8d16-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8d16-115">Application</span></span>|<span data-ttu-id="e8d16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d16-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8d16-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8d16-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8d16-118">Optional query parameters</span></span>

<span data-ttu-id="e8d16-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8d16-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8d16-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8d16-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-121">Request headers</span></span>

| <span data-ttu-id="e8d16-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e8d16-122">Name</span></span>      |<span data-ttu-id="e8d16-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d16-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8d16-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8d16-124">Authorization</span></span> | <span data-ttu-id="e8d16-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8d16-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8d16-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-127">Request body</span></span>

<span data-ttu-id="e8d16-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8d16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d16-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d16-129">Response</span></span>

<span data-ttu-id="e8d16-130">Se tiver êxito, este método retornará um código de resposta e o objeto `200 OK` [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-130">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8d16-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8d16-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8d16-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d16-132">Request</span></span>

<span data-ttu-id="e8d16-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8d16-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8d16-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d16-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_reviewsetquery"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="e8d16-135">C#</span><span class="sxs-lookup"><span data-stu-id="e8d16-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8d16-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8d16-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8d16-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8d16-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8d16-138">Java</span><span class="sxs-lookup"><span data-stu-id="e8d16-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8d16-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d16-139">Response</span></span>

<span data-ttu-id="e8d16-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d16-140">The following is an example of the response.</span></span>

> <span data-ttu-id="e8d16-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e8d16-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


