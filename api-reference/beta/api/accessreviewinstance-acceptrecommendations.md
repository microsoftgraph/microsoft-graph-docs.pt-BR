---
title: 'accessReviewInstance: acceptRecommendations'
description: 'Permite a aceitação de recomendações em todas as decisões não revisadas em uma instância de revisão de acesso em que elas são revisadas. '
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2e9505a0cf7e3b0e52d54c45ed7d85ee4e09651e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048432"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="2ae75-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="2ae75-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="2ae75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ae75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ae75-105">Permite a aceitação de recomendações em todos os [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) não revisados em um [accessReviewInstance](../resources/accessreviewinstance.md) em que eles são os revisores.</span><span class="sxs-lookup"><span data-stu-id="2ae75-105">Allows the acceptance of recommendations on all not reviewed [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) on an [accessReviewInstance](../resources/accessreviewinstance.md) that they are the reviewer on.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ae75-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ae75-106">Permissions</span></span>
<span data-ttu-id="2ae75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ae75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ae75-109">Permission type</span></span>                        | <span data-ttu-id="2ae75-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ae75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ae75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ae75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ae75-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ae75-112">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="2ae75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ae75-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="2ae75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ae75-114">Not supported.</span></span> |

<span data-ttu-id="2ae75-115">O usuário de entrada também deve ser um revisor no accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="2ae75-115">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="2ae75-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ae75-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="2ae75-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae75-117">Request headers</span></span>
<span data-ttu-id="2ae75-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ae75-118">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="2ae75-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae75-119">Request body</span></span>
<span data-ttu-id="2ae75-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ae75-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ae75-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae75-121">Response</span></span>
<span data-ttu-id="2ae75-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ae75-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ae75-124">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ae75-124">Examples</span></span>
### <a name="request"></a><span data-ttu-id="2ae75-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ae75-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ae75-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ae75-126">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="2ae75-127">C#</span><span class="sxs-lookup"><span data-stu-id="2ae75-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ae75-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ae75-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ae75-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ae75-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ae75-130">Java</span><span class="sxs-lookup"><span data-stu-id="2ae75-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ae75-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ae75-131">Response</span></span>
><span data-ttu-id="2ae75-132">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ae75-132">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Accept recommendations accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
