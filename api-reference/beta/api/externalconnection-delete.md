---
title: Excluir externalConnection
description: Excluir um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: ab69d1c90b0f3e0767c339dd1d0e4b44020ce4b0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869775"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="76460-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="76460-103">Delete externalConnection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76460-104">Excluir um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="76460-104">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="76460-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="76460-105">Permissions</span></span>

<span data-ttu-id="76460-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76460-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76460-108">Permission type</span></span>                        | <span data-ttu-id="76460-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="76460-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76460-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76460-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="76460-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76460-111">Not supported.</span></span> |
| <span data-ttu-id="76460-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76460-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76460-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76460-113">Not supported.</span></span> |
| <span data-ttu-id="76460-114">Application</span><span class="sxs-lookup"><span data-stu-id="76460-114">Application</span></span>                            | <span data-ttu-id="76460-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76460-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76460-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76460-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76460-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76460-117">Request headers</span></span>

| <span data-ttu-id="76460-118">Nome</span><span class="sxs-lookup"><span data-stu-id="76460-118">Name</span></span>          | <span data-ttu-id="76460-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="76460-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="76460-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="76460-120">Authorization</span></span> | <span data-ttu-id="76460-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76460-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76460-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76460-123">Request body</span></span>

<span data-ttu-id="76460-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="76460-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76460-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="76460-125">Response</span></span>

<span data-ttu-id="76460-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76460-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76460-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="76460-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76460-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76460-129">Request</span></span>

<span data-ttu-id="76460-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="76460-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76460-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="76460-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76460-132">C#</span><span class="sxs-lookup"><span data-stu-id="76460-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76460-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76460-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76460-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76460-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="76460-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="76460-135">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="76460-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="76460-136">The following is an example of the response.</span></span>

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
