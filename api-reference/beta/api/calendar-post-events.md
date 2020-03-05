---
title: Criar evento
description: Use essa API para criar um novo evento no calendário especificado ou no padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 18664a3698abf29a047c5da93257d29268691a7d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440966"
---
# <a name="create-event"></a><span data-ttu-id="a47a9-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="a47a9-103">Create event</span></span>

<span data-ttu-id="a47a9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a47a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a47a9-105">Use esta API para criar um novo evento em um calendário.</span><span class="sxs-lookup"><span data-stu-id="a47a9-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="a47a9-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="a47a9-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="a47a9-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a47a9-107">Permissions</span></span>
<span data-ttu-id="a47a9-108">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="a47a9-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="a47a9-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a47a9-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a47a9-110">Calendário</span><span class="sxs-lookup"><span data-stu-id="a47a9-110">Calendar</span></span> | <span data-ttu-id="a47a9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a47a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a47a9-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a47a9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a47a9-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a47a9-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="a47a9-114">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="a47a9-114">user calendar</span></span> | <span data-ttu-id="a47a9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a47a9-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="a47a9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a47a9-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="a47a9-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a47a9-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="a47a9-118">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="a47a9-118">group calendar</span></span> | <span data-ttu-id="a47a9-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a47a9-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="a47a9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a47a9-120">Not supported.</span></span> | <span data-ttu-id="a47a9-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a47a9-121">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="a47a9-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a47a9-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="a47a9-123">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="a47a9-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="a47a9-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="a47a9-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="a47a9-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="a47a9-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="a47a9-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a47a9-126">Request headers</span></span>
| <span data-ttu-id="a47a9-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a47a9-127">Header</span></span>       | <span data-ttu-id="a47a9-128">Valor</span><span class="sxs-lookup"><span data-stu-id="a47a9-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a47a9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a47a9-129">Authorization</span></span>  | <span data-ttu-id="a47a9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a47a9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a47a9-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a47a9-132">Content-Type</span></span>  | <span data-ttu-id="a47a9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a47a9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a47a9-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a47a9-135">Request body</span></span>
<span data-ttu-id="a47a9-136">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a47a9-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a47a9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a47a9-137">Response</span></span>

<span data-ttu-id="a47a9-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a47a9-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a47a9-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a47a9-139">Examples</span></span>

### <a name="example-1-create-an-event-in-a-specific-calendar"></a><span data-ttu-id="a47a9-140">Exemplo 1: criar um evento em um calendário específico</span><span class="sxs-lookup"><span data-stu-id="a47a9-140">Example 1: Create an event in a specific calendar</span></span>

#### <a name="request"></a><span data-ttu-id="a47a9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a47a9-141">Request</span></span>
<span data-ttu-id="a47a9-142">O exemplo a seguir cria um evento em um calendário específico e atribui ao evento um valor opcional de **TransactionId** .</span><span class="sxs-lookup"><span data-stu-id="a47a9-142">The following example creates an event in a specific calendar and assigns the event an optional **transactionId** value.</span></span>

<span data-ttu-id="a47a9-143">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a47a9-143">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="a47a9-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a47a9-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="a47a9-145">C#</span><span class="sxs-lookup"><span data-stu-id="a47a9-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a47a9-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a47a9-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a47a9-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a47a9-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a47a9-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a47a9-148">Response</span></span>
<span data-ttu-id="a47a9-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a47a9-149">Here is an example of the response.</span></span> 

><span data-ttu-id="a47a9-150">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a47a9-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a47a9-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a47a9-151">All  the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": false,
    "onlineMeetingProvider": "unknown",
    "onlineMeeting": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    }
}
```

### <a name="example-2-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="a47a9-152">Exemplo 2: criar e habilitar um evento como uma reunião online</span><span class="sxs-lookup"><span data-stu-id="a47a9-152">Example 2: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="a47a9-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a47a9-153">Request</span></span>
<span data-ttu-id="a47a9-154">O exemplo a seguir cria um evento no calendário especificado do usuário conectado e o habilita como uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="a47a9-154">The following example creates an event in the specified calendar of the signed-in user and enables it as an online meeting.</span></span>

<span data-ttu-id="a47a9-155">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a47a9-155">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="a47a9-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a47a9-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU8zAAAAAGtlAAA="],
  "name": "create_event_from_calendar_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars/AAMkAGViNDU8zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does next month work for you?"
  },
  "start": {
      "dateTime": "2019-03-10T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-10T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="a47a9-157">C#</span><span class="sxs-lookup"><span data-stu-id="a47a9-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a47a9-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a47a9-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a47a9-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a47a9-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a47a9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a47a9-160">Response</span></span>
<span data-ttu-id="a47a9-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a47a9-161">Here is an example of the response.</span></span> 

> <span data-ttu-id="a47a9-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a47a9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU8zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA=",
    "createdDateTime": "2019-02-28T21:36:26.7105485Z",
    "lastModifiedDateTime": "2019-02-28T21:36:26.9577227Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjGjw==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200C780DAE",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does next month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZe6CkAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes next month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-10T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-10T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Megan Bowen",
            "address": "MeganB@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
