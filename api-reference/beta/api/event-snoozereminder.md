---
title: 'event: snoozeReminder'
description: Adie um lembrete para um evento em um calendário do usuário até um novo horário.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 440b46b3cb2bebff8f3586e201a0503edcc59000
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874981"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="a5eb3-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="a5eb3-103">event: snoozeReminder</span></span>

> <span data-ttu-id="a5eb3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5eb3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5eb3-106">Adie um lembrete para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md) do usuário até um novo horário.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-106">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5eb3-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="a5eb3-107">Permissions</span></span>
<span data-ttu-id="a5eb3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5eb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5eb3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5eb3-110">Permission type</span></span>      | <span data-ttu-id="a5eb3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5eb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5eb3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5eb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5eb3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5eb3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5eb3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5eb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5eb3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5eb3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a5eb3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5eb3-116">Application</span></span> | <span data-ttu-id="a5eb3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5eb3-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5eb3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5eb3-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="a5eb3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5eb3-119">Request headers</span></span>
| <span data-ttu-id="a5eb3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5eb3-120">Name</span></span>       | <span data-ttu-id="a5eb3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5eb3-121">Type</span></span> | <span data-ttu-id="a5eb3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5eb3-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5eb3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5eb3-123">Authorization</span></span>  | <span data-ttu-id="a5eb3-124">string</span><span class="sxs-lookup"><span data-stu-id="a5eb3-124">string</span></span>  | <span data-ttu-id="a5eb3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a5eb3-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a5eb3-127">Content-Type</span></span> | <span data-ttu-id="a5eb3-128">string</span><span class="sxs-lookup"><span data-stu-id="a5eb3-128">string</span></span>  | <span data-ttu-id="a5eb3-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5eb3-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5eb3-131">Request body</span></span>
<span data-ttu-id="a5eb3-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a5eb3-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a5eb3-133">Parameter</span></span>    | <span data-ttu-id="a5eb3-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5eb3-134">Type</span></span>   |<span data-ttu-id="a5eb3-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5eb3-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5eb3-136">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="a5eb3-136">newReminderTime</span></span>|<span data-ttu-id="a5eb3-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a5eb3-137">DateTimeTimeZone</span></span>|<span data-ttu-id="a5eb3-138">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-138">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="a5eb3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5eb3-139">Response</span></span>

<span data-ttu-id="a5eb3-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5eb3-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5eb3-142">Example</span></span>
<span data-ttu-id="a5eb3-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-143">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a5eb3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5eb3-144">Request</span></span>
<span data-ttu-id="a5eb3-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-145">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a5eb3-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5eb3-146">Response</span></span>
<span data-ttu-id="a5eb3-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5eb3-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
