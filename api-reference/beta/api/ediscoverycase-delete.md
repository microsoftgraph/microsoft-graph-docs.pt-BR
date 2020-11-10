---
title: Excluir ediscoveryCase
description: Excluir um objeto ediscoveryCase.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 836e510906e0e35ce1a1be4b8a6556d0467e9e10
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966773"
---
# <a name="delete-ediscoverycase"></a><span data-ttu-id="46fd7-103">Excluir ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="46fd7-103">Delete ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46fd7-104">Excluir um objeto [ediscoveryCase](../resources/ediscoverycase.md) .</span><span class="sxs-lookup"><span data-stu-id="46fd7-104">Delete an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46fd7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46fd7-105">Permissions</span></span>

<span data-ttu-id="46fd7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46fd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46fd7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46fd7-108">Permission type</span></span>                        | <span data-ttu-id="46fd7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46fd7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46fd7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46fd7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="46fd7-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="46fd7-111">User.Read</span></span>      |
| <span data-ttu-id="46fd7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46fd7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46fd7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46fd7-113">Not supported.</span></span> |
| <span data-ttu-id="46fd7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46fd7-114">Application</span></span>                            | <span data-ttu-id="46fd7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46fd7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46fd7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46fd7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="46fd7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46fd7-117">Request headers</span></span>

| <span data-ttu-id="46fd7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46fd7-118">Name</span></span>          | <span data-ttu-id="46fd7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46fd7-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="46fd7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="46fd7-120">Authorization</span></span> | <span data-ttu-id="46fd7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46fd7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46fd7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46fd7-123">Request body</span></span>

<span data-ttu-id="46fd7-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46fd7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46fd7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="46fd7-125">Response</span></span>

<span data-ttu-id="46fd7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46fd7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46fd7-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46fd7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46fd7-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46fd7-129">Request</span></span>

<span data-ttu-id="46fd7-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46fd7-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="46fd7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="46fd7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_ediscoverycase"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```
# <a name="c"></a>[<span data-ttu-id="46fd7-132">C#</span><span class="sxs-lookup"><span data-stu-id="46fd7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46fd7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46fd7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46fd7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46fd7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46fd7-135">Java</span><span class="sxs-lookup"><span data-stu-id="46fd7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46fd7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="46fd7-136">Response</span></span>

<span data-ttu-id="46fd7-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46fd7-137">The following is an example of the response.</span></span>

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
  "description": "Delete ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


