---
title: 'accessReviewInstance: sendReminder'
description: Envia um lembrete aos revisores de um accessReviewInstance ativo no momento.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 20e662e0501091b4482c44450f4223ed5d39a95a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048404"
---
# <a name="accessreviewinstance-sendreminder"></a><span data-ttu-id="df8d8-103">accessReviewInstance: sendReminder</span><span class="sxs-lookup"><span data-stu-id="df8d8-103">accessReviewInstance: sendReminder</span></span>

<span data-ttu-id="df8d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df8d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df8d8-105">Envie um lembrete aos revisores de um [accessReviewInstance](../resources/accessreviewinstance.md)ativo no momento.</span><span class="sxs-lookup"><span data-stu-id="df8d8-105">Send a reminder to the reviewers of a currently active [accessReviewInstance](../resources/accessreviewinstance.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df8d8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="df8d8-106">Permissions</span></span>
<span data-ttu-id="df8d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df8d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df8d8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df8d8-109">Permission type</span></span>                        | <span data-ttu-id="df8d8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="df8d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="df8d8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df8d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df8d8-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8d8-112">AccessReview.ReadWrite.All</span></span> |
|<span data-ttu-id="df8d8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df8d8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df8d8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df8d8-114">Not supported.</span></span>|
|<span data-ttu-id="df8d8-115">Application</span><span class="sxs-lookup"><span data-stu-id="df8d8-115">Application</span></span>                            | <span data-ttu-id="df8d8-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8d8-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df8d8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df8d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions/{definitionId}/instances/{instanceId}/sendReminder
```
## <a name="request-headers"></a><span data-ttu-id="df8d8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df8d8-118">Request headers</span></span>
<span data-ttu-id="df8d8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df8d8-119">None.</span></span>

## <a name="request-body"></a><span data-ttu-id="df8d8-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df8d8-120">Request body</span></span>
<span data-ttu-id="df8d8-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="df8d8-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df8d8-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8d8-122">Response</span></span>
<span data-ttu-id="df8d8-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df8d8-p102">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df8d8-125">Exemplos</span><span class="sxs-lookup"><span data-stu-id="df8d8-125">Examples</span></span>
### <a name="request"></a><span data-ttu-id="df8d8-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df8d8-126">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="df8d8-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="df8d8-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sendReminder_accessReview_2"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/04e5c3b2-9db2-40d3-a204-128f4956ae8e/instances/70463350-742e-4909-bfa5-bc23447bd002/sendReminder
```
# <a name="c"></a>[<span data-ttu-id="df8d8-128">C#</span><span class="sxs-lookup"><span data-stu-id="df8d8-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sendreminder-accessreview-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df8d8-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df8d8-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sendreminder-accessreview-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df8d8-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df8d8-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sendreminder-accessreview-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df8d8-131">Java</span><span class="sxs-lookup"><span data-stu-id="df8d8-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sendreminder-accessreview-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a><span data-ttu-id="df8d8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="df8d8-132">Response</span></span>
><span data-ttu-id="df8d8-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="df8d8-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
