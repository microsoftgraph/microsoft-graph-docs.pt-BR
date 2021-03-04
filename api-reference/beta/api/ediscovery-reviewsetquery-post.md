---
title: Criar reviewSetQuery
description: Use essa API para criar uma nova reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 311b9d4571e9b83122d7a69d596a4856342bb941
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445765"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="31632-103">Criar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="31632-103">Create reviewSetQuery</span></span>

<span data-ttu-id="31632-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="31632-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31632-105">Crie um novo [objeto reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="31632-105">Create a new [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="31632-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="31632-106">Permissions</span></span>

<span data-ttu-id="31632-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31632-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="31632-109">Permission type</span></span>|<span data-ttu-id="31632-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="31632-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31632-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="31632-111">Delegated (work or school account)</span></span>|<span data-ttu-id="31632-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31632-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="31632-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="31632-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31632-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31632-114">Not supported.</span></span>|
|<span data-ttu-id="31632-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="31632-115">Application</span></span>|<span data-ttu-id="31632-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="31632-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31632-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="31632-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="31632-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="31632-118">Request headers</span></span>

| <span data-ttu-id="31632-119">Nome</span><span class="sxs-lookup"><span data-stu-id="31632-119">Name</span></span>          | <span data-ttu-id="31632-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="31632-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="31632-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="31632-121">Authorization</span></span> | <span data-ttu-id="31632-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="31632-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="31632-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="31632-124">Request body</span></span>

<span data-ttu-id="31632-125">No corpo da solicitação, fornece uma representação JSON do [objeto reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="31632-125">In the request body, supply a JSON representation of [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span> <span data-ttu-id="31632-126">A tabela a seguir lista as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="31632-126">The following table lists the required properties.</span></span>

| <span data-ttu-id="31632-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31632-127">Property</span></span>     | <span data-ttu-id="31632-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="31632-128">Type</span></span>        | <span data-ttu-id="31632-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="31632-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="31632-130">displayName</span><span class="sxs-lookup"><span data-stu-id="31632-130">displayName</span></span>  | <span data-ttu-id="31632-131">string</span><span class="sxs-lookup"><span data-stu-id="31632-131">string</span></span>      | <span data-ttu-id="31632-132">O nome da consulta conjunto de revisão</span><span class="sxs-lookup"><span data-stu-id="31632-132">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="31632-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="31632-133">Response</span></span>

<span data-ttu-id="31632-134">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="31632-134">If successful, this method returns a `201 Created` response code and a new [microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="31632-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="31632-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="31632-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="31632-136">Request</span></span>

<span data-ttu-id="31632-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="31632-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="31632-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="31632-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reviewsetquery"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries
Content-type: application/json

{
   "displayName":"My Query 1",
   "query":"(subject:\"Quarterly Financials\")"
}
```
# <a name="c"></a>[<span data-ttu-id="31632-139">C#</span><span class="sxs-lookup"><span data-stu-id="31632-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="31632-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="31632-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="31632-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="31632-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="31632-142">Java</span><span class="sxs-lookup"><span data-stu-id="31632-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="31632-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="31632-143">Response</span></span>

<span data-ttu-id="31632-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="31632-144">The following is an example of the response.</span></span>

> <span data-ttu-id="31632-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="31632-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery"
} -->

```http
HTTP/1.1 201 Created
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
    "query": "(subject:\"Quarterly Financials\")"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


