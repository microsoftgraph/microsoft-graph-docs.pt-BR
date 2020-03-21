---
title: Excluir externalItem
description: Excluir um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 263d04ed1b254a52d9eacab19997e40cdac4dc67
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892539"
---
# <a name="delete-externalitem"></a><span data-ttu-id="d4889-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="d4889-103">Delete externalItem</span></span>

<span data-ttu-id="d4889-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4889-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4889-105">Excluir um [externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d4889-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="d4889-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4889-106">Permissions</span></span>

<span data-ttu-id="d4889-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4889-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4889-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4889-109">Permission type</span></span>                        | <span data-ttu-id="d4889-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4889-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4889-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4889-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4889-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4889-112">Not supported.</span></span> |
| <span data-ttu-id="d4889-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4889-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4889-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4889-114">Not supported.</span></span> |
| <span data-ttu-id="d4889-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4889-115">Application</span></span>                            | <span data-ttu-id="d4889-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4889-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4889-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4889-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="d4889-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="d4889-118">Path parameters</span></span>

| <span data-ttu-id="d4889-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d4889-119">Parameter</span></span>     | <span data-ttu-id="d4889-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4889-120">Type</span></span>   | <span data-ttu-id="d4889-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4889-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="d4889-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="d4889-122">connection-id</span></span> | <span data-ttu-id="d4889-123">string</span><span class="sxs-lookup"><span data-stu-id="d4889-123">string</span></span> | <span data-ttu-id="d4889-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="d4889-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="d4889-125">item-id</span><span class="sxs-lookup"><span data-stu-id="d4889-125">item-id</span></span>       | <span data-ttu-id="d4889-126">string</span><span class="sxs-lookup"><span data-stu-id="d4889-126">string</span></span> | <span data-ttu-id="d4889-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="d4889-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="d4889-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4889-128">Request headers</span></span>

| <span data-ttu-id="d4889-129">Nome</span><span class="sxs-lookup"><span data-stu-id="d4889-129">Name</span></span>          | <span data-ttu-id="d4889-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4889-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="d4889-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4889-131">Authorization</span></span> | <span data-ttu-id="d4889-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4889-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4889-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4889-134">Request body</span></span>

<span data-ttu-id="d4889-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4889-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4889-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4889-136">Response</span></span>

<span data-ttu-id="d4889-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4889-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4889-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d4889-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4889-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4889-140">Request</span></span>

<span data-ttu-id="d4889-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4889-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4889-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4889-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="d4889-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4889-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="d4889-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4889-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="d4889-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4889-145">The following is an example of the response.</span></span>

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
