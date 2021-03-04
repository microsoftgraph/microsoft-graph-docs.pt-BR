---
title: Excluir caso
description: Excluir um objeto case.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7c6958312795b304896904585ff0d5d66a74960a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445848"
---
# <a name="delete-case"></a><span data-ttu-id="b8834-103">Excluir caso</span><span class="sxs-lookup"><span data-stu-id="b8834-103">Delete case</span></span>

<span data-ttu-id="b8834-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b8834-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8834-105">Excluir um [objeto case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="b8834-105">Delete a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8834-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8834-106">Permissions</span></span>

<span data-ttu-id="b8834-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8834-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8834-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8834-109">Permission type</span></span>|<span data-ttu-id="b8834-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8834-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8834-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8834-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b8834-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8834-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="b8834-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8834-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8834-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8834-114">Not supported.</span></span>|
|<span data-ttu-id="b8834-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8834-115">Application</span></span>|<span data-ttu-id="b8834-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8834-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8834-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8834-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b8834-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8834-118">Request headers</span></span>

| <span data-ttu-id="b8834-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b8834-119">Name</span></span>          | <span data-ttu-id="b8834-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8834-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b8834-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8834-121">Authorization</span></span> | <span data-ttu-id="b8834-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8834-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8834-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8834-124">Request body</span></span>

<span data-ttu-id="b8834-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8834-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8834-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8834-126">Response</span></span>

<span data-ttu-id="b8834-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8834-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b8834-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b8834-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b8834-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8834-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b8834-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8834-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_case"
}-->

```http
DELETE https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
```

# <a name="c"></a>[<span data-ttu-id="b8834-131">C#</span><span class="sxs-lookup"><span data-stu-id="b8834-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8834-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8834-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8834-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8834-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8834-134">Java</span><span class="sxs-lookup"><span data-stu-id="b8834-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="b8834-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8834-135">Response</span></span>

<span data-ttu-id="b8834-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8834-136">The following is an example of the response.</span></span>

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
  "description": "Delete case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
