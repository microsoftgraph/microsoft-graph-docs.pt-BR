---
title: 'accessReviewInstance: applyDecisions'
description: Aplicar decisões em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 93cc4d2e4f5c42ebe47bed00caf227779b579df2
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030287"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="b1d16-103">accessReviewInstance: applyDecisions</span><span class="sxs-lookup"><span data-stu-id="b1d16-103">accessReviewInstance: applyDecisions</span></span>
<span data-ttu-id="b1d16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1d16-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1d16-105">Aplicar decisões de revisão ao recurso revisado em [um accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="b1d16-105">Apply review decisions to the resource reviewed in an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="b1d16-106">As decisões serão aplicadas automaticamente **se o autoApplyDecisionsEnabled** do parâmetro **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true` .</span><span class="sxs-lookup"><span data-stu-id="b1d16-106">Decisions are applied automatically if the **autoApplyDecisionsEnabled** of the **settings** parameter of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1d16-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1d16-107">Permissions</span></span>
<span data-ttu-id="b1d16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1d16-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1d16-110">Permission type</span></span>|<span data-ttu-id="b1d16-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1d16-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1d16-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1d16-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1d16-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d16-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="b1d16-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1d16-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1d16-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1d16-115">Not supported.</span></span>|
|<span data-ttu-id="b1d16-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1d16-116">Application</span></span>|<span data-ttu-id="b1d16-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1d16-117">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1d16-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1d16-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="b1d16-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d16-119">Request headers</span></span>
|<span data-ttu-id="b1d16-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b1d16-120">Name</span></span>|<span data-ttu-id="b1d16-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1d16-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1d16-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1d16-122">Authorization</span></span>|<span data-ttu-id="b1d16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1d16-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1d16-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d16-125">Request body</span></span>
<span data-ttu-id="b1d16-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b1d16-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1d16-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1d16-127">Response</span></span>

<span data-ttu-id="b1d16-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b1d16-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b1d16-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b1d16-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1d16-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1d16-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f49101/applyDecisions
```


### <a name="response"></a><span data-ttu-id="b1d16-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1d16-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
