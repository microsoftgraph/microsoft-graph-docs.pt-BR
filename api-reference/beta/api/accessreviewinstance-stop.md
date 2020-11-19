---
title: Parar accessReviewInstance
description: Parar um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7e2ab7d5dddfbc1b5903f4a4379e8133278dc6bc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221972"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="fdf86-103">Parar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="fdf86-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="fdf86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdf86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdf86-105">Parar um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="fdf86-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="fdf86-106">Para impedir que uma revisão de acesso recorrente inicie instâncias futuras, [atualize-](accessreviewscheduledefinition-update.md) a para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="fdf86-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="fdf86-107">Depois que a revisão do Access for interrompida, os revisores não poderão mais fornecer entradas e as decisões de revisão do Access poderão ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="fdf86-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdf86-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdf86-108">Permissions</span></span>
<span data-ttu-id="fdf86-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf86-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdf86-111">Permission type</span></span>                        | <span data-ttu-id="fdf86-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdf86-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdf86-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdf86-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fdf86-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf86-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="fdf86-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdf86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf86-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf86-116">Not supported.</span></span>|
|<span data-ttu-id="fdf86-117">Application</span><span class="sxs-lookup"><span data-stu-id="fdf86-117">Application</span></span>                            | <span data-ttu-id="fdf86-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf86-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fdf86-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf86-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="fdf86-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf86-120">Request headers</span></span>
<span data-ttu-id="fdf86-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fdf86-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="fdf86-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf86-122">Request body</span></span>
<span data-ttu-id="fdf86-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdf86-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdf86-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf86-124">Response</span></span>
<span data-ttu-id="fdf86-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdf86-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fdf86-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fdf86-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="fdf86-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf86-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fdf86-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf86-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="fdf86-130">C#</span><span class="sxs-lookup"><span data-stu-id="fdf86-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdf86-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdf86-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdf86-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdf86-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdf86-133">Java</span><span class="sxs-lookup"><span data-stu-id="fdf86-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="fdf86-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf86-134">Response</span></span>
><span data-ttu-id="fdf86-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdf86-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
