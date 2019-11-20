---
title: Excluir externalConnection
description: Excluir um externalConnection.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: cd3b6e70a5385ba0ad03e3fe79270dd6ad8a2804
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747199"
---
# <a name="delete-externalconnection"></a><span data-ttu-id="2c1f9-103">Excluir externalConnection</span><span class="sxs-lookup"><span data-stu-id="2c1f9-103">Delete externalConnection</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c1f9-104">Excluir um [externalConnection](../resources/externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="2c1f9-104">Delete an [externalConnection](../resources/externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="2c1f9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c1f9-105">Permissions</span></span>

<span data-ttu-id="2c1f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c1f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c1f9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c1f9-108">Permission type</span></span>                        | <span data-ttu-id="2c1f9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c1f9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c1f9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c1f9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c1f9-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-111">Not supported.</span></span> |
| <span data-ttu-id="2c1f9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c1f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c1f9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-113">Not supported.</span></span> |
| <span data-ttu-id="2c1f9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c1f9-114">Application</span></span>                            | <span data-ttu-id="2c1f9-115">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c1f9-115">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c1f9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1f9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2c1f9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c1f9-117">Request headers</span></span>

| <span data-ttu-id="2c1f9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2c1f9-118">Name</span></span>          | <span data-ttu-id="2c1f9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c1f9-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="2c1f9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c1f9-120">Authorization</span></span> | <span data-ttu-id="2c1f9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c1f9-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c1f9-123">Request body</span></span>

<span data-ttu-id="2c1f9-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c1f9-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c1f9-125">Response</span></span>

<span data-ttu-id="2c1f9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c1f9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c1f9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c1f9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c1f9-129">Request</span></span>

<span data-ttu-id="2c1f9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2c1f9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c1f9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connection"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c1f9-132">C#</span><span class="sxs-lookup"><span data-stu-id="2c1f9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c1f9-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c1f9-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c1f9-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c1f9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2c1f9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c1f9-135">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="2c1f9-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2c1f9-136">The following is an example of the response.</span></span>

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
