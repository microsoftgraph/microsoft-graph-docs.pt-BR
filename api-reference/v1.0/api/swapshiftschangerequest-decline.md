---
title: 'swapShiftsChangeRequest: recusar'
description: Recusar uma solicitação Shift de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4814fb3ef9d416d6d3bc5be1815b746277a25426
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846181"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="1fcf9-103">swapShiftsChangeRequest: recusar</span><span class="sxs-lookup"><span data-stu-id="1fcf9-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="1fcf9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fcf9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fcf9-105">Recusar um objeto [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="1fcf9-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fcf9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fcf9-106">Permissions</span></span>

<span data-ttu-id="1fcf9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fcf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fcf9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fcf9-109">Permission type</span></span>                        | <span data-ttu-id="1fcf9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fcf9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1fcf9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fcf9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fcf9-112">Schedule. ReadWrite. All, Group. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1fcf9-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="1fcf9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fcf9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fcf9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-114">Not supported.</span></span>                              |
| <span data-ttu-id="1fcf9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fcf9-115">Application</span></span>                            | <span data-ttu-id="1fcf9-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fcf9-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="1fcf9-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1fcf9-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1fcf9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcf9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="1fcf9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcf9-120">Request headers</span></span>

| <span data-ttu-id="1fcf9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1fcf9-121">Name</span></span>          | <span data-ttu-id="1fcf9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcf9-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1fcf9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fcf9-123">Authorization</span></span> | <span data-ttu-id="1fcf9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1fcf9-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="1fcf9-126">Content-type</span></span> | <span data-ttu-id="1fcf9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fcf9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcf9-129">Request body</span></span>

<span data-ttu-id="1fcf9-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1fcf9-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1fcf9-131">Parameter</span></span>    | <span data-ttu-id="1fcf9-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fcf9-132">Type</span></span>        | <span data-ttu-id="1fcf9-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fcf9-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1fcf9-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="1fcf9-134">message</span></span>|<span data-ttu-id="1fcf9-135">String</span><span class="sxs-lookup"><span data-stu-id="1fcf9-135">String</span></span>|<span data-ttu-id="1fcf9-136">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="1fcf9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcf9-137">Response</span></span>

<span data-ttu-id="1fcf9-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1fcf9-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1fcf9-140">Examples</span></span>

<span data-ttu-id="1fcf9-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1fcf9-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fcf9-142">Request</span></span>

<span data-ttu-id="1fcf9-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1fcf9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fcf9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="1fcf9-145">C#</span><span class="sxs-lookup"><span data-stu-id="1fcf9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fcf9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fcf9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fcf9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fcf9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1fcf9-148">Java</span><span class="sxs-lookup"><span data-stu-id="1fcf9-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="1fcf9-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fcf9-149">Response</span></span>

<span data-ttu-id="1fcf9-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1fcf9-150">The following is an example of the response.</span></span>
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
