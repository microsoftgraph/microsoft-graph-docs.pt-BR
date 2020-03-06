---
title: Criar evento
description: Use essa API para criar um novo evento no calendário especificado ou no padrão.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a78006e5ce1364191ed125f374ff1dc6d774ed6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518788"
---
# <a name="create-event"></a><span data-ttu-id="e0d0f-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="e0d0f-103">Create event</span></span>

<span data-ttu-id="e0d0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0d0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0d0f-105">Use esta API para criar um novo evento em um calendário.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-105">Use this API to create a new event in a calendar.</span></span> <span data-ttu-id="e0d0f-106">O calendário pode ser um para um [usuário](../resources/user.md) ou o calendário padrão de um [grupo](../resources/group.md) do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-106">The calendar can be one for a [user](../resources/user.md), or the default calendar of an Office 365 [group](../resources/group.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e0d0f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0d0f-107">Permissions</span></span>
<span data-ttu-id="e0d0f-108">Dependendo do tipo de calendário em que o evento se encontra e do tipo de permissão (delegada ou aplicativo) solicitada, para chamar essa API é necessário ter umas das seguintes permissões.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-108">Depending on the type of calendar that the event is created in and the permission type (delegated or application) requested, one of the following permissions is required to call this API.</span></span> <span data-ttu-id="e0d0f-109">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0d0f-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0d0f-110">Calendário</span><span class="sxs-lookup"><span data-stu-id="e0d0f-110">Calendar</span></span> | <span data-ttu-id="e0d0f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0d0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0d0f-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0d0f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0d0f-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0d0f-113">Application</span></span> |
|:-----|:-----|:-----|:-----|
| <span data-ttu-id="e0d0f-114">calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="e0d0f-114">user calendar</span></span> | <span data-ttu-id="e0d0f-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0d0f-115">Calendars.ReadWrite</span></span> | <span data-ttu-id="e0d0f-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0d0f-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="e0d0f-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0d0f-117">Calendars.ReadWrite</span></span> |
| <span data-ttu-id="e0d0f-118">calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="e0d0f-118">group calendar</span></span> | <span data-ttu-id="e0d0f-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0d0f-119">Group.ReadWrite.All</span></span> | <span data-ttu-id="e0d0f-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-120">Not supported.</span></span> | <span data-ttu-id="e0d0f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0d0f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0d0f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e0d0f-123">Um [calendar](../resources/calendar.md) padrão de um usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-123">A user's or group's default [calendar](../resources/calendar.md).</span></span>
```http
POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events
POST /groups/{id}/calendar/events
```
<span data-ttu-id="e0d0f-124">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-124">A user's [calendar](../resources/calendar.md) in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events

POST /me/calendarGroup/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
```
<span data-ttu-id="e0d0f-125">Um [calendar](../resources/calendar.md) de um usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-125">A user's [calendar](../resources/calendar.md) in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
POST /me/calendarGroups/{id}/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="e0d0f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0d0f-126">Request headers</span></span>
| <span data-ttu-id="e0d0f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0d0f-127">Header</span></span>       | <span data-ttu-id="e0d0f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="e0d0f-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0d0f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0d0f-129">Authorization</span></span>  | <span data-ttu-id="e0d0f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0d0f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0d0f-132">Content-Type</span></span>  | <span data-ttu-id="e0d0f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0d0f-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0d0f-135">Request body</span></span>
<span data-ttu-id="e0d0f-136">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="e0d0f-136">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0d0f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0d0f-137">Response</span></span>

<span data-ttu-id="e0d0f-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-138">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0d0f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0d0f-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0d0f-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0d0f-140">Request</span></span>
<span data-ttu-id="e0d0f-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-141">Here is an example of the request.</span></span>
<span data-ttu-id="e0d0f-142">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="e0d0f-142">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0d0f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0d0f-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGViNDU7zAAAAAGtlAAA="],
  "name": "create_event_from_calendar"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does mid month work for you?"
  },
  "start": {
      "dateTime": "2019-03-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-03-15T14:00:00",
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
# <a name="c"></a>[<span data-ttu-id="e0d0f-144">C#</span><span class="sxs-lookup"><span data-stu-id="e0d0f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-calendar-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0d0f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0d0f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-calendar-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0d0f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0d0f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-calendar-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0d0f-147">Java</span><span class="sxs-lookup"><span data-stu-id="e0d0f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-calendar-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e0d0f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0d0f-148">Response</span></span>
<span data-ttu-id="e0d0f-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0d0f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('5d8d505c-864f-4804-88c7-4583c966cde8')/calendars('AAMkAGViNDU7zAAAAAGtlAAA%3D')/events/$entity",
    "@odata.etag": "W/\"/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==\"",
    "id": "AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA=",
    "createdDateTime": "2019-02-28T21:17:57.56197Z",
    "lastModifiedDateTime": "2019-02-28T21:17:59.044919Z",
    "changeKey": "/IUUrIl3PkG1JCSsPfU+8wAAGXjEpA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E641B4C",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does mid month work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkAGViNDU7zAAAAA7zAAAZb2ckAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes mid month work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-03-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-03-15T14:00:00.0000000",
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
<!-- {
  "type": "#page.annotation",
  "description": "Create event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
