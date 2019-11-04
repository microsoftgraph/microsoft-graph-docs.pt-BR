---
title: Excluir trustFrameworkKeySet
description: Excluir um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ea8fcebe75e39397d62affc586a5db24cee7853
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938271"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="93775-103">Excluir trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="93775-103">Delete trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93775-104">Excluir um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="93775-104">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="93775-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="93775-105">Permissions</span></span>

<span data-ttu-id="93775-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93775-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93775-108">Permission type</span></span>                        | <span data-ttu-id="93775-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93775-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="93775-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93775-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="93775-111">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="93775-111">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="93775-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93775-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93775-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93775-113">Not supported.</span></span> |
| <span data-ttu-id="93775-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93775-114">Application</span></span>                            | <span data-ttu-id="93775-115">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="93775-115">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93775-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93775-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="93775-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93775-117">Request headers</span></span>

| <span data-ttu-id="93775-118">Nome</span><span class="sxs-lookup"><span data-stu-id="93775-118">Name</span></span>          | <span data-ttu-id="93775-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="93775-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="93775-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="93775-120">Authorization</span></span> | <span data-ttu-id="93775-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93775-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93775-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93775-123">Request body</span></span>

<span data-ttu-id="93775-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93775-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93775-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="93775-125">Response</span></span>

<span data-ttu-id="93775-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93775-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93775-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93775-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="93775-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93775-129">Request</span></span>

<span data-ttu-id="93775-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93775-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93775-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="93775-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93775-132">C#</span><span class="sxs-lookup"><span data-stu-id="93775-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93775-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93775-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93775-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93775-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="93775-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="93775-135">Response</span></span>

<span data-ttu-id="93775-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93775-136">The following is an example of the response.</span></span>

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
