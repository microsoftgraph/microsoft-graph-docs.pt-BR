---
title: Excluir externalConnection
description: Excluir um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 1b3e795c51f6ded27bb9f63706939c5a5ff1fa8b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965660"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="1dd1b-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="1dd1b-103">Delete externalConnection</span></span>

<span data-ttu-id="1dd1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dd1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd1b-105">Excluir um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="1dd1b-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="1dd1b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dd1b-106">Permissions</span></span>

<span data-ttu-id="1dd1b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dd1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1dd1b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dd1b-109">Permission type</span></span>                        | <span data-ttu-id="1dd1b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dd1b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1dd1b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dd1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1dd1b-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-112">Not supported.</span></span> |
| <span data-ttu-id="1dd1b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dd1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dd1b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-114">Not supported.</span></span> |
| <span data-ttu-id="1dd1b-115">Application</span><span class="sxs-lookup"><span data-stu-id="1dd1b-115">Application</span></span>                            | <span data-ttu-id="1dd1b-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dd1b-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dd1b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd1b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1dd1b-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd1b-118">Request headers</span></span>

| <span data-ttu-id="1dd1b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1dd1b-119">Name</span></span>          | <span data-ttu-id="1dd1b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dd1b-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1dd1b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dd1b-121">Authorization</span></span> | <span data-ttu-id="1dd1b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dd1b-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd1b-124">Request body</span></span>

<span data-ttu-id="1dd1b-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dd1b-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd1b-126">Response</span></span>

<span data-ttu-id="1dd1b-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1dd1b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1dd1b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1dd1b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dd1b-130">Request</span></span>

<span data-ttu-id="1dd1b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1dd1b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dd1b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="1dd1b-133">C#</span><span class="sxs-lookup"><span data-stu-id="1dd1b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dd1b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dd1b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dd1b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dd1b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dd1b-136">Java</span><span class="sxs-lookup"><span data-stu-id="1dd1b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="1dd1b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dd1b-137">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="1dd1b-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1dd1b-138">The following is an example of the response.</span></span>

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
  "description": "Delete externalConnection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


