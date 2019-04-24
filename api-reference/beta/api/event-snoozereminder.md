---
title: 'event: snoozeReminder'
description: Adiar um lembrete para um evento em um calendário de usuário até um novo horário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 15cd83b1af1b68088bd9a789fdeacc88f7d7b3e4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457411"
---
# <a name="event-snoozereminder"></a><span data-ttu-id="2f415-103">event: snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="2f415-103">event: snoozeReminder</span></span>

<span data-ttu-id="2f415-104">Adiar um lembrete para um [evento](../resources/event.md) em um [calendário](../resources/calendar.md) de usuário até um novo horário.</span><span class="sxs-lookup"><span data-stu-id="2f415-104">Postpone a reminder for an [event](../resources/event.md) in a user [calendar](../resources/calendar.md) until a new time.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f415-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2f415-105">Permissions</span></span>
<span data-ttu-id="2f415-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f415-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f415-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f415-108">Permission type</span></span>      | <span data-ttu-id="2f415-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2f415-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f415-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f415-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2f415-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f415-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f415-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f415-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f415-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f415-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2f415-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f415-114">Application</span></span> | <span data-ttu-id="2f415-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2f415-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f415-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f415-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="2f415-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f415-117">Request headers</span></span>
| <span data-ttu-id="2f415-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2f415-118">Name</span></span>       | <span data-ttu-id="2f415-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f415-119">Type</span></span> | <span data-ttu-id="2f415-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f415-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f415-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f415-121">Authorization</span></span>  | <span data-ttu-id="2f415-122">string</span><span class="sxs-lookup"><span data-stu-id="2f415-122">string</span></span>  | <span data-ttu-id="2f415-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f415-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2f415-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f415-125">Content-Type</span></span> | <span data-ttu-id="2f415-126">string</span><span class="sxs-lookup"><span data-stu-id="2f415-126">string</span></span>  | <span data-ttu-id="2f415-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f415-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f415-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f415-129">Request body</span></span>
<span data-ttu-id="2f415-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f415-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2f415-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2f415-131">Parameter</span></span>    | <span data-ttu-id="2f415-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f415-132">Type</span></span>   |<span data-ttu-id="2f415-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f415-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f415-134">newReminderTime</span><span class="sxs-lookup"><span data-stu-id="2f415-134">newReminderTime</span></span>|<span data-ttu-id="2f415-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2f415-135">DateTimeTimeZone</span></span>|<span data-ttu-id="2f415-136">A nova data e hora para disparar o lembrete.</span><span class="sxs-lookup"><span data-stu-id="2f415-136">The new date and time to trigger the reminder.</span></span>|

## <a name="response"></a><span data-ttu-id="2f415-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f415-137">Response</span></span>

<span data-ttu-id="2f415-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f415-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f415-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f415-140">Example</span></span>
<span data-ttu-id="2f415-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2f415-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2f415-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f415-142">Request</span></span>
<span data-ttu-id="2f415-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f415-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="2f415-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f415-144">Response</span></span>
<span data-ttu-id="2f415-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f415-145">Here is an example of the response.</span></span>
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
