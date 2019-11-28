---
title: Excluir externalItem
description: Exclua um externalItem ou externalfile.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 34a34c3913ccf4da490a79b2449e06ff45fc8512
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636810"
---
# <a name="delete-externalitem"></a><span data-ttu-id="72c1c-103">Excluir externalItem</span><span class="sxs-lookup"><span data-stu-id="72c1c-103">Delete externalItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c1c-104">Exclua um [externalitem](../resources/externalitem.md) ou [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="72c1c-104">Delete an [externalitem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="72c1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72c1c-105">Permissions</span></span>

<span data-ttu-id="72c1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72c1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72c1c-108">Permission type</span></span>                        | <span data-ttu-id="72c1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72c1c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72c1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72c1c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72c1c-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72c1c-111">Not supported.</span></span> |
| <span data-ttu-id="72c1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72c1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72c1c-113">Not supported.</span></span> |
| <span data-ttu-id="72c1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72c1c-114">Application</span></span>                            | <span data-ttu-id="72c1c-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72c1c-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="72c1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72c1c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="72c1c-117">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="72c1c-117">Path parameters</span></span>

| <span data-ttu-id="72c1c-118">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="72c1c-118">Parameter</span></span>     | <span data-ttu-id="72c1c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="72c1c-119">Type</span></span>   | <span data-ttu-id="72c1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="72c1c-120">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="72c1c-121">ID de conexão</span><span class="sxs-lookup"><span data-stu-id="72c1c-121">connection-id</span></span> | <span data-ttu-id="72c1c-122">string</span><span class="sxs-lookup"><span data-stu-id="72c1c-122">string</span></span> | <span data-ttu-id="72c1c-123">A `id` Propriedade do [externalConnection](../resources/externalconnection.md) que contém</span><span class="sxs-lookup"><span data-stu-id="72c1c-123">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="72c1c-124">item-id</span><span class="sxs-lookup"><span data-stu-id="72c1c-124">item-id</span></span>       | <span data-ttu-id="72c1c-125">string</span><span class="sxs-lookup"><span data-stu-id="72c1c-125">string</span></span> | <span data-ttu-id="72c1c-126">A propriedade fornecida `id` pelo desenvolvedor do [externalItem](../resources/externalitem.md) ou do [externalfile](../resources/externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="72c1c-126">The developer-provided `id` property of the [externalItem](../resources/externalitem.md) or [externalFile](../resources/externalfile.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="72c1c-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72c1c-127">Request headers</span></span>

| <span data-ttu-id="72c1c-128">Nome</span><span class="sxs-lookup"><span data-stu-id="72c1c-128">Name</span></span>          | <span data-ttu-id="72c1c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="72c1c-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="72c1c-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="72c1c-130">Authorization</span></span> | <span data-ttu-id="72c1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72c1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72c1c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72c1c-133">Request body</span></span>

<span data-ttu-id="72c1c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72c1c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="72c1c-135">Response</span></span>

<span data-ttu-id="72c1c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72c1c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72c1c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72c1c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72c1c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72c1c-139">Request</span></span>

<span data-ttu-id="72c1c-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72c1c-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="72c1c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c1c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
PATCH https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72c1c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c1c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="72c1c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="72c1c-143">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="72c1c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72c1c-144">The following is an example of the response.</span></span>

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
