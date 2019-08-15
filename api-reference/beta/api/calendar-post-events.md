---
title: Criar evento
description: Use essa API para criar um novo evento no calendário especificado ou no padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 042f3fba0f916dc709654b2492cc53834ca7c488
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419108"
---
# <a name="create-event"></a><span data-ttu-id="1ebc9-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="1ebc9-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ebc9-104">Use esta API para criar um novo evento em um calendário.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-104">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="1ebc9-105">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-105">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="1ebc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ebc9-106">Permissions</span></span>
<span data-ttu-id="1ebc9-107">Dependendo do tipo de calendário em que o evento é criado e do tipo de permissão (delegado ou aplicativo) solicitado, uma das seguintes permissões é necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-107">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="1ebc9-108">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ebc9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ebc9-109">Calendário</span><span class="sxs-lookup"><span data-stu-id="1ebc9-109">Calendar</span></span> | <span data-ttu-id="1ebc9-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ebc9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ebc9-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ebc9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ebc9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1ebc9-112">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="1ebc9-113">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="1ebc9-113">user calendar</span></span> | <span data-ttu-id="1ebc9-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ebc9-114">Calendars.ReadWrite</span></span> | <span data-ttu-id="1ebc9-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ebc9-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="1ebc9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ebc9-116">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="1ebc9-117">grupo calendar</span><span class="sxs-lookup"><span data-stu-id="1ebc9-117">group calendar</span></span> | <span data-ttu-id="1ebc9-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ebc9-118">Group.ReadWrite.All</span></span> | <span data-ttu-id="1ebc9-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-119">Not supported.</span></span> | <span data-ttu-id="1ebc9-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-120">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="1ebc9-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ebc9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="1ebc9-122">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-122">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="1ebc9-123">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-123">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="1ebc9-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-124">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="1ebc9-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ebc9-125">Request headers</span></span>
| <span data-ttu-id="1ebc9-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ebc9-126">Header</span></span>       | <span data-ttu-id="1ebc9-127">Valor</span><span class="sxs-lookup"><span data-stu-id="1ebc9-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ebc9-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ebc9-128">Authorization</span></span>  | <span data-ttu-id="1ebc9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1ebc9-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ebc9-131">Content-Type</span></span>  | <span data-ttu-id="1ebc9-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ebc9-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ebc9-134">Request body</span></span>
<span data-ttu-id="1ebc9-135">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1ebc9-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1ebc9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ebc9-136">Response</span></span>

<span data-ttu-id="1ebc9-137">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-137">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ebc9-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ebc9-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ebc9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ebc9-139">Request</span></span>
<span data-ttu-id="1ebc9-140">O exemplo a seguir cria um evento no calendário especificado do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-140">The following example creates an event in the specified calendar of the signed-in user's.</span></span>

<span data-ttu-id="1ebc9-141">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1ebc9-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1ebc9-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ebc9-142">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="1ebc9-143">C#</span><span class="sxs-lookup"><span data-stu-id="1ebc9-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ebc9-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ebc9-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1ebc9-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="1ebc9-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1ebc9-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ebc9-146">Response</span></span>
<span data-ttu-id="1ebc9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ebc9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
