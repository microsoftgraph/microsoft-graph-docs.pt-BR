---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e72e8cc5149ecad9f60353428b357a725a6d5187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969253"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="22391-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="22391-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="22391-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22391-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22391-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="22391-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22391-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22391-106">Permissions</span></span>

<span data-ttu-id="22391-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22391-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22391-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22391-109">Permission type</span></span>                        | <span data-ttu-id="22391-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22391-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22391-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22391-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22391-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22391-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="22391-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22391-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22391-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22391-114">Not supported.</span></span> |
| <span data-ttu-id="22391-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22391-115">Application</span></span>                            | <span data-ttu-id="22391-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22391-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22391-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22391-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="22391-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22391-118">Request headers</span></span>

| <span data-ttu-id="22391-119">Nome</span><span class="sxs-lookup"><span data-stu-id="22391-119">Name</span></span>          | <span data-ttu-id="22391-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="22391-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="22391-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="22391-121">Authorization</span></span> | <span data-ttu-id="22391-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22391-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22391-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="22391-124">Content-type</span></span> | <span data-ttu-id="22391-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22391-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22391-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22391-127">Request body</span></span>

<span data-ttu-id="22391-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22391-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="22391-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="22391-129">Parameter</span></span>    | <span data-ttu-id="22391-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="22391-130">Type</span></span>        | <span data-ttu-id="22391-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22391-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22391-132">mensagem</span><span class="sxs-lookup"><span data-stu-id="22391-132">message</span></span>|<span data-ttu-id="22391-133">String</span><span class="sxs-lookup"><span data-stu-id="22391-133">String</span></span>|<span data-ttu-id="22391-134">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="22391-134">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="22391-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="22391-135">Response</span></span>

<span data-ttu-id="22391-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22391-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22391-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22391-138">Examples</span></span>

<span data-ttu-id="22391-139">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="22391-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="22391-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22391-140">Request</span></span>

<span data-ttu-id="22391-141">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="22391-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22391-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="22391-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="22391-143">C#</span><span class="sxs-lookup"><span data-stu-id="22391-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22391-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22391-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22391-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22391-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22391-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="22391-146">Response</span></span>

<span data-ttu-id="22391-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22391-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
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


