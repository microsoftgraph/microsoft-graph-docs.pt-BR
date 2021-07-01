---
title: 'accessReviewInstance: applyDecisions'
description: Aplicar decisões em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4d198df270427afa910ec962b5f92b821ebd7fa6
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209895"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="7e312-103">accessReviewInstance: applyDecisions</span><span class="sxs-lookup"><span data-stu-id="7e312-103">accessReviewInstance: applyDecisions</span></span>
<span data-ttu-id="7e312-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e312-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e312-105">Aplicar decisões de revisão ao recurso revisado em [um accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="7e312-105">Apply review decisions to the resource reviewed in an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="7e312-106">As decisões serão aplicadas automaticamente **se o autoApplyDecisionsEnabled** do parâmetro **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) for `true` .</span><span class="sxs-lookup"><span data-stu-id="7e312-106">Decisions are applied automatically if the **autoApplyDecisionsEnabled** of the **settings** parameter of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) is `true`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e312-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e312-107">Permissions</span></span>
<span data-ttu-id="7e312-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e312-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e312-110">Permission type</span></span>|<span data-ttu-id="7e312-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e312-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e312-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e312-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e312-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e312-113">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="7e312-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e312-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e312-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e312-115">Not supported.</span></span>|
|<span data-ttu-id="7e312-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e312-116">Application</span></span>|<span data-ttu-id="7e312-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e312-117">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e312-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e312-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="7e312-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e312-119">Request headers</span></span>
|<span data-ttu-id="7e312-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7e312-120">Name</span></span>|<span data-ttu-id="7e312-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e312-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7e312-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e312-122">Authorization</span></span>|<span data-ttu-id="7e312-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e312-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e312-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e312-125">Request body</span></span>
<span data-ttu-id="7e312-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e312-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e312-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e312-127">Response</span></span>

<span data-ttu-id="7e312-128">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e312-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7e312-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e312-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e312-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e312-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7e312-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e312-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-5678-8868-0810c7f49101/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="7e312-132">C#</span><span class="sxs-lookup"><span data-stu-id="7e312-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-applydecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e312-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e312-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-applydecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e312-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e312-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-applydecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e312-135">Java</span><span class="sxs-lookup"><span data-stu-id="7e312-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-applydecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7e312-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e312-136">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
