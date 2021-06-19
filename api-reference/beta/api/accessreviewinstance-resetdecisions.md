---
title: 'accessReviewInstance: resetDecisions'
description: Redefine todos os objetos accessReviewInstanceDecisionItem em um accessReviewInstance como `notReviewed` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cfe9e5c0fe7390a9c2204678b7a926ef225154cf
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031428"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="0d1a0-103">accessReviewInstance: resetDecisions</span><span class="sxs-lookup"><span data-stu-id="0d1a0-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="0d1a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d1a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d1a0-105">Redefine as decisões de todos os [objetos accessReviewInstanceDecisionItem em](../resources/accessreviewinstancedecisionitem.md) [um accessReviewInstance](../resources/accessreviewinstance.md) como `notReviewed` .</span><span class="sxs-lookup"><span data-stu-id="0d1a0-105">Resets decisions of all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d1a0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d1a0-106">Permissions</span></span>
<span data-ttu-id="0d1a0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d1a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d1a0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d1a0-109">Permission type</span></span>|<span data-ttu-id="0d1a0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d1a0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d1a0-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d1a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0d1a0-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d1a0-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0d1a0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d1a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d1a0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d1a0-114">Not supported.</span></span>|
|<span data-ttu-id="0d1a0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d1a0-115">Application</span></span>|<span data-ttu-id="0d1a0-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d1a0-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d1a0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d1a0-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="0d1a0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1a0-118">Request headers</span></span>
|<span data-ttu-id="0d1a0-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0d1a0-119">Name</span></span>|<span data-ttu-id="0d1a0-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d1a0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d1a0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d1a0-121">Authorization</span></span>|<span data-ttu-id="0d1a0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d1a0-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d1a0-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1a0-124">Request body</span></span>
<span data-ttu-id="0d1a0-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d1a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d1a0-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d1a0-126">Response</span></span>

<span data-ttu-id="0d1a0-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0d1a0-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0d1a0-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d1a0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d1a0-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d1a0-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-44b5-ae36-41b923c3bf87/resetDecisions
```


### <a name="response"></a><span data-ttu-id="0d1a0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d1a0-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
