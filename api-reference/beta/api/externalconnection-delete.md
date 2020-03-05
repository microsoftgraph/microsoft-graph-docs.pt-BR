---
title: Excluir externalConnection
description: Excluir um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 809175827de2347d473607fa701647d0db5c9c4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422289"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="e3f47-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="e3f47-103">Delete externalConnection</span></span>

<span data-ttu-id="e3f47-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e3f47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3f47-105">Excluir um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="e3f47-105">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="e3f47-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3f47-106">Permissions</span></span>

<span data-ttu-id="e3f47-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3f47-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3f47-109">Permission type</span></span>                        | <span data-ttu-id="e3f47-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3f47-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3f47-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3f47-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3f47-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3f47-112">Not supported.</span></span> |
| <span data-ttu-id="e3f47-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3f47-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3f47-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3f47-114">Not supported.</span></span> |
| <span data-ttu-id="e3f47-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3f47-115">Application</span></span>                            | <span data-ttu-id="e3f47-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3f47-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3f47-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f47-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e3f47-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f47-118">Request headers</span></span>

| <span data-ttu-id="e3f47-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e3f47-119">Name</span></span>          | <span data-ttu-id="e3f47-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3f47-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e3f47-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3f47-121">Authorization</span></span> | <span data-ttu-id="e3f47-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3f47-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3f47-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f47-124">Request body</span></span>

<span data-ttu-id="e3f47-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3f47-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3f47-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f47-126">Response</span></span>

<span data-ttu-id="e3f47-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f47-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3f47-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3f47-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3f47-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3f47-130">Request</span></span>

<span data-ttu-id="e3f47-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3f47-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e3f47-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e3f47-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="c"></a>[<span data-ttu-id="e3f47-133">C#</span><span class="sxs-lookup"><span data-stu-id="e3f47-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e3f47-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e3f47-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e3f47-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e3f47-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="e3f47-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3f47-136">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="e3f47-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3f47-137">The following is an example of the response.</span></span>

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
