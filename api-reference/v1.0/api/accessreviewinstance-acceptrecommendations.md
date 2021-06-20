---
title: 'accessReviewInstance: acceptRecommendations'
description: Permite a aceitação de recomendações sobre decisões para uma instância de revisão de acesso que não tenha sido revisada pelo usuário chamador que é um revistor.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 60a9e59579f094e2c517c33ee96276220062599b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031018"
---
# <a name="accessreviewinstance-acceptrecommendations"></a><span data-ttu-id="0f176-103">accessReviewInstance: acceptRecommendations</span><span class="sxs-lookup"><span data-stu-id="0f176-103">accessReviewInstance: acceptRecommendations</span></span>

<span data-ttu-id="0f176-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f176-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f176-105">Permite a aceitação de recomendações em todos os objetos [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) que não foram revisados em um [objeto accessReviewInstance](../resources/accessreviewinstance.md) para o qual o usuário de chamada é um revisor.</span><span class="sxs-lookup"><span data-stu-id="0f176-105">Allows the acceptance of recommendations on all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects that have not been reviewed on an [accessReviewInstance](../resources/accessreviewinstance.md) object for which the calling user is a reviewer.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f176-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f176-106">Permissions</span></span>
<span data-ttu-id="0f176-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f176-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f176-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f176-109">Permission type</span></span>|<span data-ttu-id="0f176-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f176-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f176-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f176-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f176-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f176-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="0f176-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f176-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f176-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f176-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f176-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f176-115">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/acceptRecommendations
```

## <a name="request-headers"></a><span data-ttu-id="0f176-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f176-116">Request headers</span></span>
|<span data-ttu-id="0f176-117">Nome</span><span class="sxs-lookup"><span data-stu-id="0f176-117">Name</span></span>|<span data-ttu-id="0f176-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f176-118">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f176-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f176-119">Authorization</span></span>|<span data-ttu-id="0f176-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f176-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f176-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f176-122">Request body</span></span>
<span data-ttu-id="0f176-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0f176-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f176-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f176-124">Response</span></span>

<span data-ttu-id="0f176-125">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f176-125">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0f176-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0f176-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f176-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f176-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_acceptrecommendations"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f91006/acceptRecommendations
```


### <a name="response"></a><span data-ttu-id="0f176-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f176-128">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
