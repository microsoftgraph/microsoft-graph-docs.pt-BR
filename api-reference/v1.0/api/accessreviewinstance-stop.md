---
title: 'accessReviewInstance: stop'
description: Pare um accessReviewInstance ativo no momento.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e119d3c914a793bfc083722fb329bd18a72b46df
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030996"
---
# <a name="accessreviewinstance-stop"></a><span data-ttu-id="184b2-103">accessReviewInstance: stop</span><span class="sxs-lookup"><span data-stu-id="184b2-103">accessReviewInstance: stop</span></span>
<span data-ttu-id="184b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="184b2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="184b2-105">Pare um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="184b2-105">Stop a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span> <span data-ttu-id="184b2-106">Depois que a instância de revisão de acesso é interrompida, o status da instância é marcado como , os revisadores não podem mais dar entrada e as decisões de revisão de acesso `Completed` são aplicadas.</span><span class="sxs-lookup"><span data-stu-id="184b2-106">After the access review instance stops, the instance status is marked as `Completed`, the reviewers can no longer give input, and the access review decisions are applied.</span></span>

<span data-ttu-id="184b2-107">Parar uma instância não interromperá instâncias futuras.</span><span class="sxs-lookup"><span data-stu-id="184b2-107">Stopping an instance will not stop future instances.</span></span> <span data-ttu-id="184b2-108">Para impedir que uma revisão de acesso recorrente seja iniciar instâncias futuras, [atualize](accessreviewscheduledefinition-update.md) a definição de agendamento para alterar sua data de término agendada.</span><span class="sxs-lookup"><span data-stu-id="184b2-108">To prevent a recurring access review from starting future instances, [update the schedule definition](accessreviewscheduledefinition-update.md) to change its scheduled end date.</span></span>

## <a name="permissions"></a><span data-ttu-id="184b2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="184b2-109">Permissions</span></span>
<span data-ttu-id="184b2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="184b2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184b2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="184b2-112">Permission type</span></span>|<span data-ttu-id="184b2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="184b2-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="184b2-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="184b2-114">Delegated (work or school account)</span></span>|<span data-ttu-id="184b2-115">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184b2-115">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="184b2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="184b2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="184b2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="184b2-117">Not supported.</span></span>|
|<span data-ttu-id="184b2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="184b2-118">Application</span></span>|<span data-ttu-id="184b2-119">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184b2-119">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="184b2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="184b2-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stop
```

## <a name="request-headers"></a><span data-ttu-id="184b2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="184b2-121">Request headers</span></span>
|<span data-ttu-id="184b2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="184b2-122">Name</span></span>|<span data-ttu-id="184b2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="184b2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="184b2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="184b2-124">Authorization</span></span>|<span data-ttu-id="184b2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="184b2-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="184b2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="184b2-127">Request body</span></span>
<span data-ttu-id="184b2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="184b2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="184b2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="184b2-129">Response</span></span>

<span data-ttu-id="184b2-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="184b2-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="184b2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="184b2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="184b2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="184b2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_stop"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/stop
```


### <a name="response"></a><span data-ttu-id="184b2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="184b2-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
