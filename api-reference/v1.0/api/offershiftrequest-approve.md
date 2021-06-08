---
title: 'offerShiftRequest: aprovar'
description: Aprovar um objeto offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 370e9399b7f4848209190fb771128a51ac820501
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788070"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="2b9d5-103">offerShiftRequest: aprovar</span><span class="sxs-lookup"><span data-stu-id="2b9d5-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="2b9d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b9d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2b9d5-105">Aprovar um [objeto offerShiftRequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="2b9d5-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b9d5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b9d5-106">Permissions</span></span>

<span data-ttu-id="2b9d5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2b9d5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b9d5-109">Permission type</span></span>                        | <span data-ttu-id="2b9d5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b9d5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2b9d5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b9d5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2b9d5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b9d5-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="2b9d5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b9d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b9d5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-114">Not supported.</span></span> |
| <span data-ttu-id="2b9d5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b9d5-115">Application</span></span>                            | <span data-ttu-id="2b9d5-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b9d5-116">Schedule.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="2b9d5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b9d5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="2b9d5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9d5-118">Request headers</span></span>

| <span data-ttu-id="2b9d5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2b9d5-119">Name</span></span>          | <span data-ttu-id="2b9d5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b9d5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2b9d5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b9d5-121">Authorization</span></span> | <span data-ttu-id="2b9d5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b9d5-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="2b9d5-124">Content-type</span></span> | <span data-ttu-id="2b9d5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b9d5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9d5-127">Request body</span></span>

<span data-ttu-id="2b9d5-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b9d5-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2b9d5-129">Parameter</span></span>    | <span data-ttu-id="2b9d5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b9d5-130">Type</span></span>        | <span data-ttu-id="2b9d5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b9d5-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b9d5-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="2b9d5-132">message</span></span>|<span data-ttu-id="2b9d5-133">String</span><span class="sxs-lookup"><span data-stu-id="2b9d5-133">String</span></span>|<span data-ttu-id="2b9d5-134">Mensagem personalizada enviada na aprovação.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="2b9d5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b9d5-135">Response</span></span>

<span data-ttu-id="2b9d5-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2b9d5-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2b9d5-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2b9d5-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b9d5-139">Request</span></span>

<span data-ttu-id="2b9d5-140">O exemplo a seguir mostra uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b9d5-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b9d5-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="c"></a>[<span data-ttu-id="2b9d5-142">C#</span><span class="sxs-lookup"><span data-stu-id="2b9d5-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b9d5-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b9d5-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b9d5-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b9d5-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b9d5-145">Java</span><span class="sxs-lookup"><span data-stu-id="2b9d5-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="2b9d5-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b9d5-146">Response</span></span>

<span data-ttu-id="2b9d5-147">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="2b9d5-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

