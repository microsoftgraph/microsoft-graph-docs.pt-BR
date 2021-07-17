---
title: Excluir externalItem
description: Exclua um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 26b556a71f6eda6ee2860fc897eb14d58ae9a249
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466969"
---
# <a name="delete-externalitem"></a><span data-ttu-id="ce24c-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="ce24c-103">Delete externalItem</span></span>

<span data-ttu-id="ce24c-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="ce24c-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce24c-105">Excluir [um externalitem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="ce24c-105">Delete an [externalitem](../resources/externalconnectors-externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce24c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce24c-106">Permissions</span></span>

<span data-ttu-id="ce24c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce24c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce24c-109">Permission type</span></span>                        | <span data-ttu-id="ce24c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce24c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce24c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce24c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce24c-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce24c-112">Not supported.</span></span> |
| <span data-ttu-id="ce24c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce24c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce24c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce24c-114">Not supported.</span></span> |
| <span data-ttu-id="ce24c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce24c-115">Application</span></span>                            | <span data-ttu-id="ce24c-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce24c-116">ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce24c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce24c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="ce24c-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="ce24c-118">Path parameters</span></span>

| <span data-ttu-id="ce24c-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce24c-119">Parameter</span></span>     | <span data-ttu-id="ce24c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce24c-120">Type</span></span>   | <span data-ttu-id="ce24c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce24c-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="ce24c-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="ce24c-122">connection-id</span></span> | <span data-ttu-id="ce24c-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce24c-123">string</span></span> | <span data-ttu-id="ce24c-124">A `id` propriedade do [externalConnection que](../resources/externalconnectors-externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="ce24c-124">The `id` property of the containing [externalConnection](../resources/externalconnectors-externalconnection.md)</span></span> |
| <span data-ttu-id="ce24c-125">item-id</span><span class="sxs-lookup"><span data-stu-id="ce24c-125">item-id</span></span>       | <span data-ttu-id="ce24c-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce24c-126">string</span></span> | <span data-ttu-id="ce24c-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalconnectors-externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="ce24c-127">The developer-provided `id` property of the [externalItem](../resources/externalconnectors-externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ce24c-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24c-128">Request headers</span></span>

| <span data-ttu-id="ce24c-129">Nome</span><span class="sxs-lookup"><span data-stu-id="ce24c-129">Name</span></span>          | <span data-ttu-id="ce24c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce24c-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ce24c-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce24c-131">Authorization</span></span> | <span data-ttu-id="ce24c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce24c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce24c-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24c-134">Request body</span></span>

<span data-ttu-id="ce24c-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce24c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce24c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce24c-136">Response</span></span>

<span data-ttu-id="ce24c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce24c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce24c-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce24c-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce24c-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce24c-140">Request</span></span>

<span data-ttu-id="ce24c-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce24c-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce24c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce24c-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="ce24c-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce24c-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ce24c-144">C#</span><span class="sxs-lookup"><span data-stu-id="ce24c-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce24c-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce24c-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce24c-146">Java</span><span class="sxs-lookup"><span data-stu-id="ce24c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ce24c-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce24c-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="ce24c-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce24c-148">The following is an example of the response.</span></span>

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


