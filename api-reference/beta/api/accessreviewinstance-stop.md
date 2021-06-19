---
title: Parar accessReviewInstance
description: Pare um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c59b08c3a451d54a03502b28d2f05350f38e126f
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030485"
---
# <a name="stop-accessreviewinstance"></a><span data-ttu-id="8dbee-103">Parar accessReviewInstance</span><span class="sxs-lookup"><span data-stu-id="8dbee-103">Stop accessReviewInstance</span></span>

<span data-ttu-id="8dbee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8dbee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dbee-105">Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="8dbee-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="8dbee-106">Depois que a instância de revisão de acesso parar, o status da instância será , os revisadores não poderão mais dar entrada e as decisões de revisão de acesso `Completed` podem ser aplicadas.</span><span class="sxs-lookup"><span data-stu-id="8dbee-106">After the access review instance stops, the instance status will be `Completed`, the reviewers can no longer give input, and the access review decisions can be applied.</span></span>

<span data-ttu-id="8dbee-107">Parar uma instância não terá efeito em instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="8dbee-107">Stopping an instance will not effect future instances.</span></span> <span data-ttu-id="8dbee-108">Para impedir que uma revisão de acesso recorrente seja iniciar instâncias futuras, [atualize](accessreviewscheduledefinition-update.md) a definição de agendamento para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="8dbee-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dbee-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dbee-109">Permissions</span></span>
<span data-ttu-id="8dbee-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dbee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dbee-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dbee-112">Permission type</span></span>                        | <span data-ttu-id="8dbee-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dbee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8dbee-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dbee-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dbee-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbee-115">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="8dbee-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dbee-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dbee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dbee-117">Not supported.</span></span>|
|<span data-ttu-id="8dbee-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dbee-118">Application</span></span>                            | <span data-ttu-id="8dbee-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbee-119">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8dbee-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dbee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/stop
```

## <a name="request-headers"></a><span data-ttu-id="8dbee-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-121">Request headers</span></span>
<span data-ttu-id="8dbee-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8dbee-122">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="8dbee-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-123">Request body</span></span>
<span data-ttu-id="8dbee-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8dbee-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8dbee-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbee-125">Response</span></span>
<span data-ttu-id="8dbee-p104">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dbee-p104">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dbee-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8dbee-128">Examples</span></span>
### <a name="request"></a><span data-ttu-id="8dbee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8dbee-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dbee-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReviewInstance"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stop
```
# <a name="c"></a>[<span data-ttu-id="8dbee-131">C#</span><span class="sxs-lookup"><span data-stu-id="8dbee-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreviewinstance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dbee-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dbee-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreviewinstance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dbee-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dbee-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreviewinstance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dbee-134">Java</span><span class="sxs-lookup"><span data-stu-id="8dbee-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/stop-accessreviewinstance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="8dbee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbee-135">Response</span></span>
><span data-ttu-id="8dbee-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8dbee-136">**Note:** The response object shown here might be shortened for readability.</span></span>
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
