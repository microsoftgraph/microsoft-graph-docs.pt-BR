---
title: Excluir externalConnection
description: Excluir um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 14bbecb760768a0b2af984b737aaa9e3f1a28e10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48006913"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="41092-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="41092-103">Delete externalConnection</span></span>

<span data-ttu-id="41092-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41092-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41092-105">Excluir um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="41092-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="41092-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="41092-106">Permissions</span></span>

<span data-ttu-id="41092-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41092-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41092-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41092-109">Permission type</span></span>                        | <span data-ttu-id="41092-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="41092-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41092-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41092-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="41092-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41092-112">Not supported.</span></span> |
| <span data-ttu-id="41092-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41092-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41092-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41092-114">Not supported.</span></span> |
| <span data-ttu-id="41092-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41092-115">Application</span></span>                            | <span data-ttu-id="41092-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41092-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41092-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41092-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="41092-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41092-118">Request headers</span></span>

| <span data-ttu-id="41092-119">Nome</span><span class="sxs-lookup"><span data-stu-id="41092-119">Name</span></span>          | <span data-ttu-id="41092-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="41092-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="41092-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="41092-121">Authorization</span></span> | <span data-ttu-id="41092-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41092-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41092-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41092-124">Request body</span></span>

<span data-ttu-id="41092-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41092-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41092-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="41092-126">Response</span></span>

<span data-ttu-id="41092-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41092-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41092-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="41092-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41092-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41092-130">Request</span></span>

<span data-ttu-id="41092-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="41092-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41092-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="41092-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="41092-133">C#</span><span class="sxs-lookup"><span data-stu-id="41092-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41092-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41092-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41092-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41092-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="41092-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="41092-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="41092-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="41092-137">The following is an example of the response.</span></span>

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


