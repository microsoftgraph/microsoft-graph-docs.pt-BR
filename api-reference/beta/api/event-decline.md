---
title: 'event: decline'
description: Recusar o convite para o evento específico em um calendário de usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3b6f648d5bbe3adbff5fcfd4f852a2b1c5e75a79
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259231"
---
# <a name="event-decline"></a><span data-ttu-id="2b7fc-103">event: decline</span><span class="sxs-lookup"><span data-stu-id="2b7fc-103">event: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b7fc-104">Recusar o convite para o [evento](../resources/event.md) especificado em um [calendário](../resources/calendar.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-104">Decline invitation to the specified [event](../resources/event.md) in a user [calendar](../resources/calendar.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2b7fc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2b7fc-105">Permissions</span></span>
<span data-ttu-id="2b7fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b7fc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2b7fc-108">Permission type</span></span>      | <span data-ttu-id="2b7fc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2b7fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b7fc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2b7fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2b7fc-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b7fc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2b7fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b7fc-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2b7fc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b7fc-114">Application</span></span> | <span data-ttu-id="2b7fc-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2b7fc-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b7fc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2b7fc-116">HTTP request</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="2b7fc-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fc-117">Request headers</span></span>

| <span data-ttu-id="2b7fc-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2b7fc-118">Name</span></span>       | <span data-ttu-id="2b7fc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b7fc-119">Type</span></span> | <span data-ttu-id="2b7fc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b7fc-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2b7fc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2b7fc-121">Authorization</span></span>  | <span data-ttu-id="2b7fc-122">string</span><span class="sxs-lookup"><span data-stu-id="2b7fc-122">string</span></span>  | <span data-ttu-id="2b7fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b7fc-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2b7fc-125">Content-Type</span></span> | <span data-ttu-id="2b7fc-126">string</span><span class="sxs-lookup"><span data-stu-id="2b7fc-126">string</span></span>  | <span data-ttu-id="2b7fc-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b7fc-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fc-129">Request body</span></span>

<span data-ttu-id="2b7fc-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2b7fc-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2b7fc-131">Parameter</span></span>    | <span data-ttu-id="2b7fc-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b7fc-132">Type</span></span>   |<span data-ttu-id="2b7fc-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b7fc-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b7fc-134">comment</span><span class="sxs-lookup"><span data-stu-id="2b7fc-134">comment</span></span>|<span data-ttu-id="2b7fc-135">String</span><span class="sxs-lookup"><span data-stu-id="2b7fc-135">String</span></span>|<span data-ttu-id="2b7fc-p104">Texto incluído na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p104">Text included in the response. Optional.</span></span>|
|<span data-ttu-id="2b7fc-138">sendResponse</span><span class="sxs-lookup"><span data-stu-id="2b7fc-138">sendResponse</span></span>|<span data-ttu-id="2b7fc-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="2b7fc-139">Boolean</span></span>|<span data-ttu-id="2b7fc-p105">`true` se uma resposta deve ser enviada ao organizador; caso contrário, `false`. Opcional. O padrão é `true`.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p105">`true` if a response is to be sent to the organizer; otherwise, `false`. Optional. Default is `true`.</span></span>|

## <a name="response"></a><span data-ttu-id="2b7fc-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7fc-143">Response</span></span>

<span data-ttu-id="2b7fc-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-p106">If successful, this method returns a `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b7fc-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b7fc-146">Example</span></span>

<span data-ttu-id="2b7fc-147">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-147">Here is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2b7fc-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b7fc-148">Request</span></span>

<span data-ttu-id="2b7fc-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-149">Here is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="2b7fc-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b7fc-150">Response</span></span>

<span data-ttu-id="2b7fc-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b7fc-151">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="2b7fc-152">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2b7fc-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2b7fc-153">C#</span><span class="sxs-lookup"><span data-stu-id="2b7fc-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_decline-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2b7fc-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="2b7fc-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_decline-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2b7fc-155">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2b7fc-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/event_decline-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-decline.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
