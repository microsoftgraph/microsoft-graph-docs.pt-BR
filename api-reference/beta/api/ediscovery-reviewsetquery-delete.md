---
title: Excluir reviewSetQuery
description: Exclua um objeto reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 01120e7702c2dc055ed0827d41b827a7330827bb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445770"
---
# <a name="delete-reviewsetquery"></a><span data-ttu-id="fae0a-103">Excluir reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="fae0a-103">Delete reviewSetQuery</span></span>

<span data-ttu-id="fae0a-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="fae0a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fae0a-105">Exclua [um objeto reviewSetQuery.](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="fae0a-105">Delete a [reviewSetQuery](../resources/ediscovery-reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fae0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fae0a-106">Permissions</span></span>

<span data-ttu-id="fae0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fae0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fae0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fae0a-109">Permission type</span></span>|<span data-ttu-id="fae0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fae0a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fae0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fae0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fae0a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fae0a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="fae0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fae0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fae0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fae0a-114">Not supported.</span></span>|
|<span data-ttu-id="fae0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fae0a-115">Application</span></span>|<span data-ttu-id="fae0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fae0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fae0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fae0a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fae0a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fae0a-118">Request headers</span></span>

| <span data-ttu-id="fae0a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fae0a-119">Name</span></span>          | <span data-ttu-id="fae0a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fae0a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fae0a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fae0a-121">Authorization</span></span> | <span data-ttu-id="fae0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fae0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fae0a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fae0a-124">Request body</span></span>

<span data-ttu-id="fae0a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fae0a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fae0a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fae0a-126">Response</span></span>

<span data-ttu-id="fae0a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fae0a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fae0a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fae0a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fae0a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fae0a-130">Request</span></span>

<span data-ttu-id="fae0a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fae0a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fae0a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="fae0a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_reviewsetquery"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries/6b5358b0-2ce2-4369-b9cf-65392fe56807
```
# <a name="c"></a>[<span data-ttu-id="fae0a-133">C#</span><span class="sxs-lookup"><span data-stu-id="fae0a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fae0a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fae0a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fae0a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fae0a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fae0a-136">Java</span><span class="sxs-lookup"><span data-stu-id="fae0a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fae0a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fae0a-137">Response</span></span>

<span data-ttu-id="fae0a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fae0a-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete reviewSetQuery",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


