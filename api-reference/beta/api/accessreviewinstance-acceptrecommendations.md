---
title: 'accessReviewInstance: acceptRecommendations'
description: 'Permite a aceitação de recomendações em todas as decisões que não foram revisadas para uma instância de revisão de acesso para a qual o usuário de chamada é um revistor. '
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b955bc637c3f536ca5cb8a3e24ad65990296ab2e
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030751"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="16728-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="16728-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="16728-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16728-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16728-105">Permite a aceitação de recomendações em todos os objetos [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) que não foram revisados para um [objeto accessReviewInstance](../resources/accessreviewinstance.md) para o qual o usuário de chamada é um revisor.</span><span class="sxs-lookup"><span data-stu-id="16728-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed for an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span> <span data-ttu-id="16728-106">Recomendações serão **gerados se recommendationsEnabled** estiver `true` no objeto [accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="16728-106">Recommendations are generated if **recommendationsEnabled** is `true` on the [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span> <span data-ttu-id="16728-107">Se não houver uma recomendação em [um objeto accessReviewInstanceDecisionItem,](../resources/accessreviewinstancedecisionitem.md) nenhuma decisão será registrada.</span><span class="sxs-lookup"><span data-stu-id="16728-107">If there is not a recommendation on an [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) object no decision will be recorded.</span></span>

## <a name="permissions"></a><span data-ttu-id="16728-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="16728-108">Permissions</span></span>
<span data-ttu-id="16728-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16728-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16728-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16728-111">Permission type</span></span>                        | <span data-ttu-id="16728-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16728-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="16728-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16728-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="16728-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16728-114">AccessReview.ReadWrite.All</span></span> |
| <span data-ttu-id="16728-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16728-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="16728-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16728-116">Not supported.</span></span> |

<span data-ttu-id="16728-117">O usuário de entrada também deve ser um revisor no accessReviewInstance.</span><span class="sxs-lookup"><span data-stu-id="16728-117">The signed-in user must also be a reviewer on the accessReviewInstance.</span></span>

## <a name="http-request"></a><span data-ttu-id="16728-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16728-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/pendingAccessReviewInstances/{instance-id}/acceptRecommendations
```
## <a name="request-headers"></a><span data-ttu-id="16728-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16728-119">Request headers</span></span>
<span data-ttu-id="16728-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16728-120">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="16728-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16728-121">Request body</span></span>
<span data-ttu-id="16728-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16728-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16728-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="16728-123">Response</span></span>
<span data-ttu-id="16728-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16728-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16728-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="16728-126">Examples</span></span>
### <a name="request"></a><span data-ttu-id="16728-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16728-127">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="16728-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="16728-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "acceptrecommendations_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/acceptRecommendations
```
# <a name="c"></a>[<span data-ttu-id="16728-129">C#</span><span class="sxs-lookup"><span data-stu-id="16728-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/acceptrecommendations-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16728-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16728-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/acceptrecommendations-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16728-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16728-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/acceptrecommendations-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16728-132">Java</span><span class="sxs-lookup"><span data-stu-id="16728-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/acceptrecommendations-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16728-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="16728-133">Response</span></span>
><span data-ttu-id="16728-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="16728-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
