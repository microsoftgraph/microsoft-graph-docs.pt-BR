---
title: 'accessReviewInstance: resetDecisions'
description: Redefine todos os objetos accessReviewInstanceDecisionItem em um accessReviewInstance como `notReviewed` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 778618535bc8d9d0eaf6dcc19ad697fa23de7db5
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031000"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="af1e9-103">accessReviewInstance: resetDecisions</span><span class="sxs-lookup"><span data-stu-id="af1e9-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="af1e9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af1e9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af1e9-105">Redefine todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em [um accessReviewInstance](../resources/accessreviewinstance.md) como `notReviewed` .</span><span class="sxs-lookup"><span data-stu-id="af1e9-105">Resets all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="af1e9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af1e9-106">Permissions</span></span>
<span data-ttu-id="af1e9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af1e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af1e9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af1e9-109">Permission type</span></span>|<span data-ttu-id="af1e9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af1e9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af1e9-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af1e9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="af1e9-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1e9-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="af1e9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af1e9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af1e9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="af1e9-114">Not supported.</span></span>|
|<span data-ttu-id="af1e9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af1e9-115">Application</span></span>|<span data-ttu-id="af1e9-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af1e9-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af1e9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af1e9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="af1e9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e9-118">Request headers</span></span>
|<span data-ttu-id="af1e9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="af1e9-119">Name</span></span>|<span data-ttu-id="af1e9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="af1e9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="af1e9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="af1e9-121">Authorization</span></span>|<span data-ttu-id="af1e9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af1e9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="af1e9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e9-124">Request body</span></span>
<span data-ttu-id="af1e9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="af1e9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af1e9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e9-126">Response</span></span>

<span data-ttu-id="af1e9-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="af1e9-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="af1e9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="af1e9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="af1e9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af1e9-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions
```


### <a name="response"></a><span data-ttu-id="af1e9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="af1e9-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
