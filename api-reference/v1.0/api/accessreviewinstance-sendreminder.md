---
title: 'accessReviewInstance: sendReminder'
description: Envia um lembrete aos revisores de um accessReviewInstance ativo no momento.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 00608ba03cbf3106b9707fc0e236328f2dfd1e65
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210952"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="7e550-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="7e550-103">accessReviewInstance: sendReminder</span></span>
<span data-ttu-id="7e550-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e550-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e550-105">Envie um lembrete aos revisores de um [accessReviewInstance ativo.](../resources/accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="7e550-105">Send a reminder to the reviewers of an active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e550-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e550-106">Permissions</span></span>
<span data-ttu-id="7e550-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e550-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e550-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e550-109">Permission type</span></span>|<span data-ttu-id="7e550-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e550-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e550-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e550-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7e550-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e550-112">AccessReview.ReadWrite.All</span></span>|
|<span data-ttu-id="7e550-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e550-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e550-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e550-114">Not supported.</span></span>|
|<span data-ttu-id="7e550-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e550-115">Application</span></span>|<span data-ttu-id="7e550-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e550-116">AccessReview.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e550-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e550-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/sendReminder
```

## <a name="request-headers"></a><span data-ttu-id="7e550-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e550-118">Request headers</span></span>
|<span data-ttu-id="7e550-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7e550-119">Name</span></span>|<span data-ttu-id="7e550-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e550-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7e550-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e550-121">Authorization</span></span>|<span data-ttu-id="7e550-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e550-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e550-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e550-124">Request body</span></span>
<span data-ttu-id="7e550-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e550-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e550-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e550-126">Response</span></span>

<span data-ttu-id="7e550-127">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7e550-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7e550-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7e550-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7e550-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e550-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7e550-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e550-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_sendreminder"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="7e550-131">C#</span><span class="sxs-lookup"><span data-stu-id="7e550-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-sendreminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e550-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e550-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-sendreminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e550-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e550-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-sendreminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e550-134">Java</span><span class="sxs-lookup"><span data-stu-id="7e550-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-sendreminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7e550-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e550-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
