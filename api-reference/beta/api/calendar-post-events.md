---
title: Criar evento
description: Use essa API para criar um novo evento no calendário especificado ou no padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dad5e83e515fbbbcd8f762966d89080f2f662c21
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994918"
---
# <a name="create-event"></a><span data-ttu-id="2c708-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="2c708-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c708-104">Use esta API para criar um novo evento em um calendário.</span><span class="sxs-lookup"><span data-stu-id="2c708-104">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="2c708-105">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2c708-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="2c708-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c708-106">Permissions</span></span>
<span data-ttu-id="2c708-107">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="2c708-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="2c708-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c708-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c708-109">Calendário</span><span class="sxs-lookup"><span data-stu-id="2c708-109">Calendar</span></span> | <span data-ttu-id="2c708-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c708-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c708-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c708-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c708-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c708-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="2c708-113">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="2c708-113">user calendar</span></span> | <span data-ttu-id="2c708-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c708-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="2c708-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c708-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="2c708-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c708-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="2c708-117">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="2c708-117">group calendar</span></span> | <span data-ttu-id="2c708-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c708-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="2c708-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c708-119">Not supported.</span></span> | <span data-ttu-id="2c708-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c708-120">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="2c708-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c708-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="2c708-122">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="2c708-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="2c708-123">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="2c708-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="2c708-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="2c708-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="2c708-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c708-125">Request headers</span></span>
| <span data-ttu-id="2c708-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2c708-126">Header</span></span>       | <span data-ttu-id="2c708-127">Valor</span><span class="sxs-lookup"><span data-stu-id="2c708-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2c708-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c708-128">Authorization</span></span>  | <span data-ttu-id="2c708-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c708-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2c708-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2c708-131">Content-Type</span></span>  | <span data-ttu-id="2c708-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c708-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2c708-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c708-134">Request body</span></span>
<span data-ttu-id="2c708-135">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2c708-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2c708-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c708-136">Response</span></span>

<span data-ttu-id="2c708-137">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c708-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c708-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c708-138">Examples</span></span>

### <a name="example-1-create-an-event-in-a-specific-calendar"></a><span data-ttu-id="2c708-139">Exemplo 1: criar um evento em um calendário específico</span><span class="sxs-lookup"><span data-stu-id="2c708-139">Example 1: Create an event in a specific calendar</span></span>

#### <a name="request"></a><span data-ttu-id="2c708-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c708-140">Request</span></span>
<span data-ttu-id="2c708-141">O exemplo a seguir cria um evento no calendário especificado do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2c708-141">The following example creates an event in the specified calendar of the signed-in user's.</span></span>

<span data-ttu-id="2c708-142">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2c708-142">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2c708-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c708-143">HTTP</span></span>](#tab/http)
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
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c708-144">C#</span><span class="sxs-lookup"><span data-stu-id="2c708-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c708-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c708-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c708-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c708-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c708-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c708-147">Response</span></span>
<span data-ttu-id="2c708-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c708-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="2c708-151">Exemplo 2: criar e habilitar um evento como uma reunião online</span><span class="sxs-lookup"><span data-stu-id="2c708-151">Example 2: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="2c708-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c708-152">Request</span></span>
<span data-ttu-id="2c708-153">O exemplo a seguir cria um evento no calendário especificado do usuário conectado e o habilita como uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="2c708-153">The following example creates an event in the specified calendar of the signed-in user's and enables it as an online meeting.</span></span>

<span data-ttu-id="2c708-154">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="2c708-154">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2c708-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c708-155">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c708-156">C#</span><span class="sxs-lookup"><span data-stu-id="2c708-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c708-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c708-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c708-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c708-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2c708-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c708-159">Response</span></span>
<span data-ttu-id="2c708-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c708-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
