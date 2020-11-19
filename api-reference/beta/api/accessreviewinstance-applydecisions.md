---
title: 'accessReviewInstance: applyDecisions'
description: Aplicar decisões em um accessReviewInstance.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0af1ae1291a95145041a3e92bedf948c766bd1c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214716"
---
# <a name="accessreviewinstance-applydecisions"></a><span data-ttu-id="5f6ff-103">accessReviewInstance: applyDecisions</span><span class="sxs-lookup"><span data-stu-id="5f6ff-103">accessReviewInstance: applyDecisions</span></span>

<span data-ttu-id="5f6ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f6ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f6ff-105">Aplicar decisões de revisão em um [accessReviewInstance](../resources/accessreviewinstance.md).</span><span class="sxs-lookup"><span data-stu-id="5f6ff-105">Apply review decisions on an [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

<span data-ttu-id="5f6ff-106">Observe que as decisões serão aplicadas automaticamente se o parâmetro autoApplyDecisionsEnabled for true no [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)da revisão.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-106">Note that decisions will be applied automatically if the autoApplyDecisionsEnabled parameter is True in the review's [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5f6ff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f6ff-107">Permissions</span></span>
<span data-ttu-id="5f6ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f6ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f6ff-110">Permission type</span></span>                        | <span data-ttu-id="5f6ff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f6ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f6ff-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f6ff-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5f6ff-113">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f6ff-113">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="5f6ff-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f6ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f6ff-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-115">Not supported.</span></span>|
|<span data-ttu-id="5f6ff-116">Application</span><span class="sxs-lookup"><span data-stu-id="5f6ff-116">Application</span></span>                            | <span data-ttu-id="5f6ff-117">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f6ff-117">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f6ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f6ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/applyDecisions
```

## <a name="request-headers"></a><span data-ttu-id="5f6ff-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f6ff-119">Request headers</span></span>
|<span data-ttu-id="5f6ff-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5f6ff-120">Name</span></span>|<span data-ttu-id="5f6ff-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f6ff-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f6ff-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f6ff-122">Authorization</span></span>|<span data-ttu-id="5f6ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5f6ff-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5f6ff-125">Content-Type</span></span>|<span data-ttu-id="5f6ff-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f6ff-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f6ff-128">Request body</span></span>
<span data-ttu-id="5f6ff-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f6ff-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f6ff-130">Response</span></span>
<span data-ttu-id="5f6ff-131">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-131">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5f6ff-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f6ff-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f6ff-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f6ff-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f6ff-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f6ff-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_applydecisions"
}
-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/applyDecisions
```
# <a name="c"></a>[<span data-ttu-id="5f6ff-135">C#</span><span class="sxs-lookup"><span data-stu-id="5f6ff-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-applydecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f6ff-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f6ff-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-applydecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f6ff-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f6ff-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-applydecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f6ff-138">Java</span><span class="sxs-lookup"><span data-stu-id="5f6ff-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-applydecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="5f6ff-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f6ff-139">Response</span></span>
<span data-ttu-id="5f6ff-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f6ff-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
