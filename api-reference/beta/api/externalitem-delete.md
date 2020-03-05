---
title: Excluir externalItem
description: Exclua um externalItem ou externalfile.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 6d5cf833b6f91a76c8fee63c81bd6dd6db32d548
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42422009"
---
# <a name="delete-externalitem"></a><span data-ttu-id="ce70e-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="ce70e-103">Delete externalItem</span></span>

<span data-ttu-id="ce70e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce70e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce70e-105">Exclua um [externalitem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="ce70e-105">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="ce70e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce70e-106">Permissions</span></span>

<span data-ttu-id="ce70e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce70e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce70e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce70e-109">Permission type</span></span>                        | <span data-ttu-id="ce70e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce70e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce70e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce70e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce70e-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce70e-112">Not supported.</span></span> |
| <span data-ttu-id="ce70e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce70e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce70e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce70e-114">Not supported.</span></span> |
| <span data-ttu-id="ce70e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce70e-115">Application</span></span>                            | <span data-ttu-id="ce70e-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce70e-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce70e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce70e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="ce70e-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="ce70e-118">Path parameters</span></span>

| <span data-ttu-id="ce70e-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ce70e-119">Parameter</span></span>     | <span data-ttu-id="ce70e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce70e-120">Type</span></span>   | <span data-ttu-id="ce70e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce70e-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="ce70e-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="ce70e-122">connection-id</span></span> | <span data-ttu-id="ce70e-123">string</span><span class="sxs-lookup"><span data-stu-id="ce70e-123">string</span></span> | <span data-ttu-id="ce70e-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="ce70e-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="ce70e-125">item-id</span><span class="sxs-lookup"><span data-stu-id="ce70e-125">item-id</span></span>       | <span data-ttu-id="ce70e-126">string</span><span class="sxs-lookup"><span data-stu-id="ce70e-126">string</span></span> | <span data-ttu-id="ce70e-127">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="ce70e-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="ce70e-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce70e-128">Request headers</span></span>

| <span data-ttu-id="ce70e-129">Nome</span><span class="sxs-lookup"><span data-stu-id="ce70e-129">Name</span></span>          | <span data-ttu-id="ce70e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce70e-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="ce70e-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce70e-131">Authorization</span></span> | <span data-ttu-id="ce70e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce70e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce70e-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce70e-134">Request body</span></span>

<span data-ttu-id="ce70e-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce70e-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce70e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce70e-136">Response</span></span>

<span data-ttu-id="ce70e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce70e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce70e-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce70e-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce70e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce70e-140">Request</span></span>

<span data-ttu-id="ce70e-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce70e-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce70e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce70e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="ce70e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce70e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="ce70e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce70e-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="ce70e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce70e-145">The following is an example of the response.</span></span>

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
