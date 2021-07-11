---
title: Obter connectionOperation
description: Recupere as propriedades de uma connectionOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f709d05f1b93b3443dffc5171da6deb39dadc187
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366573"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="19e64-103">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="19e64-103">Get connectionOperation</span></span>

<span data-ttu-id="19e64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19e64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e64-105">Recupere as propriedades de [uma connectionOperation](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="19e64-105">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="19e64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="19e64-106">Permissions</span></span>

<span data-ttu-id="19e64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19e64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19e64-109">Permission type</span></span>                        | <span data-ttu-id="19e64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19e64-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19e64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19e64-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19e64-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19e64-112">Not supported.</span></span> |
| <span data-ttu-id="19e64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19e64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19e64-114">Not supported.</span></span> |
| <span data-ttu-id="19e64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19e64-115">Application</span></span>                            | <span data-ttu-id="19e64-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19e64-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19e64-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19e64-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="19e64-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19e64-118">Request headers</span></span>

| <span data-ttu-id="19e64-119">Nome</span><span class="sxs-lookup"><span data-stu-id="19e64-119">Name</span></span>          | <span data-ttu-id="19e64-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="19e64-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="19e64-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="19e64-121">Authorization</span></span> | <span data-ttu-id="19e64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19e64-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19e64-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19e64-124">Request body</span></span>

<span data-ttu-id="19e64-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19e64-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19e64-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="19e64-126">Response</span></span>

<span data-ttu-id="19e64-127">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [connectionOperation](../resources/connectionoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19e64-127">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="19e64-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="19e64-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="19e64-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19e64-129">Request</span></span>

<span data-ttu-id="19e64-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19e64-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="19e64-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e64-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="c"></a>[<span data-ttu-id="19e64-132">C#</span><span class="sxs-lookup"><span data-stu-id="19e64-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19e64-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19e64-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19e64-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19e64-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="19e64-135">Java</span><span class="sxs-lookup"><span data-stu-id="19e64-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectionoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="19e64-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="19e64-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="19e64-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19e64-137">The following is an example of the response.</span></span>

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


