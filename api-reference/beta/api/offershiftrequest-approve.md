---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offershiftrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 51de5257597947f1a7a83740862e9e8f89ccf728
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313762"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="b389c-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="b389c-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="b389c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b389c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b389c-105">Aprovar um objeto [offershiftrequest](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b389c-105">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b389c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b389c-106">Permissions</span></span>

<span data-ttu-id="b389c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b389c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b389c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b389c-109">Permission type</span></span>                        | <span data-ttu-id="b389c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b389c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b389c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b389c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b389c-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b389c-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b389c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b389c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b389c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b389c-114">Not supported.</span></span> |
| <span data-ttu-id="b389c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b389c-115">Application</span></span>                            | <span data-ttu-id="b389c-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b389c-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b389c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b389c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="b389c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b389c-118">Request headers</span></span>

| <span data-ttu-id="b389c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b389c-119">Name</span></span>          | <span data-ttu-id="b389c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b389c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b389c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b389c-121">Authorization</span></span> | <span data-ttu-id="b389c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b389c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b389c-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="b389c-124">Content-type</span></span> | <span data-ttu-id="b389c-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b389c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b389c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b389c-127">Request body</span></span>

<span data-ttu-id="b389c-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b389c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b389c-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b389c-129">Parameter</span></span>    | <span data-ttu-id="b389c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b389c-130">Type</span></span>        | <span data-ttu-id="b389c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b389c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b389c-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="b389c-132">message</span></span>|<span data-ttu-id="b389c-133">String</span><span class="sxs-lookup"><span data-stu-id="b389c-133">String</span></span>|<span data-ttu-id="b389c-134">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="b389c-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="b389c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b389c-135">Response</span></span>

<span data-ttu-id="b389c-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b389c-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b389c-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b389c-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b389c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b389c-139">Request</span></span>

<span data-ttu-id="b389c-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b389c-140">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b389c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="b389c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="javascript"></a>[<span data-ttu-id="b389c-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b389c-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="b389c-143">C#</span><span class="sxs-lookup"><span data-stu-id="b389c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b389c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b389c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b389c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b389c-145">Response</span></span>

<span data-ttu-id="b389c-146">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="b389c-146">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


