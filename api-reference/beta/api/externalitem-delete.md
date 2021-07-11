---
title: Excluir externalItem
description: Exclua um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 2506d03831637d27ebe3b874361f650e843f1cf4
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366792"
---
# <a name="delete-externalitem"></a><span data-ttu-id="dcd02-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="dcd02-103">Delete externalItem</span></span>

<span data-ttu-id="dcd02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcd02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcd02-105">Excluir [um externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="dcd02-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd02-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcd02-106">Permissions</span></span>

<span data-ttu-id="dcd02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcd02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcd02-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcd02-109">Permission type</span></span>                        | <span data-ttu-id="dcd02-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcd02-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcd02-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcd02-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcd02-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcd02-112">Not supported.</span></span> |
| <span data-ttu-id="dcd02-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcd02-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd02-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcd02-114">Not supported.</span></span> |
| <span data-ttu-id="dcd02-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcd02-115">Application</span></span>                            | <span data-ttu-id="dcd02-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcd02-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcd02-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd02-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="dcd02-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="dcd02-118">Path parameters</span></span>

| <span data-ttu-id="dcd02-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="dcd02-119">Parameter</span></span>     | <span data-ttu-id="dcd02-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcd02-120">Type</span></span>   | <span data-ttu-id="dcd02-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd02-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="dcd02-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="dcd02-122">connection-id</span></span> | <span data-ttu-id="dcd02-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcd02-123">string</span></span> | <span data-ttu-id="dcd02-124">A `id` propriedade do [externalConnection que](../resources/externalconnection.md) contém</span><span class="sxs-lookup"><span data-stu-id="dcd02-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="dcd02-125">item-id</span><span class="sxs-lookup"><span data-stu-id="dcd02-125">item-id</span></span>       | <span data-ttu-id="dcd02-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dcd02-126">string</span></span> | <span data-ttu-id="dcd02-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="dcd02-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="dcd02-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd02-128">Request headers</span></span>

| <span data-ttu-id="dcd02-129">Nome</span><span class="sxs-lookup"><span data-stu-id="dcd02-129">Name</span></span>          | <span data-ttu-id="dcd02-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd02-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dcd02-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcd02-131">Authorization</span></span> | <span data-ttu-id="dcd02-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcd02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcd02-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd02-134">Request body</span></span>

<span data-ttu-id="dcd02-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcd02-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcd02-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd02-136">Response</span></span>

<span data-ttu-id="dcd02-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd02-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcd02-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcd02-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcd02-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd02-140">Request</span></span>

<span data-ttu-id="dcd02-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcd02-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcd02-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd02-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="dcd02-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcd02-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dcd02-144">C#</span><span class="sxs-lookup"><span data-stu-id="dcd02-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcd02-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcd02-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcd02-146">Java</span><span class="sxs-lookup"><span data-stu-id="dcd02-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="dcd02-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd02-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="dcd02-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd02-148">The following is an example of the response.</span></span>

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


