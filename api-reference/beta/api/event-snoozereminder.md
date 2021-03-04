---
title: 'event: snoozeReminder'
description: Adie um lembrete para um evento em um calendário do usuário até uma nova hora.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 835219be8d6cd286c8ed54edac9363800b0cc6f5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436194"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="04eb2-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="04eb2-103">event: snoozeReminder</span></span>

<span data-ttu-id="04eb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04eb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04eb2-105">Adie um lembrete para [um evento](../resources/event.md) em um calendário do [usuário](../resources/calendar.md) até uma nova hora.</span><span class="sxs-lookup"><span data-stu-id="04eb2-105">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="04eb2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="04eb2-106">Permissions</span></span>
<span data-ttu-id="04eb2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04eb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04eb2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04eb2-109">Permission type</span></span>      | <span data-ttu-id="04eb2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04eb2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04eb2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04eb2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04eb2-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04eb2-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="04eb2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04eb2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04eb2-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04eb2-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="04eb2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04eb2-115">Application</span></span> | <span data-ttu-id="04eb2-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04eb2-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04eb2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04eb2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/events/{id}/snoozeReminder

POST /me/calendar/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder

POST /me/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder

POST /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
POST /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder
```
## <a name="request-headers"></a><span data-ttu-id="04eb2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04eb2-118">Request headers</span></span>
| <span data-ttu-id="04eb2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="04eb2-119">Name</span></span>       | <span data-ttu-id="04eb2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="04eb2-120">Type</span></span> | <span data-ttu-id="04eb2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="04eb2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04eb2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="04eb2-122">Authorization</span></span>  | <span data-ttu-id="04eb2-123">string</span><span class="sxs-lookup"><span data-stu-id="04eb2-123">string</span></span>  | <span data-ttu-id="04eb2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04eb2-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="04eb2-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04eb2-126">Content-Type</span></span> | <span data-ttu-id="04eb2-127">string</span><span class="sxs-lookup"><span data-stu-id="04eb2-127">string</span></span>  | <span data-ttu-id="04eb2-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04eb2-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04eb2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04eb2-130">Request body</span></span>
<span data-ttu-id="04eb2-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04eb2-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="04eb2-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="04eb2-132">Parameter</span></span>    | <span data-ttu-id="04eb2-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="04eb2-133">Type</span></span>   |<span data-ttu-id="04eb2-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="04eb2-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04eb2-135">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="04eb2-135">newReminderTime</span></span>|<span data-ttu-id="04eb2-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="04eb2-136">DateTimeTimeZone</span></span>|<span data-ttu-id="04eb2-137">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="04eb2-137">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="04eb2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="04eb2-138">Response</span></span>

<span data-ttu-id="04eb2-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04eb2-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04eb2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04eb2-141">Example</span></span>
<span data-ttu-id="04eb2-142">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="04eb2-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="04eb2-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04eb2-143">Request</span></span>
<span data-ttu-id="04eb2-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04eb2-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04eb2-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="04eb2-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="04eb2-146">C#</span><span class="sxs-lookup"><span data-stu-id="04eb2-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04eb2-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04eb2-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04eb2-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04eb2-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04eb2-149">Java</span><span class="sxs-lookup"><span data-stu-id="04eb2-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-snoozereminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04eb2-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="04eb2-150">Response</span></span>
<span data-ttu-id="04eb2-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04eb2-151">Here is an example of the response.</span></span>
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


