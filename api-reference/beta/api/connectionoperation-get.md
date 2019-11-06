---
title: Obter connectionOperation
description: Recupere as propriedades de um connectionOperation.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 570eb444d34b35a316d1093a523937d230d1ed40
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994806"
---
# <a name="get-connectionoperation"></a><span data-ttu-id="f617a-103">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="f617a-103">Get connectionOperation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f617a-104">Recupere as propriedades de um [connectionOperation](../resources/connectionoperation.md).</span><span class="sxs-lookup"><span data-stu-id="f617a-104">Retrieve the properties of a [connectionOperation](../resources/connectionoperation.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f617a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f617a-105">Permissions</span></span>

<span data-ttu-id="f617a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f617a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f617a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f617a-108">Permission type</span></span>                        | <span data-ttu-id="f617a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f617a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f617a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f617a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f617a-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f617a-111">Not supported.</span></span> |
| <span data-ttu-id="f617a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f617a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f617a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f617a-113">Not supported.</span></span> |
| <span data-ttu-id="f617a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f617a-114">Application</span></span>                            | <span data-ttu-id="f617a-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f617a-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f617a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f617a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /external/connections/{connection-id}/operations/{operation-id}
```

## <a name="request-headers"></a><span data-ttu-id="f617a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f617a-117">Request headers</span></span>

| <span data-ttu-id="f617a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f617a-118">Name</span></span>          | <span data-ttu-id="f617a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f617a-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f617a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f617a-120">Authorization</span></span> | <span data-ttu-id="f617a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f617a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f617a-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f617a-123">Request body</span></span>

<span data-ttu-id="f617a-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f617a-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f617a-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f617a-125">Response</span></span>

<span data-ttu-id="f617a-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [connectionOperation](../resources/connectionoperation.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f617a-126">If successful, this method returns a `200 OK` response code and the requested [connectionOperation](../resources/connectionoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f617a-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f617a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f617a-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f617a-128">Request</span></span>

<span data-ttu-id="f617a-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f617a-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f617a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f617a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectionoperation"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/connections/contosohr/operations/3ed1595a-4bae-43c2-acda-ef973e581323
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f617a-131">C#</span><span class="sxs-lookup"><span data-stu-id="f617a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectionoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f617a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f617a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectionoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f617a-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f617a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectionoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="f617a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f617a-134">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="f617a-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f617a-135">The following is an example of the response.</span></span>

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
