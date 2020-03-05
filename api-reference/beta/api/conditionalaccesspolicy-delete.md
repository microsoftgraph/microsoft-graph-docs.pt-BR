---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9738dd411b2174d42951335ce3b20c7a16e6bbe6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438019"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="48f39-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="48f39-103">Delete conditionalAccessPolicy</span></span>

<span data-ttu-id="48f39-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="48f39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48f39-105">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="48f39-105">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48f39-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="48f39-106">Permissions</span></span>

<span data-ttu-id="48f39-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48f39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48f39-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="48f39-109">Permission type</span></span>                        | <span data-ttu-id="48f39-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="48f39-110">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="48f39-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="48f39-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48f39-112">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="48f39-112">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="48f39-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="48f39-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48f39-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f39-114">Not supported.</span></span> |
|<span data-ttu-id="48f39-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="48f39-115">Application</span></span>                            | <span data-ttu-id="48f39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="48f39-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48f39-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="48f39-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="48f39-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="48f39-118">Request headers</span></span>

| <span data-ttu-id="48f39-119">Nome</span><span class="sxs-lookup"><span data-stu-id="48f39-119">Name</span></span>          | <span data-ttu-id="48f39-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f39-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48f39-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="48f39-121">Authorization</span></span> | <span data-ttu-id="48f39-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="48f39-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="48f39-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="48f39-124">Request body</span></span>

<span data-ttu-id="48f39-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="48f39-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48f39-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f39-126">Response</span></span>

<span data-ttu-id="48f39-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="48f39-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48f39-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="48f39-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48f39-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="48f39-130">Request</span></span>

<span data-ttu-id="48f39-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="48f39-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48f39-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="48f39-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="c"></a>[<span data-ttu-id="48f39-133">C#</span><span class="sxs-lookup"><span data-stu-id="48f39-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="48f39-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48f39-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48f39-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48f39-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="48f39-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="48f39-136">Response</span></span>

<span data-ttu-id="48f39-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="48f39-137">The following is an example of the response.</span></span>

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
