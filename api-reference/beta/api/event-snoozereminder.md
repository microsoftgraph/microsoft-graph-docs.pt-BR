---
title: 'event: snoozeReminder'
description: Adiar um lembrete para um evento em um calendário de usuário até um novo horário.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9082ce27e232e06db7867385942e409dfbbe727d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43365044"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="94634-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="94634-103">event: snoozeReminder</span></span>

<span data-ttu-id="94634-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94634-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94634-105">Adiar um lembrete para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md) de usuário até um novo horário.</span><span class="sxs-lookup"><span data-stu-id="94634-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="94634-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94634-106">Permissions</span></span>
<span data-ttu-id="94634-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94634-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94634-109">Permission type</span></span>      | <span data-ttu-id="94634-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94634-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94634-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94634-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94634-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94634-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94634-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94634-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94634-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94634-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="94634-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94634-115">Application</span></span> | <span data-ttu-id="94634-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="94634-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="94634-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94634-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="94634-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94634-118">Request headers</span></span>
| <span data-ttu-id="94634-119">Nome</span><span class="sxs-lookup"><span data-stu-id="94634-119">Name</span></span>       | <span data-ttu-id="94634-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="94634-120">Type</span></span> | <span data-ttu-id="94634-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94634-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="94634-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94634-122">Authorization</span></span>  | <span data-ttu-id="94634-123">string</span><span class="sxs-lookup"><span data-stu-id="94634-123">string</span></span>  | <span data-ttu-id="94634-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94634-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94634-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94634-126">Content-Type</span></span> | <span data-ttu-id="94634-127">string</span><span class="sxs-lookup"><span data-stu-id="94634-127">string</span></span>  | <span data-ttu-id="94634-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94634-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94634-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94634-130">Request body</span></span>
<span data-ttu-id="94634-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94634-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="94634-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94634-132">Parameter</span></span>    | <span data-ttu-id="94634-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="94634-133">Type</span></span>   |<span data-ttu-id="94634-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="94634-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94634-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="94634-135">newReminderTime</span></span>|<span data-ttu-id="94634-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="94634-136">DateTimeTimeZone</span></span>|<span data-ttu-id="94634-137">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="94634-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="94634-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94634-138">Response</span></span>

<span data-ttu-id="94634-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94634-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94634-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94634-141">Example</span></span>
<span data-ttu-id="94634-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="94634-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="94634-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94634-143">Request</span></span>
<span data-ttu-id="94634-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94634-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94634-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="94634-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/beta/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "2016-10-19T10:37:00Z",
    "timeZone": "timeZone-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="94634-146">C#</span><span class="sxs-lookup"><span data-stu-id="94634-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94634-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94634-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94634-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94634-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94634-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="94634-149">Response</span></span>
<span data-ttu-id="94634-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94634-150">Here is an example of the response.</span></span>
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
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
