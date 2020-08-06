---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f56b02963a6d2d9aa1f2ee5c11776ef3c172c735
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566123"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="1a73e-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="1a73e-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="1a73e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a73e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a73e-105">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1a73e-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a73e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a73e-106">Permissions</span></span>

<span data-ttu-id="1a73e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a73e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a73e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a73e-109">Permission type</span></span>                        | <span data-ttu-id="1a73e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a73e-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
| <span data-ttu-id="1a73e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a73e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a73e-112">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="1a73e-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="1a73e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a73e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a73e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a73e-114">Not supported.</span></span> |
| <span data-ttu-id="1a73e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a73e-115">Application</span></span>                            | <span data-ttu-id="1a73e-116">Policy. Read. All e Policy. ReadWrite. ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="1a73e-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a73e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a73e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1a73e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a73e-118">Request headers</span></span>

| <span data-ttu-id="1a73e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1a73e-119">Name</span></span>          | <span data-ttu-id="1a73e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a73e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1a73e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a73e-121">Authorization</span></span> | <span data-ttu-id="1a73e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a73e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a73e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a73e-124">Request body</span></span>

<span data-ttu-id="1a73e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a73e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a73e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a73e-126">Response</span></span>

<span data-ttu-id="1a73e-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a73e-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a73e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a73e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a73e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a73e-130">Request</span></span>

<span data-ttu-id="1a73e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a73e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a73e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a73e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/identity/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="1a73e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1a73e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a73e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a73e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a73e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a73e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a73e-136">Java</span><span class="sxs-lookup"><span data-stu-id="1a73e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-conditionalaccesspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="1a73e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a73e-137">Response</span></span>

<span data-ttu-id="1a73e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a73e-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conditionalAccessPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
