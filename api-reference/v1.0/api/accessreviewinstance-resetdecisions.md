---
title: 'accessReviewInstance: resetDecisions'
description: Redefine todos os objetos accessReviewInstanceDecisionItem em um accessReviewInstance como `notReviewed` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 269c3f4891fb62d9191991ffa50dc70635268020
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209755"
---
# <a name="accessreviewinstance-resetdecisions"></a><span data-ttu-id="a608e-103">accessReviewInstance: resetDecisions</span><span class="sxs-lookup"><span data-stu-id="a608e-103">accessReviewInstance: resetDecisions</span></span>
<span data-ttu-id="a608e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a608e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a608e-105">Redefine todos os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em [um accessReviewInstance](../resources/accessreviewinstance.md) como `notReviewed` .</span><span class="sxs-lookup"><span data-stu-id="a608e-105">Resets all [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) objects on an [accessReviewInstance](../resources/accessreviewinstance.md) to `notReviewed`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a608e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a608e-106">Permissions</span></span>
<span data-ttu-id="a608e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a608e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a608e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a608e-109">Permission type</span></span>|<span data-ttu-id="a608e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a608e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a608e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a608e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a608e-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a608e-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="a608e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a608e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a608e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a608e-114">Not supported.</span></span>|
|<span data-ttu-id="a608e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a608e-115">Application</span></span>|<span data-ttu-id="a608e-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a608e-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a608e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a608e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/resetDecisions
```

## <a name="request-headers"></a><span data-ttu-id="a608e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a608e-118">Request headers</span></span>
|<span data-ttu-id="a608e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a608e-119">Name</span></span>|<span data-ttu-id="a608e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a608e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a608e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a608e-121">Authorization</span></span>|<span data-ttu-id="a608e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a608e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a608e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a608e-124">Request body</span></span>
<span data-ttu-id="a608e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a608e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a608e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a608e-126">Response</span></span>

<span data-ttu-id="a608e-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a608e-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a608e-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a608e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a608e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a608e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a608e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a608e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_resetdecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/resetDecisions
```
# <a name="c"></a>[<span data-ttu-id="a608e-131">C#</span><span class="sxs-lookup"><span data-stu-id="a608e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-resetdecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a608e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a608e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-resetdecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a608e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a608e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-resetdecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a608e-134">Java</span><span class="sxs-lookup"><span data-stu-id="a608e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-resetdecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a608e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a608e-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
