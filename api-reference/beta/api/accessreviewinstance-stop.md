---
title: Parar accessReviewInstance
description: Pare um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4f9a7dde832cc4d8dcf8353df65789d38d201a7a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439139"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="b210e-103">Parar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="b210e-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="b210e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b210e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b210e-105">Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="b210e-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="b210e-106">Para impedir que uma revisão de acesso recorrente inseja instâncias futuras, [atualize-a](accessreviewscheduledefinition-update.md) para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="b210e-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="b210e-107">Depois que a revisão de acesso parar, os revisadores não poderão mais dar entrada e as decisões de revisão de acesso podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="b210e-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="b210e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="b210e-108">Permissions</span></span>
<span data-ttu-id="b210e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b210e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b210e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b210e-111">Permission type</span></span>                        | <span data-ttu-id="b210e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b210e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b210e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b210e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="b210e-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b210e-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="b210e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b210e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b210e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b210e-116">Not supported.</span></span>|
|<span data-ttu-id="b210e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b210e-117">Application</span></span>                            | <span data-ttu-id="b210e-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b210e-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b210e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b210e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="b210e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b210e-120">Request headers</span></span>
<span data-ttu-id="b210e-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b210e-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="b210e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b210e-122">Request body</span></span>
<span data-ttu-id="b210e-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b210e-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b210e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="b210e-124">Response</span></span>
<span data-ttu-id="b210e-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b210e-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b210e-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b210e-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b210e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b210e-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b210e-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="b210e-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="b210e-130">C#</span><span class="sxs-lookup"><span data-stu-id="b210e-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b210e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b210e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b210e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b210e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b210e-133">Java</span><span class="sxs-lookup"><span data-stu-id="b210e-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="b210e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b210e-134">Response</span></span>
><span data-ttu-id="b210e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b210e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
