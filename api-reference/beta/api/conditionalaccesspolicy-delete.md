---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bc4d00975fc92e9e561ebfaa1b403f351b0baf9d
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636768"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="56810-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="56810-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56810-104">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="56810-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="56810-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="56810-105">Permissions</span></span>

<span data-ttu-id="56810-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56810-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56810-108">Permission type</span></span>                        | <span data-ttu-id="56810-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56810-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="56810-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56810-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="56810-111">Policy.ReadWrite.ConditionalAccess</span><span class="sxs-lookup"><span data-stu-id="56810-111">Policy.ReadWrite.ConditionalAccess</span></span> |
|<span data-ttu-id="56810-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56810-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56810-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56810-113">Not supported.</span></span> |
|<span data-ttu-id="56810-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56810-114">Application</span></span>                            | <span data-ttu-id="56810-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56810-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56810-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56810-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56810-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56810-117">Request headers</span></span>

| <span data-ttu-id="56810-118">Nome</span><span class="sxs-lookup"><span data-stu-id="56810-118">Name</span></span>          | <span data-ttu-id="56810-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="56810-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="56810-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="56810-120">Authorization</span></span> | <span data-ttu-id="56810-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56810-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56810-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56810-123">Request body</span></span>

<span data-ttu-id="56810-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56810-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56810-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="56810-125">Response</span></span>

<span data-ttu-id="56810-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56810-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="56810-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="56810-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="56810-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56810-129">Request</span></span>

<span data-ttu-id="56810-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56810-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56810-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="56810-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56810-132">C#</span><span class="sxs-lookup"><span data-stu-id="56810-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56810-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56810-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56810-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56810-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="56810-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="56810-135">Response</span></span>

<span data-ttu-id="56810-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56810-136">The following is an example of the response.</span></span>

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
