---
title: Obter connectionOperation
description: Recupere as propriedades de um connectionOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 24d6b25675ae440562a8376da66af371fed4b00b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002958"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="87acb-103">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="87acb-103">Get connectionOperation</span></span>

<span data-ttu-id="87acb-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="87acb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87acb-105">Recupere as propriedades de um [connectionOperation](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="87acb-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="87acb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87acb-106">Permissions</span></span>

<span data-ttu-id="87acb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87acb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87acb-109">Permission type</span></span>                        | <span data-ttu-id="87acb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87acb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87acb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87acb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87acb-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87acb-112">Not supported.</span></span> |
| <span data-ttu-id="87acb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87acb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87acb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87acb-114">Not supported.</span></span> |
| <span data-ttu-id="87acb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87acb-115">Application</span></span>                            | <span data-ttu-id="87acb-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87acb-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87acb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87acb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="87acb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87acb-118">Request headers</span></span>

| <span data-ttu-id="87acb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="87acb-119">Name</span></span>          | <span data-ttu-id="87acb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87acb-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="87acb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87acb-121">Authorization</span></span> | <span data-ttu-id="87acb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87acb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87acb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87acb-124">Request body</span></span>

<span data-ttu-id="87acb-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87acb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87acb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="87acb-126">Response</span></span>

<span data-ttu-id="87acb-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [connectionOperation](../resources/connectionoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87acb-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87acb-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87acb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87acb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87acb-129">Request</span></span>

<span data-ttu-id="87acb-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87acb-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87acb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="87acb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="87acb-132">C#</span><span class="sxs-lookup"><span data-stu-id="87acb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87acb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87acb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87acb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87acb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="87acb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87acb-135">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="87acb-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87acb-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "expectError": true,
  "@odata.type": "microsoft.graph.connectionOperation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "3ed1595a-4bae-43c2-acda-ef973e581323",
  "status": "failed",
  "error": {
    "message": "Server error, something went wrong"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectionOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


