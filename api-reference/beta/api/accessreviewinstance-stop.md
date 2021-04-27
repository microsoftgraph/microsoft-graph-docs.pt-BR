---
title: Parar accessReviewInstance
description: Pare um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0655b0acd7dbd32b0ae4aae5337422f26f9c7c96
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048390"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="f0669-103">Parar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="f0669-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="f0669-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0669-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0669-105">Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="f0669-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="f0669-106">Para impedir que uma revisão de acesso recorrente inseja instâncias futuras, [atualize-a](accessreviewscheduledefinition-update.md) para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="f0669-106">To prevent a recurring access review from starting future instances, [update it](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>  <span data-ttu-id="f0669-107">Depois que a revisão de acesso parar, os revisadores não poderão mais dar entrada e as decisões de revisão de acesso podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="f0669-107">After the access review stops, reviewers can no longer give input, and the access review decisions can be applied.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0669-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0669-108">Permissions</span></span>
<span data-ttu-id="f0669-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0669-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0669-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0669-111">Permission type</span></span>                        | <span data-ttu-id="f0669-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0669-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0669-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0669-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0669-114">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0669-114">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="f0669-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0669-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0669-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0669-116">Not supported.</span></span>|
|<span data-ttu-id="f0669-117">Application</span><span class="sxs-lookup"><span data-stu-id="f0669-117">Application</span></span>                            | <span data-ttu-id="f0669-118">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0669-118">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0669-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0669-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="f0669-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0669-120">Request headers</span></span>
<span data-ttu-id="f0669-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0669-121">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="f0669-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0669-122">Request body</span></span>
<span data-ttu-id="f0669-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0669-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0669-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0669-124">Response</span></span>
<span data-ttu-id="f0669-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0669-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0669-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f0669-127">Examples</span></span>
### <a name="request"></a><span data-ttu-id="f0669-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0669-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f0669-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0669-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="f0669-130">C#</span><span class="sxs-lookup"><span data-stu-id="f0669-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0669-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0669-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0669-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0669-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0669-133">Java</span><span class="sxs-lookup"><span data-stu-id="f0669-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="f0669-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0669-134">Response</span></span>
><span data-ttu-id="f0669-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f0669-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
