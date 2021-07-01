---
title: 'accessReviewInstance: stop'
description: Pare um accessReviewInstance ativo no momento.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 08b9974b1b496a3ff50048d72dbb65659758658e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211026"
---
# <a name="accessreviewinstance-stop"></a><span data-ttu-id="d61e8-103">accessReviewInstance: stop</span><span class="sxs-lookup"><span data-stu-id="d61e8-103">accessReviewInstance: stop</span></span>
<span data-ttu-id="d61e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d61e8-105">Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="d61e8-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="d61e8-106">Depois que a instância de revisão de acesso é interrompida, o status da instância é marcado como , os revisadores não podem mais dar entrada e as decisões de revisão de acesso `Completed` são aplicadas.</span><span class="sxs-lookup"><span data-stu-id="d61e8-106">After the access review instance stops, the instance status is marked as `Completed`, the reviewers can no longer give input, and the access review decisions are applied.</span></span>

<span data-ttu-id="d61e8-107">Parar uma instância não interromperá instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="d61e8-107">Stopping an instance will not stop future instances.</span></span> <span data-ttu-id="d61e8-108">Para impedir que uma revisão de acesso recorrente seja iniciar instâncias futuras, [atualize](accessreviewscheduledefinition-update.md) a definição de agendamento para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="d61e8-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="d61e8-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d61e8-109">Permissions</span></span>
<span data-ttu-id="d61e8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d61e8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d61e8-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d61e8-112">Permission type</span></span>|<span data-ttu-id="d61e8-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d61e8-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d61e8-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d61e8-114">Delegated (work or school account)</span></span>|<span data-ttu-id="d61e8-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61e8-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="d61e8-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d61e8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d61e8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d61e8-117">Not supported.</span></span>|
|<span data-ttu-id="d61e8-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d61e8-118">Application</span></span>|<span data-ttu-id="d61e8-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61e8-119">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d61e8-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d61e8-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stop
```

## <a name="request-headers"></a><span data-ttu-id="d61e8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d61e8-121">Request headers</span></span>
|<span data-ttu-id="d61e8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d61e8-122">Name</span></span>|<span data-ttu-id="d61e8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d61e8-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d61e8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d61e8-124">Authorization</span></span>|<span data-ttu-id="d61e8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d61e8-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d61e8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d61e8-127">Request body</span></span>
<span data-ttu-id="d61e8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d61e8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d61e8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61e8-129">Response</span></span>

<span data-ttu-id="d61e8-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d61e8-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d61e8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d61e8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d61e8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d61e8-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d61e8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d61e8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_stop"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/stop
```
# <a name="c"></a>[<span data-ttu-id="d61e8-134">C#</span><span class="sxs-lookup"><span data-stu-id="d61e8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-stop-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d61e8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d61e8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-stop-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d61e8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d61e8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-stop-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d61e8-137">Java</span><span class="sxs-lookup"><span data-stu-id="d61e8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-stop-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d61e8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d61e8-138">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
