---
title: Excluir trustFrameworkKeySet
description: Excluir um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69987f35f6b915e8b6a7bd3fa4dafe1b124e58a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027367"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="7a8a3-103">Excluir trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="7a8a3-103">Delete trustFrameworkKeySet</span></span>

<span data-ttu-id="7a8a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a8a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a8a3-105">Excluir um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="7a8a3-105">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a8a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a8a3-106">Permissions</span></span>

<span data-ttu-id="7a8a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a8a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a8a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a8a3-109">Permission type</span></span>                        | <span data-ttu-id="7a8a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a8a3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7a8a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a8a3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a8a3-112">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7a8a3-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="7a8a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a8a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a8a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-114">Not supported.</span></span> |
| <span data-ttu-id="7a8a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a8a3-115">Application</span></span>                            | <span data-ttu-id="7a8a3-116">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7a8a3-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a8a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a8a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7a8a3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a8a3-118">Request headers</span></span>

| <span data-ttu-id="7a8a3-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a8a3-119">Name</span></span>          | <span data-ttu-id="7a8a3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a8a3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7a8a3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a8a3-121">Authorization</span></span> | <span data-ttu-id="7a8a3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a8a3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a8a3-124">Request body</span></span>

<span data-ttu-id="7a8a3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a8a3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a8a3-126">Response</span></span>

<span data-ttu-id="7a8a3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7a8a3-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7a8a3-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7a8a3-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a8a3-130">Request</span></span>

<span data-ttu-id="7a8a3-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a8a3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a8a3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="7a8a3-133">C#</span><span class="sxs-lookup"><span data-stu-id="7a8a3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a8a3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a8a3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a8a3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a8a3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7a8a3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a8a3-136">Response</span></span>

<span data-ttu-id="7a8a3-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7a8a3-137">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


