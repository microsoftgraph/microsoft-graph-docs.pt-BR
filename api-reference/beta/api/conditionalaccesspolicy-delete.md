---
title: Excluir conditionalAccessPolicy
description: Excluir um conditionalAccessPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b5a24f3e6fa7bc548c7d0d57f9a972701b00e69
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936759"
---
# <a name="delete-conditionalaccesspolicy"></a><span data-ttu-id="a12a3-103">Excluir conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="a12a3-103">Delete conditionalAccessPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12a3-104">Excluir um objeto [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="a12a3-104">Delete a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a12a3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a12a3-105">Permissions</span></span>

<span data-ttu-id="a12a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a12a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a12a3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a12a3-108">Permission type</span></span>                        | <span data-ttu-id="a12a3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a12a3-109">Permissions (from least to most privileged)</span></span>                    |
|:--------------------------------------|:---------------------------------------------------------------|
|<span data-ttu-id="a12a3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a12a3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a12a3-111">Policy. ReadWrite. ConditionalAccess e Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a12a3-111">Policy.ReadWrite.ConditionalAccess and Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a12a3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a12a3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12a3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a12a3-113">Not supported.</span></span> |
|<span data-ttu-id="a12a3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a12a3-114">Application</span></span>                            | <span data-ttu-id="a12a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a12a3-115">Not supported.</span></span> |

>[!NOTE]
><span data-ttu-id="a12a3-116">Essa API requer várias permissões.</span><span class="sxs-lookup"><span data-stu-id="a12a3-116">This API requires multiple permissions.</span></span> <span data-ttu-id="a12a3-117">Para obter detalhes, consulte [known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span><span class="sxs-lookup"><span data-stu-id="a12a3-117">For details, see [Known issues](/graph/known-issues#conditional-access-policies-and-named-locations).</span></span>

## <a name="http-request"></a><span data-ttu-id="a12a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a12a3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /conditionalAccess/policies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a12a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a12a3-119">Request headers</span></span>

| <span data-ttu-id="a12a3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a12a3-120">Name</span></span>          | <span data-ttu-id="a12a3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a12a3-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a12a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a12a3-122">Authorization</span></span> | <span data-ttu-id="a12a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a12a3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a12a3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a12a3-125">Request body</span></span>

<span data-ttu-id="a12a3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a12a3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a12a3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a12a3-127">Response</span></span>

<span data-ttu-id="a12a3-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a12a3-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a12a3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a12a3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a12a3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a12a3-131">Request</span></span>

<span data-ttu-id="a12a3-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a12a3-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a12a3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a12a3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conditionalaccesspolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/conditionalAccess/policies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a12a3-134">C#</span><span class="sxs-lookup"><span data-stu-id="a12a3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conditionalaccesspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a12a3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a12a3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conditionalaccesspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a12a3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a12a3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conditionalaccesspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a12a3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a12a3-137">Response</span></span>

<span data-ttu-id="a12a3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a12a3-138">The following is an example of the response.</span></span>

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
