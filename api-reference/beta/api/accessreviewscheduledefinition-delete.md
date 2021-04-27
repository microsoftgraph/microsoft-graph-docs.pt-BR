---
title: Excluir accessReviewScheduleDefinition
description: Exclua um objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 53ef0c8f98c240ad0544b7d816c12ec1cac8c507
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048362"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="27d74-103">Excluir accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="27d74-103">Delete accessReviewScheduleDefinition</span></span>

<span data-ttu-id="27d74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27d74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d74-105">[Exclua um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="27d74-105">Delete an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27d74-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="27d74-106">Permissions</span></span>
<span data-ttu-id="27d74-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27d74-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27d74-109">Permission type</span></span>                        | <span data-ttu-id="27d74-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27d74-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="27d74-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27d74-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27d74-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d74-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="27d74-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27d74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27d74-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27d74-114">Not supported.</span></span>|
|<span data-ttu-id="27d74-115">Application</span><span class="sxs-lookup"><span data-stu-id="27d74-115">Application</span></span>                            | <span data-ttu-id="27d74-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d74-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d74-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27d74-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a><span data-ttu-id="27d74-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27d74-118">Request headers</span></span>
<span data-ttu-id="27d74-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="27d74-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="27d74-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27d74-120">Request body</span></span>
<span data-ttu-id="27d74-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27d74-121">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="27d74-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d74-122">Response</span></span>
<span data-ttu-id="27d74-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d74-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27d74-125">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27d74-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="27d74-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d74-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="27d74-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="27d74-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/29f2d16e-9ca6-4052-bbfe-802c48981fd8
```
# <a name="c"></a>[<span data-ttu-id="27d74-128">C#</span><span class="sxs-lookup"><span data-stu-id="27d74-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27d74-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27d74-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27d74-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27d74-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27d74-131">Java</span><span class="sxs-lookup"><span data-stu-id="27d74-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="27d74-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d74-132">Response</span></span>
><span data-ttu-id="27d74-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27d74-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
