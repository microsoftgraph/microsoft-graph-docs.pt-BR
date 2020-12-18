---
title: Criar reviewSetQuery
description: Use esta API para criar um novo reviewSetQuery.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2635c446c6e0332df780c71be61232bb364ad683
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714099"
---
# <a name="create-reviewsetquery"></a><span data-ttu-id="b677d-103">Criar reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="b677d-103">Create reviewSetQuery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b677d-104">Criar um novo objeto [reviewSetQuery](../resources/reviewsetquery.md) .</span><span class="sxs-lookup"><span data-stu-id="b677d-104">Create a new [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b677d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b677d-105">Permissions</span></span>

<span data-ttu-id="b677d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b677d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b677d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b677d-108">Permission type</span></span>                        | <span data-ttu-id="b677d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b677d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b677d-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b677d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b677d-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="b677d-111">User.Read</span></span> |
| <span data-ttu-id="b677d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b677d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b677d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b677d-113">Not supported.</span></span> |
| <span data-ttu-id="b677d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b677d-114">Application</span></span>                            | <span data-ttu-id="b677d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b677d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b677d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b677d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases/{id}/reviewSets/{id}/queries
```

## <a name="request-headers"></a><span data-ttu-id="b677d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b677d-117">Request headers</span></span>

| <span data-ttu-id="b677d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b677d-118">Name</span></span>          | <span data-ttu-id="b677d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b677d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b677d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b677d-120">Authorization</span></span> | <span data-ttu-id="b677d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b677d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b677d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b677d-123">Request body</span></span>

<span data-ttu-id="b677d-124">No corpo da solicitação, forneça uma representação JSON do objeto [reviewSetQuery](../resources/reviewsetquery.md) .</span><span class="sxs-lookup"><span data-stu-id="b677d-124">In the request body, supply a JSON representation of [reviewSetQuery](../resources/reviewsetquery.md) object.</span></span> <span data-ttu-id="b677d-125">A tabela a seguir lista as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="b677d-125">The following table lists the required properties.</span></span>

| <span data-ttu-id="b677d-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b677d-126">Property</span></span>     | <span data-ttu-id="b677d-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="b677d-127">Type</span></span>        | <span data-ttu-id="b677d-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="b677d-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b677d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="b677d-129">displayName</span></span>  | <span data-ttu-id="b677d-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b677d-130">string</span></span>      | <span data-ttu-id="b677d-131">O nome da consulta do conjunto de revisão</span><span class="sxs-lookup"><span data-stu-id="b677d-131">The name of the review set query</span></span> |

## <a name="response"></a><span data-ttu-id="b677d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b677d-132">Response</span></span>

<span data-ttu-id="b677d-133">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [reviewSetQuery](../resources/reviewsetquery.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b677d-133">If successful, this method returns a `201 Created` response code and a new [reviewSetQuery](../resources/reviewsetquery.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b677d-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b677d-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b677d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b677d-135">Request</span></span>

<span data-ttu-id="b677d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b677d-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b677d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b677d-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b677d-138">C#</span><span class="sxs-lookup"><span data-stu-id="b677d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reviewsetquery-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b677d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b677d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reviewsetquery-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b677d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b677d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reviewsetquery-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b677d-141">Java</span><span class="sxs-lookup"><span data-stu-id="b677d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reviewsetquery-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b677d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="b677d-142">Response</span></span>

<span data-ttu-id="b677d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b677d-143">The following is an example of the response.</span></span>

> <span data-ttu-id="b677d-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b677d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reviewSetQuery"
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


