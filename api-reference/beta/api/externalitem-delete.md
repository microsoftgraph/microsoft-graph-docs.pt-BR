---
title: Excluir externalItem
description: Excluir um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: f9abe39baa29ba247994d4ea6ff8c30bd7f28f72
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006766"
---
# <a name="delete-externalitem"></a><span data-ttu-id="d2304-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="d2304-103">Delete externalItem</span></span>

<span data-ttu-id="d2304-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2304-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2304-105">Excluir um [externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d2304-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d2304-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d2304-106">Permissions</span></span>

<span data-ttu-id="d2304-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d2304-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d2304-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2304-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d2304-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2304-109">Permission type</span></span>                        | <span data-ttu-id="d2304-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d2304-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d2304-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2304-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d2304-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2304-112">Not supported.</span></span> |
| <span data-ttu-id="d2304-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2304-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2304-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2304-114">Not supported.</span></span> |
| <span data-ttu-id="d2304-115">Application</span><span class="sxs-lookup"><span data-stu-id="d2304-115">Application</span></span>                            | <span data-ttu-id="d2304-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2304-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2304-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2304-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d2304-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d2304-118">Path parameters</span></span>

| <span data-ttu-id="d2304-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d2304-119">Parameter</span></span>     | <span data-ttu-id="d2304-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2304-120">Type</span></span>   | <span data-ttu-id="d2304-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2304-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d2304-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="d2304-122">connection-id</span></span> | <span data-ttu-id="d2304-123">string</span><span class="sxs-lookup"><span data-stu-id="d2304-123">string</span></span> | <span data-ttu-id="d2304-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="d2304-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="d2304-125">item-id</span><span class="sxs-lookup"><span data-stu-id="d2304-125">item-id</span></span>       | <span data-ttu-id="d2304-126">string</span><span class="sxs-lookup"><span data-stu-id="d2304-126">string</span></span> | <span data-ttu-id="d2304-127">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d2304-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d2304-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2304-128">Request headers</span></span>

| <span data-ttu-id="d2304-129">Nome</span><span class="sxs-lookup"><span data-stu-id="d2304-129">Name</span></span>          | <span data-ttu-id="d2304-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2304-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d2304-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2304-131">Authorization</span></span> | <span data-ttu-id="d2304-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="d2304-132">Bearer {token}.</span></span> <span data-ttu-id="d2304-133">Required.</span><span class="sxs-lookup"><span data-stu-id="d2304-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2304-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2304-134">Request body</span></span>

<span data-ttu-id="d2304-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d2304-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2304-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2304-136">Response</span></span>

<span data-ttu-id="d2304-137">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="d2304-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="d2304-138">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="d2304-138">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d2304-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d2304-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d2304-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2304-140">Request</span></span>

<span data-ttu-id="d2304-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2304-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d2304-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2304-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="d2304-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2304-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d2304-144">C#</span><span class="sxs-lookup"><span data-stu-id="d2304-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2304-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2304-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d2304-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2304-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d2304-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d2304-147">The following is an example of the response.</span></span>

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
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
