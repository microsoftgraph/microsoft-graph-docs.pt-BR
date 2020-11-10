---
title: 'offerShiftRequest: recusar'
description: Recusar uma solicitação de mudança de oferta.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a09a74645abf8fd9c6bc537246d6b96d91e9d546
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981290"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="996c4-103">offerShiftRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="996c4-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="996c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="996c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="996c4-105">Recusar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="996c4-105">Decline an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="996c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="996c4-106">Permissions</span></span>

<span data-ttu-id="996c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="996c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="996c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="996c4-109">Permission type</span></span>                        | <span data-ttu-id="996c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="996c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="996c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="996c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="996c4-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="996c4-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="996c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="996c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="996c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="996c4-114">Not supported.</span></span> |
| <span data-ttu-id="996c4-115">Application</span><span class="sxs-lookup"><span data-stu-id="996c4-115">Application</span></span>                            | <span data-ttu-id="996c4-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="996c4-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="996c4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="996c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="996c4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="996c4-118">Request headers</span></span>

| <span data-ttu-id="996c4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="996c4-119">Name</span></span>          | <span data-ttu-id="996c4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="996c4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="996c4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="996c4-121">Authorization</span></span> | <span data-ttu-id="996c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="996c4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="996c4-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="996c4-124">Content-type</span></span> | <span data-ttu-id="996c4-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="996c4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="996c4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="996c4-127">Request body</span></span>

<span data-ttu-id="996c4-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="996c4-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="996c4-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="996c4-129">Parameter</span></span>    | <span data-ttu-id="996c4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="996c4-130">Type</span></span>        | <span data-ttu-id="996c4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="996c4-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="996c4-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="996c4-132">message</span></span>|<span data-ttu-id="996c4-133">String</span><span class="sxs-lookup"><span data-stu-id="996c4-133">String</span></span>|<span data-ttu-id="996c4-134">Mensagem personalizada enviada ao recusar.</span><span class="sxs-lookup"><span data-stu-id="996c4-134">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="996c4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="996c4-135">Response</span></span>

<span data-ttu-id="996c4-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="996c4-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="996c4-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="996c4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="996c4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="996c4-139">Request</span></span>

<span data-ttu-id="996c4-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="996c4-140">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="996c4-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="996c4-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="javascript"></a>[<span data-ttu-id="996c4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="996c4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="996c4-143">C#</span><span class="sxs-lookup"><span data-stu-id="996c4-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="996c4-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="996c4-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="996c4-145">Java</span><span class="sxs-lookup"><span data-stu-id="996c4-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="996c4-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="996c4-146">Response</span></span>

<span data-ttu-id="996c4-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="996c4-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


