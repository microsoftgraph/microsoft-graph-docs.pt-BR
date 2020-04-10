---
title: Excluir trustFrameworkKeySet
description: Excluir um objeto **trustFrameworkKeySet** .
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9280371537ebd82452a22910d4729dc5b9b5bab
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43215928"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="256a1-103">Excluir trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="256a1-103">Delete trustFrameworkKeySet</span></span>

<span data-ttu-id="256a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="256a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="256a1-105">Excluir um [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span><span class="sxs-lookup"><span data-stu-id="256a1-105">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="256a1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="256a1-106">Permissions</span></span>

<span data-ttu-id="256a1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="256a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="256a1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="256a1-109">Permission type</span></span>                        | <span data-ttu-id="256a1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="256a1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="256a1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="256a1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="256a1-112">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="256a1-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="256a1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="256a1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="256a1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="256a1-114">Not supported.</span></span> |
| <span data-ttu-id="256a1-115">Application</span><span class="sxs-lookup"><span data-stu-id="256a1-115">Application</span></span>                            | <span data-ttu-id="256a1-116">TrustFrameworkKeySet. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="256a1-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="256a1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="256a1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="256a1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="256a1-118">Request headers</span></span>

| <span data-ttu-id="256a1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="256a1-119">Name</span></span>          | <span data-ttu-id="256a1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="256a1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="256a1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="256a1-121">Authorization</span></span> | <span data-ttu-id="256a1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="256a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="256a1-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="256a1-124">Request body</span></span>

<span data-ttu-id="256a1-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="256a1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="256a1-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="256a1-126">Response</span></span>

<span data-ttu-id="256a1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="256a1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="256a1-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="256a1-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="256a1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="256a1-130">Request</span></span>

<span data-ttu-id="256a1-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="256a1-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="256a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="256a1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="256a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="256a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="256a1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="256a1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="256a1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="256a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="256a1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="256a1-136">Response</span></span>

<span data-ttu-id="256a1-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="256a1-137">The following is an example of the response.</span></span>

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
