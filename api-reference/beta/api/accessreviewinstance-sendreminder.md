---
title: 'accessReviewInstance: sendReminder'
description: Envia um lembrete aos revisores de um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8d18613b1fc59db04ce0f7fdfe6d3937542ed0dd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943053"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="29b13-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="29b13-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="29b13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29b13-105">Envie um lembrete aos revisores de um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="29b13-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="29b13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="29b13-106">Permissions</span></span>
<span data-ttu-id="29b13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29b13-109">Permission type</span></span>                        | <span data-ttu-id="29b13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29b13-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="29b13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29b13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="29b13-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b13-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="29b13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29b13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29b13-114">Not supported.</span></span>|
|<span data-ttu-id="29b13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29b13-115">Application</span></span>                            | <span data-ttu-id="29b13-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29b13-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29b13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29b13-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="29b13-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29b13-118">Request headers</span></span>
<span data-ttu-id="29b13-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29b13-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="29b13-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29b13-120">Request body</span></span>
<span data-ttu-id="29b13-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="29b13-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29b13-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b13-122">Response</span></span>
<span data-ttu-id="29b13-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29b13-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29b13-125">Exemplos</span><span class="sxs-lookup"><span data-stu-id="29b13-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="29b13-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29b13-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29b13-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="29b13-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="29b13-128">C#</span><span class="sxs-lookup"><span data-stu-id="29b13-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29b13-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29b13-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29b13-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29b13-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29b13-131">Java</span><span class="sxs-lookup"><span data-stu-id="29b13-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="29b13-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b13-132">Response</span></span>
><span data-ttu-id="29b13-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29b13-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "SendReminder accessReviewInstance",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
