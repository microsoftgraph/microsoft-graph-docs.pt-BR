---
title: 'event: snoozeReminder'
description: Adiar um lembrete para um evento em um calendário de usuário até um novo horário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 45c5c44fa720a1c07267f288087812c70dec40f9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859469"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="ccdde-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="ccdde-103">event: snoozeReminder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccdde-104">Adiar um lembrete para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md) de usuário até um novo horário.</span><span class="sxs-lookup"><span data-stu-id="ccdde-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccdde-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccdde-105">Permissions</span></span>
<span data-ttu-id="ccdde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccdde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccdde-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccdde-108">Permission type</span></span>      | <span data-ttu-id="ccdde-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccdde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccdde-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccdde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ccdde-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccdde-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ccdde-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccdde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccdde-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccdde-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ccdde-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccdde-114">Application</span></span> | <span data-ttu-id="ccdde-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccdde-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccdde-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccdde-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="ccdde-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccdde-117">Request headers</span></span>
| <span data-ttu-id="ccdde-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ccdde-118">Name</span></span>       | <span data-ttu-id="ccdde-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccdde-119">Type</span></span> | <span data-ttu-id="ccdde-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccdde-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ccdde-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccdde-121">Authorization</span></span>  | <span data-ttu-id="ccdde-122">string</span><span class="sxs-lookup"><span data-stu-id="ccdde-122">string</span></span>  | <span data-ttu-id="ccdde-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccdde-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccdde-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ccdde-125">Content-Type</span></span> | <span data-ttu-id="ccdde-126">string</span><span class="sxs-lookup"><span data-stu-id="ccdde-126">string</span></span>  | <span data-ttu-id="ccdde-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccdde-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccdde-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccdde-129">Request body</span></span>
<span data-ttu-id="ccdde-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccdde-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ccdde-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="ccdde-131">Parameter</span></span>    | <span data-ttu-id="ccdde-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccdde-132">Type</span></span>   |<span data-ttu-id="ccdde-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccdde-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ccdde-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="ccdde-134">newReminderTime</span></span>|<span data-ttu-id="ccdde-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ccdde-135">DateTimeTimeZone</span></span>|<span data-ttu-id="ccdde-136">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="ccdde-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="ccdde-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccdde-137">Response</span></span>

<span data-ttu-id="ccdde-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccdde-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccdde-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccdde-140">Example</span></span>
<span data-ttu-id="ccdde-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="ccdde-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ccdde-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccdde-142">Request</span></span>
<span data-ttu-id="ccdde-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccdde-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ccdde-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccdde-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="ccdde-145">C#</span><span class="sxs-lookup"><span data-stu-id="ccdde-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-snoozereminder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ccdde-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="ccdde-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-snoozereminder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ccdde-147">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ccdde-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-snoozereminder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ccdde-148">Java</span><span class="sxs-lookup"><span data-stu-id="ccdde-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-snoozereminder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ccdde-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccdde-149">Response</span></span>
<span data-ttu-id="ccdde-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccdde-150">Here is an example of the response.</span></span>
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
