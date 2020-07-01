---
title: Excluir externalItem
description: Excluir um externalItem.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: be19c8ddb584ca17e6eac346996239a0c90c6738
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989986"
---
# <a name="delete-externalitem"></a><span data-ttu-id="4b416-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="4b416-103">Delete externalItem</span></span>

<span data-ttu-id="4b416-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b416-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b416-105">Excluir um [externalitem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="4b416-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="4b416-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b416-106">Permissions</span></span>

<span data-ttu-id="4b416-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4b416-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4b416-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b416-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b416-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b416-109">Permission type</span></span>                        | <span data-ttu-id="4b416-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b416-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b416-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b416-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b416-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b416-112">Not supported.</span></span> |
| <span data-ttu-id="4b416-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b416-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b416-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b416-114">Not supported.</span></span> |
| <span data-ttu-id="4b416-115">Application</span><span class="sxs-lookup"><span data-stu-id="4b416-115">Application</span></span>                            | <span data-ttu-id="4b416-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b416-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b416-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b416-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="4b416-118">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="4b416-118">Path parameters</span></span>

| <span data-ttu-id="4b416-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4b416-119">Parameter</span></span>     | <span data-ttu-id="4b416-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b416-120">Type</span></span>   | <span data-ttu-id="4b416-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b416-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="4b416-122">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="4b416-122">connection-id</span></span> | <span data-ttu-id="4b416-123">string</span><span class="sxs-lookup"><span data-stu-id="4b416-123">string</span></span> | <span data-ttu-id="4b416-124">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="4b416-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="4b416-125">item-id</span><span class="sxs-lookup"><span data-stu-id="4b416-125">item-id</span></span>       | <span data-ttu-id="4b416-126">string</span><span class="sxs-lookup"><span data-stu-id="4b416-126">string</span></span> | <span data-ttu-id="4b416-127">A propriedade fornecida pelo desenvolvedor `id` do [externalItem](../resources/externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="4b416-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="4b416-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-128">Request headers</span></span>

| <span data-ttu-id="4b416-129">Nome</span><span class="sxs-lookup"><span data-stu-id="4b416-129">Name</span></span>          | <span data-ttu-id="4b416-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b416-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4b416-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b416-131">Authorization</span></span> | <span data-ttu-id="4b416-132">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4b416-132">Bearer {token}.</span></span> <span data-ttu-id="4b416-133">Required.</span><span class="sxs-lookup"><span data-stu-id="4b416-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b416-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-134">Request body</span></span>

<span data-ttu-id="4b416-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b416-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b416-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b416-136">Response</span></span>

<span data-ttu-id="4b416-137">If successful, this method returns `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="4b416-137">If successful, this method returns `204 No Content` response code.</span></span> <span data-ttu-id="4b416-138">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="4b416-138">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b416-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4b416-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b416-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b416-140">Request</span></span>

<span data-ttu-id="4b416-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b416-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b416-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b416-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="4b416-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b416-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="4b416-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b416-144">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="4b416-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b416-145">The following is an example of the response.</span></span>

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
