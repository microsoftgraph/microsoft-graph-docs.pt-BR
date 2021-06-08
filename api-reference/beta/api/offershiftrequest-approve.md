---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offershiftrequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b2a3ef65cbf138547acbed15f1fbae884467bbc7
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786478"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="fad12-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="fad12-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="fad12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fad12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fad12-105">Aprovar um [objeto offershiftrequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="fad12-105">Approve an [offershiftrequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fad12-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fad12-106">Permissions</span></span>

<span data-ttu-id="fad12-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fad12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fad12-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fad12-109">Permission type</span></span>                        | <span data-ttu-id="fad12-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fad12-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fad12-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fad12-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fad12-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad12-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="fad12-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fad12-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fad12-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fad12-114">Not supported.</span></span> |
| <span data-ttu-id="fad12-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fad12-115">Application</span></span>                            | <span data-ttu-id="fad12-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fad12-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fad12-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fad12-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="fad12-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fad12-118">Request headers</span></span>

| <span data-ttu-id="fad12-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fad12-119">Name</span></span>          | <span data-ttu-id="fad12-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="fad12-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fad12-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fad12-121">Authorization</span></span> | <span data-ttu-id="fad12-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fad12-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fad12-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="fad12-124">Content-type</span></span> | <span data-ttu-id="fad12-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fad12-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fad12-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fad12-127">Request body</span></span>

<span data-ttu-id="fad12-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fad12-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fad12-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fad12-129">Parameter</span></span>    | <span data-ttu-id="fad12-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="fad12-130">Type</span></span>        | <span data-ttu-id="fad12-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="fad12-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fad12-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="fad12-132">message</span></span>|<span data-ttu-id="fad12-133">String</span><span class="sxs-lookup"><span data-stu-id="fad12-133">String</span></span>|<span data-ttu-id="fad12-134">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="fad12-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="fad12-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad12-135">Response</span></span>

<span data-ttu-id="fad12-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fad12-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fad12-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fad12-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fad12-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fad12-139">Request</span></span>

<span data-ttu-id="fad12-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="fad12-140">The following example shows a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fad12-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="fad12-141">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fad12-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fad12-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fad12-143">C#</span><span class="sxs-lookup"><span data-stu-id="fad12-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fad12-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fad12-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fad12-145">Java</span><span class="sxs-lookup"><span data-stu-id="fad12-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fad12-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="fad12-146">Response</span></span>

<span data-ttu-id="fad12-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="fad12-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response"
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


