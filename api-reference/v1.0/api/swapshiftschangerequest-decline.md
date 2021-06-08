---
title: 'swapShiftsChangeRequest: decline'
description: Recusar uma solicitação de turno de troca.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 86ffd631b4fe85b383421ee2a3df7447420ee05f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787531"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="c0a64-103">swapShiftsChangeRequest: decline</span><span class="sxs-lookup"><span data-stu-id="c0a64-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="c0a64-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0a64-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0a64-105">Recusar um [objeto swapShiftsChangeRequest.](../resources/swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0a64-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0a64-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0a64-106">Permissions</span></span>

<span data-ttu-id="c0a64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0a64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0a64-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0a64-109">Permission type</span></span>                        | <span data-ttu-id="c0a64-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0a64-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0a64-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0a64-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0a64-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0a64-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c0a64-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0a64-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0a64-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0a64-114">Not supported.</span></span>                              |
| <span data-ttu-id="c0a64-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0a64-115">Application</span></span>                            | <span data-ttu-id="c0a64-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0a64-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="c0a64-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="c0a64-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c0a64-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="c0a64-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c0a64-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0a64-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="c0a64-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0a64-120">Request headers</span></span>

| <span data-ttu-id="c0a64-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c0a64-121">Name</span></span>          | <span data-ttu-id="c0a64-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0a64-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c0a64-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0a64-123">Authorization</span></span> | <span data-ttu-id="c0a64-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0a64-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0a64-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c0a64-126">Content-type</span></span> | <span data-ttu-id="c0a64-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0a64-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0a64-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0a64-129">Request body</span></span>

<span data-ttu-id="c0a64-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0a64-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c0a64-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c0a64-131">Parameter</span></span>    | <span data-ttu-id="c0a64-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0a64-132">Type</span></span>        | <span data-ttu-id="c0a64-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0a64-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0a64-134">mensagem</span><span class="sxs-lookup"><span data-stu-id="c0a64-134">message</span></span>|<span data-ttu-id="c0a64-135">String</span><span class="sxs-lookup"><span data-stu-id="c0a64-135">String</span></span>|<span data-ttu-id="c0a64-136">Uma mensagem de recusa personalizada.</span><span class="sxs-lookup"><span data-stu-id="c0a64-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="c0a64-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0a64-137">Response</span></span>

<span data-ttu-id="c0a64-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0a64-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0a64-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c0a64-140">Examples</span></span>

<span data-ttu-id="c0a64-141">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c0a64-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c0a64-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0a64-142">Request</span></span>

<span data-ttu-id="c0a64-143">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0a64-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0a64-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0a64-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c0a64-145">C#</span><span class="sxs-lookup"><span data-stu-id="c0a64-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0a64-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0a64-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0a64-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0a64-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0a64-148">Java</span><span class="sxs-lookup"><span data-stu-id="c0a64-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="c0a64-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0a64-149">Response</span></span>

<span data-ttu-id="c0a64-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0a64-150">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

