---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9d2276cf38826f80289cc6b2da1112fa5a320f08
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415761"
---
# <a name="event-decline"></a><span data-ttu-id="5d3e4-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="5d3e4-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d3e4-104">Recusar o convite para o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5d3e4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d3e4-105">Permissions</span></span>
<span data-ttu-id="5d3e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d3e4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d3e4-108">Permission type</span></span>      | <span data-ttu-id="5d3e4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d3e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d3e4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d3e4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5d3e4-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3e4-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d3e4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d3e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d3e4-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3e4-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5d3e4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d3e4-114">Application</span></span> | <span data-ttu-id="5d3e4-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5d3e4-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d3e4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3e4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/events/{id}/decline
POST /users/{id | userPrincipalName}/events/{id}/decline

POST /me/calendar/events/{id}/decline
POST /users/{id | userPrincipalName}/calendar/events/{id}/decline

POST /me/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline

POST /me/calendargroup/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/decline
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="5d3e4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3e4-117">Request headers</span></span>

| <span data-ttu-id="5d3e4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5d3e4-118">Name</span></span>       | <span data-ttu-id="5d3e4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d3e4-119">Type</span></span> | <span data-ttu-id="5d3e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d3e4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d3e4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d3e4-121">Authorization</span></span>  | <span data-ttu-id="5d3e4-122">string</span><span class="sxs-lookup"><span data-stu-id="5d3e4-122">string</span></span>  | <span data-ttu-id="5d3e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5d3e4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d3e4-125">Content-Type</span></span> | <span data-ttu-id="5d3e4-126">string</span><span class="sxs-lookup"><span data-stu-id="5d3e4-126">string</span></span>  | <span data-ttu-id="5d3e4-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d3e4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3e4-129">Request body</span></span>

<span data-ttu-id="5d3e4-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5d3e4-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d3e4-131">Parameter</span></span>    | <span data-ttu-id="5d3e4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d3e4-132">Type</span></span>   |<span data-ttu-id="5d3e4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d3e4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d3e4-134">comment</span><span class="sxs-lookup"><span data-stu-id="5d3e4-134">comment</span></span>|<span data-ttu-id="5d3e4-135">String</span><span class="sxs-lookup"><span data-stu-id="5d3e4-135">String</span></span>|<span data-ttu-id="5d3e4-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="5d3e4-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="5d3e4-138">sendResponse</span></span>|<span data-ttu-id="5d3e4-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="5d3e4-139">Boolean</span></span>|<span data-ttu-id="5d3e4-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="5d3e4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d3e4-143">Response</span></span>

<span data-ttu-id="5d3e4-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d3e4-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d3e4-146">Example</span></span>

<span data-ttu-id="5d3e4-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5d3e4-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5d3e4-148">Request</span></span>

<span data-ttu-id="5d3e4-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-149">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5d3e4-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d3e4-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_decline"
}-->

```http
POST https://graph.microsoft.com/beta/me/events/{id}/decline
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5d3e4-151">C#</span><span class="sxs-lookup"><span data-stu-id="5d3e4-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d3e4-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d3e4-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5d3e4-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5d3e4-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5d3e4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d3e4-154">Response</span></span>

<span data-ttu-id="5d3e4-155">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d3e4-155">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
