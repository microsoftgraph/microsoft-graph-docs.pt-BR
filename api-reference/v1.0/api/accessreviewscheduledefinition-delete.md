---
title: Excluir accessReviewScheduleDefinition
description: Exclui um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 976d8efe286f698aec8ecaf737d921569ad5842d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210469"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="5adec-103">Excluir accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="5adec-103">Delete accessReviewScheduleDefinition</span></span>
<span data-ttu-id="5adec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5adec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5adec-105">Exclui um [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5adec-105">Deletes an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5adec-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5adec-106">Permissions</span></span>
<span data-ttu-id="5adec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5adec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5adec-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5adec-109">Permission type</span></span>|<span data-ttu-id="5adec-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5adec-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5adec-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5adec-111">Delegated (work or school account)</span></span>| <span data-ttu-id="5adec-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5adec-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="5adec-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5adec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5adec-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5adec-114">Not supported.</span></span>|
|<span data-ttu-id="5adec-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5adec-115">Application</span></span>| <span data-ttu-id="5adec-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5adec-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5adec-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5adec-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="5adec-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5adec-118">Request headers</span></span>
|<span data-ttu-id="5adec-119">Nome</span><span class="sxs-lookup"><span data-stu-id="5adec-119">Name</span></span>|<span data-ttu-id="5adec-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5adec-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5adec-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5adec-121">Authorization</span></span>|<span data-ttu-id="5adec-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5adec-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5adec-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5adec-124">Request body</span></span>
<span data-ttu-id="5adec-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5adec-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5adec-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5adec-126">Response</span></span>

<span data-ttu-id="5adec-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5adec-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5adec-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5adec-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5adec-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5adec-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5adec-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="5adec-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessreviewscheduledefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```
# <a name="c"></a>[<span data-ttu-id="5adec-131">C#</span><span class="sxs-lookup"><span data-stu-id="5adec-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5adec-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5adec-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5adec-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5adec-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5adec-134">Java</span><span class="sxs-lookup"><span data-stu-id="5adec-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5adec-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="5adec-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
