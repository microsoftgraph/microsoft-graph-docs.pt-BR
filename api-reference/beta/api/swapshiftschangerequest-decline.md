---
title: 'swapShiftsChangeRequest: decline'
description: Recusar uma solicitação de turno de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e94566fa87b9cd86bad56660db979650294ce49
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787187"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="87d71-103">swapShiftsChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="87d71-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="87d71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87d71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87d71-105">Recusar um [objeto swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="87d71-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87d71-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="87d71-106">Permissions</span></span>

<span data-ttu-id="87d71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87d71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87d71-109">Permission type</span></span>                        | <span data-ttu-id="87d71-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87d71-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87d71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87d71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87d71-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87d71-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="87d71-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87d71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87d71-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87d71-114">Not supported.</span></span> |
| <span data-ttu-id="87d71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87d71-115">Application</span></span>                            | <span data-ttu-id="87d71-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87d71-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87d71-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87d71-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="87d71-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87d71-118">Request headers</span></span>

| <span data-ttu-id="87d71-119">Nome</span><span class="sxs-lookup"><span data-stu-id="87d71-119">Name</span></span>          | <span data-ttu-id="87d71-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87d71-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="87d71-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87d71-121">Authorization</span></span> | <span data-ttu-id="87d71-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87d71-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87d71-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="87d71-124">Content-type</span></span> | <span data-ttu-id="87d71-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87d71-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87d71-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87d71-127">Request body</span></span>

<span data-ttu-id="87d71-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d71-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87d71-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="87d71-129">Parameter</span></span>    | <span data-ttu-id="87d71-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="87d71-130">Type</span></span>        | <span data-ttu-id="87d71-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="87d71-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87d71-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="87d71-132">message</span></span>|<span data-ttu-id="87d71-133">String</span><span class="sxs-lookup"><span data-stu-id="87d71-133">String</span></span>|<span data-ttu-id="87d71-134">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="87d71-134">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="87d71-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d71-135">Response</span></span>

<span data-ttu-id="87d71-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87d71-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87d71-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87d71-138">Examples</span></span>

<span data-ttu-id="87d71-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="87d71-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="87d71-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87d71-140">Request</span></span>

<span data-ttu-id="87d71-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d71-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87d71-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="87d71-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="87d71-143">C#</span><span class="sxs-lookup"><span data-stu-id="87d71-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87d71-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87d71-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87d71-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87d71-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87d71-146">Java</span><span class="sxs-lookup"><span data-stu-id="87d71-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87d71-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="87d71-147">Response</span></span>

<span data-ttu-id="87d71-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87d71-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


