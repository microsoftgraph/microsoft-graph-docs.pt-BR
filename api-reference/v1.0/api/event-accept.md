---
title: 'event: accept'
description: Aceite o evento específico em um calendário do usuário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f261a5fa6f8faf4f6d38a2a72dc06e1d1ba6b370
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448330"
---
# <a name="event-accept"></a><span data-ttu-id="811da-103">event: accept</span><span class="sxs-lookup"><span data-stu-id="811da-103">event: accept</span></span>

<span data-ttu-id="811da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="811da-105">Aceite o evento [especificado](../resources/event.md) em um calendário do [usuário.](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="811da-105">Accept the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="811da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="811da-106">Permissions</span></span>
<span data-ttu-id="811da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="811da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="811da-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="811da-109">Permission type</span></span>      | <span data-ttu-id="811da-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="811da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="811da-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="811da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="811da-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="811da-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="811da-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="811da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="811da-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="811da-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="811da-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="811da-115">Application</span></span> | <span data-ttu-id="811da-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="811da-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="811da-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="811da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/accept
POST /users/{id | userPrincipalName}/events/{id}/accept

POST /me/calendar/events/{id}/accept
POST /users/{id | userPrincipalName}/calendar/events/{id}/accept

POST /me/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/accept
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept
```
## <a name="request-headers"></a><span data-ttu-id="811da-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="811da-118">Request headers</span></span>
| <span data-ttu-id="811da-119">Nome</span><span class="sxs-lookup"><span data-stu-id="811da-119">Name</span></span>       | <span data-ttu-id="811da-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="811da-120">Type</span></span> | <span data-ttu-id="811da-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="811da-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="811da-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="811da-122">Authorization</span></span>  | <span data-ttu-id="811da-123">string</span><span class="sxs-lookup"><span data-stu-id="811da-123">string</span></span>  | <span data-ttu-id="811da-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="811da-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="811da-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="811da-126">Content-Type</span></span> | <span data-ttu-id="811da-127">string</span><span class="sxs-lookup"><span data-stu-id="811da-127">string</span></span>  | <span data-ttu-id="811da-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="811da-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="811da-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="811da-130">Request body</span></span>
<span data-ttu-id="811da-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="811da-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="811da-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="811da-132">Parameter</span></span>    | <span data-ttu-id="811da-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="811da-133">Type</span></span>   |<span data-ttu-id="811da-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="811da-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="811da-135">comment</span><span class="sxs-lookup"><span data-stu-id="811da-135">comment</span></span>|<span data-ttu-id="811da-136">String</span><span class="sxs-lookup"><span data-stu-id="811da-136">String</span></span>|<span data-ttu-id="811da-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="811da-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="811da-139">sendResponse</span><span class="sxs-lookup"><span data-stu-id="811da-139">sendResponse</span></span>|<span data-ttu-id="811da-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="811da-140">Boolean</span></span>|<span data-ttu-id="811da-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="811da-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="811da-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="811da-144">Response</span></span>

<span data-ttu-id="811da-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="811da-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="811da-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="811da-147">Example</span></span>
<span data-ttu-id="811da-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="811da-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="811da-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="811da-149">Request</span></span>
<span data-ttu-id="811da-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="811da-150">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="811da-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="811da-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_accept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/accept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="811da-152">C#</span><span class="sxs-lookup"><span data-stu-id="811da-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-accept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="811da-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="811da-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-accept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="811da-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="811da-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-accept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="811da-155">Java</span><span class="sxs-lookup"><span data-stu-id="811da-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-accept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="811da-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="811da-156">Response</span></span>
<span data-ttu-id="811da-157">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="811da-157">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: accept",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

