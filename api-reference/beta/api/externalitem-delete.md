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
# <a name="delete-externalitem"></a><span data-ttu-id="9b995-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="9b995-103">Delete externalItem</span></span>

<span data-ttu-id="9b995-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b995-105">Excluir um [externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b995-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="9b995-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9b995-106">Permissions</span></span>

<span data-ttu-id="9b995-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b995-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b995-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9b995-109">Permission type</span></span>                        | <span data-ttu-id="9b995-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9b995-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9b995-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9b995-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9b995-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b995-112">Not supported.</span></span> |
| <span data-ttu-id="9b995-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9b995-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9b995-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9b995-114">Not supported.</span></span> |
| <span data-ttu-id="9b995-115">Application</span><span class="sxs-lookup"><span data-stu-id="9b995-115">Application</span></span>                            | <span data-ttu-id="9b995-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b995-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9b995-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9b995-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="9b995-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="9b995-118">Path parameters</span></span>

| <span data-ttu-id="9b995-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9b995-119">Parameter</span></span>     | <span data-ttu-id="9b995-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b995-120">Type</span></span>   | <span data-ttu-id="9b995-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b995-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="9b995-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="9b995-122">connection-id</span></span> | <span data-ttu-id="9b995-123">string</span><span class="sxs-lookup"><span data-stu-id="9b995-123">string</span></span> | <span data-ttu-id="9b995-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="9b995-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="9b995-125">item-id</span><span class="sxs-lookup"><span data-stu-id="9b995-125">item-id</span></span>       | <span data-ttu-id="9b995-126">string</span><span class="sxs-lookup"><span data-stu-id="9b995-126">string</span></span> | <span data-ttu-id="9b995-127">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="9b995-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="9b995-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9b995-128">Request headers</span></span>

| <span data-ttu-id="9b995-129">Nome</span><span class="sxs-lookup"><span data-stu-id="9b995-129">Name</span></span>          | <span data-ttu-id="9b995-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b995-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9b995-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="9b995-131">Authorization</span></span> | <span data-ttu-id="9b995-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9b995-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b995-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9b995-134">Request body</span></span>

<span data-ttu-id="9b995-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9b995-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b995-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b995-136">Response</span></span>

<span data-ttu-id="9b995-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9b995-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9b995-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9b995-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9b995-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9b995-140">Request</span></span>

<span data-ttu-id="9b995-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9b995-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9b995-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b995-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="9b995-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b995-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9b995-144">C#</span><span class="sxs-lookup"><span data-stu-id="9b995-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b995-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b995-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="9b995-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9b995-146">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="9b995-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b995-147">The following is an example of the response.</span></span>

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
