---
title: Usar o Outlook para organizar e participar de reuniões online
description: No Outlook, o organizador da reunião pode permitir que os convidados proponham horários alternativos.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e17ffc92ae77324e855452b981e90ee4b4f3f3c5
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353242"
---
# <a name="use-outlook-to-organize-or-attend-meetings-online"></a><span data-ttu-id="da0fb-103">Use o Outlook para organizar ou participar de reuniões online</span><span class="sxs-lookup"><span data-stu-id="da0fb-103">Use Outlook to organize or attend meetings online</span></span>

<span data-ttu-id="da0fb-104">Em uma organização compatível com provedores de reuniões online, os administradores podem configurar os calendários do Outlook para oferecer suporte a reuniões que usam esses provedores, sendo um desses provedores o provedor padrão.</span><span class="sxs-lookup"><span data-stu-id="da0fb-104">In an organization that supports online meeting providers, administrators can set up Outlook calendars to support meetings that use these providers, with one of these providers being the default provider.</span></span> <span data-ttu-id="da0fb-105">Você pode [criar](#create-and-enable-a-meeting-online) ou [atualizar](#update-a-meeting-to-enable-it-online) um [evento](/graph/api/resources/event) no Outlook e permitir que os participantes ingressem na reunião online usando um provedor com suporte.</span><span class="sxs-lookup"><span data-stu-id="da0fb-105">You can [create](#create-and-enable-a-meeting-online) or [update](#update-a-meeting-to-enable-it-online) an [event](/graph/api/resources/event) in Outlook and allow attendees to join the meeting online using a supported provider.</span></span> <span data-ttu-id="da0fb-106">Você pode facilmente [obter as informações da reunião online](#get-information-to-join-meeting-online) do **evento**, incluindo a URL para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="da0fb-106">You can conveniently [get the online meeting information](#get-information-to-join-meeting-online) of the **event**, including the URL to join the meeting.</span></span> 

## <a name="calendars-and-online-meeting-providers"></a><span data-ttu-id="da0fb-107">Calendários e provedores de reuniões online</span><span class="sxs-lookup"><span data-stu-id="da0fb-107">Calendars and online meeting providers</span></span>

<span data-ttu-id="da0fb-108">Uma organização compatível com qualquer um dos seguintes provedores de reuniões online pode configurar os calendários do Outlook e habilitar a organização de reuniões online:</span><span class="sxs-lookup"><span data-stu-id="da0fb-108">An organization that supports any of the following online meeting providers can set up Outlook calendars and enable organizing meetings online:</span></span>

- <span data-ttu-id="da0fb-109">Microsoft Teams, adquirido como parte de um pacote Office 365 business ou corporativo</span><span class="sxs-lookup"><span data-stu-id="da0fb-109">Microsoft Teams, acquired as part of an Office 365 business or enterprise suite</span></span>
- <span data-ttu-id="da0fb-110">Skype</span><span class="sxs-lookup"><span data-stu-id="da0fb-110">Skype</span></span>
- <span data-ttu-id="da0fb-111">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="da0fb-111">Skype for Business</span></span>

<span data-ttu-id="da0fb-112">Procure as propriedades **allowedOnlineMeetingProviders** e **defaultOnlineMeetingProvider** para verificar se um [calendário](/graph/api/resources/calendar) do Outlook é compatível com os provedores de reuniões online.</span><span class="sxs-lookup"><span data-stu-id="da0fb-112">Look for the **allowedOnlineMeetingProviders** and **defaultOnlineMeetingProvider** properties to verify if an Outlook [calendar](/graph/api/resources/calendar) supports any online meeting providers.</span></span> <span data-ttu-id="da0fb-113">O exemplo a seguir mostra que o calendário padrão do usuário conectado é compatível com dois provedores, Microsoft Teams e Skype for Business, e usa o Microsoft Teams como o provedor de reuniões online padrão.</span><span class="sxs-lookup"><span data-stu-id="da0fb-113">The following example shows the signed-in user's default calendar supports two providers, Microsoft Teams and Skype for Business, and uses Microsoft Teams as the default online meeting provider.</span></span> 

### <a name="example-find-whether-a-calendar-supports-any-online-meeting-provider"></a><span data-ttu-id="da0fb-114">Exemplo: descobrir se um calendário é compatível com um provedor de reuniões online</span><span class="sxs-lookup"><span data-stu-id="da0fb-114">Example: Find whether a calendar supports any online meeting provider</span></span>

#### <a name="request"></a><span data-ttu-id="da0fb-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da0fb-115">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da0fb-116">HTTP</span><span class="sxs-lookup"><span data-stu-id="da0fb-116">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_support_for_online_meeting_providers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="da0fb-117">C#</span><span class="sxs-lookup"><span data-stu-id="da0fb-117">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-support-for-online-meeting-providers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da0fb-118">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da0fb-118">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-support-for-online-meeting-providers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da0fb-119">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da0fb-119">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-support-for-online-meeting-providers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da0fb-120">Java</span><span class="sxs-lookup"><span data-stu-id="da0fb-120">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-support-for-online-meeting-providers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da0fb-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0fb-121">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_calendar_support_for_online_meeting_providers",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAwAGVAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness",
        "skypeForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```

## <a name="create-and-enable-a-meeting-online"></a><span data-ttu-id="da0fb-122">Criar e habilitar uma reunião online</span><span class="sxs-lookup"><span data-stu-id="da0fb-122">Create and enable a meeting online</span></span>

<span data-ttu-id="da0fb-123">Você pode criar uma reunião e permitir que os participantes ingressem na reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores com suporte no calendário pai.</span><span class="sxs-lookup"><span data-stu-id="da0fb-123">You can create a meeting and allow attendees to join the meeting online, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the providers supported by the parent calendar.</span></span> <span data-ttu-id="da0fb-124">O exemplo a seguir criar uma reunião no calendário padrão do usuário conectado e permite que os participantes ingressem na reunião por meio do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="da0fb-124">The following example creates a meeting in the signed-in user's default calendar, and enables attendees to join the meeting via Microsoft Teams.</span></span> <span data-ttu-id="da0fb-125">A resposta inclui um **evento** com as informações da reunião online especificadas na propriedade **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-125">The response includes an **event** with online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="da0fb-126">Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-126">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="da0fb-127">Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.</span><span class="sxs-lookup"><span data-stu-id="da0fb-127">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-create-and-make-meeting-available-as-an-online-meeting"></a><span data-ttu-id="da0fb-128">Exemplo: criar e disponibilizar uma reunião online</span><span class="sxs-lookup"><span data-stu-id="da0fb-128">Example: Create and make meeting available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="da0fb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da0fb-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da0fb-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="da0fb-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_meeting_enable_online"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Prep for customer meeting",
  "body": {
    "contentType": "HTML",
    "content": "Does this time work for you?"
  },
  "start": {
      "dateTime": "2019-11-20T13:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-11-20T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Cordova conference room"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.OnMicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="da0fb-131">C#</span><span class="sxs-lookup"><span data-stu-id="da0fb-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-meeting-enable-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da0fb-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da0fb-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-meeting-enable-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da0fb-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da0fb-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-meeting-enable-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da0fb-134">Java</span><span class="sxs-lookup"><span data-stu-id="da0fb-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-meeting-enable-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da0fb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0fb-135">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "create_meeting_enable_online",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUEsA==\"",
    "id": "AAMkADAAABIGYDZAAA=",
    "createdDateTime": "2019-11-15T01:55:54.8022848Z",
    "lastModifiedDateTime": "2019-11-15T01:55:56.5162924Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUEsA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E0080000000076B29D94B32CD6010000000000000000100000005F31C591C3C328459653D025BD277439",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Prep for customer meeting",
    "bodyPreview": "Does this time work for you?\r\n________________________________________________________________________________\r\nJoin Microsoft Teams Meeting\r\n+1 323-555-0166   United States, Los Angeles (Toll)\r\nConference ID: 291 633 251#\r\nLocal numbers | Reset PIN | Lea",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAABIGYDZAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes this time work for you?\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n<div class=\"me-email-text\" style=\"color:#252424; font-family:'Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif\">\r\n<div style=\"margin-top:24px; margin-bottom:10px\"><a class=\"me-email-headline\" href=\"https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d\" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:18px; font-family:'Segoe UI Semibold','Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif; text-decoration:underline; color:#6264a7\">Join\r\n Microsoft Teams Meeting</a> </div>\r\n<div>\r\n<div><a class=\"me-email-link\" href=\"tel:&#43;1 323-886-7531,,291633251# \" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:14px; text-decoration:none; color:#6264a7\">&#43;1 323-886-7531</a>\r\n<span style=\"font-size:12px\">&nbsp; United States, Los Angeles (Toll) </span></div>\r\n</div>\r\n<div style=\"margin-top:10px; margin-bottom:20px\"><span style=\"font-size:12px\">Conference ID:\r\n</span><span style=\"font-size:14px\">291 633 251# </span></div>\r\n<div style=\"margin-bottom:24px\"><a class=\"me-email-link\" target=\"_blank\" href=\"https://dialin.teams.microsoft.com/1f9a0550-737c-41bd-8c7d-4c81dc1c4070?id=291633251\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">Local\r\n numbers</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://mysettings.lync.com/pstnconferencing\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nReset PIN</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://aka.ms/JoinTeamsMeeting\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nLearn more about Teams</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://teams.microsoft.com/meetingOptions/?organizerId=64339082-ed84-4b0b-b4ab-004ae54f3747&amp;tenantId=98a79ebe-74bf-4e07-a017-7b410848cb32&amp;threadId=19_meeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj@thread.v2&amp;messageId=0&amp;language=en-US\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nMeeting options</a> </div>\r\n<div style=\"font-size:14px; margin-bottom:4px\"></div>\r\n<div style=\"font-size:12px\"></div>\r\n</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-11-20T13:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-11-20T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Cordova conference room",
        "locationType": "default",
        "uniqueId": "Cordova conference room",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Cordova conference room",
            "locationType": "default",
            "uniqueId": "Cordova conference room",
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
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "291633251",
        "tollNumber": "+1 323-555-0166"
    }
}
```

## <a name="get-information-to-join-meeting-online"></a><span data-ttu-id="da0fb-136">Obter informações para participar da reunião online</span><span class="sxs-lookup"><span data-stu-id="da0fb-136">Get information to join meeting online</span></span>

<span data-ttu-id="da0fb-137">Os participantes e os organizadores podem usar a propriedade **isOnlineMeeting** para verificar se um [evento](/graph/api/resources/event) está habilitado para a participação online.</span><span class="sxs-lookup"><span data-stu-id="da0fb-137">Attendees and organizers can use the **isOnlineMeeting** property to verify if an [event](/graph/api/resources/event) is enabled for online participation.</span></span> <span data-ttu-id="da0fb-138">Eles podem usar a propriedade **onlineMeetingProvider** para determinar o provedor de reunião e a propriedade **onlineMeeting** de informações de conexão, incluindo **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-138">They can use the **onlineMeetingProvider** property to determine the meeting provider, and the **onlineMeeting** property for connection information including **joinUrl**.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="da0fb-139">Acesse a URL para entrar em uma reunião usando **joinUrl**, disponível por meio da propriedade **onlineMeeting** do **evento**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-139">Access the URL to join a meeting using **joinUrl**, available via the **onlineMeeting** property of the **event**.</span></span> <span data-ttu-id="da0fb-140">Não use a propriedade **onlineMeetingUrl** do **evento** porque **onlineMeetingUrl** será preterido em breve.</span><span class="sxs-lookup"><span data-stu-id="da0fb-140">Do not use the **onlineMeetingUrl** property of the **event** because **onlineMeetingUrl** will soon be deprecated.</span></span>

### <a name="example-get-online-meeting-information"></a><span data-ttu-id="da0fb-141">Exemplo: obter informações sobre a reunião online</span><span class="sxs-lookup"><span data-stu-id="da0fb-141">Example: Get online meeting information</span></span>

#### <a name="request"></a><span data-ttu-id="da0fb-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da0fb-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da0fb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="da0fb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_online_meeting_info"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGu0AABIGYDZAAA=?$select=isOnlineMeeting,onlineMeetingProvider,onlineMeeting
```
# <a name="c"></a>[<span data-ttu-id="da0fb-144">C#</span><span class="sxs-lookup"><span data-stu-id="da0fb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-online-meeting-info-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da0fb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da0fb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-online-meeting-info-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da0fb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da0fb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-online-meeting-info-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da0fb-147">Java</span><span class="sxs-lookup"><span data-stu-id="da0fb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-online-meeting-info-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da0fb-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0fb-148">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "get_event_online_meeting_info",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(isOnlineMeeting,onlineMeetingProvider,onlineMeeting)/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUExA==\"",
    "id": "AAMkADAGu0AABIGYDZAAA=",
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_ODkyNWFmNGYtZjBjYS00MDdlLTllOWQtN2E3MzJlNjM0ZWRj%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "291633251",
        "tollNumber": "+1 323-555-0166"
    }
}
```


## <a name="update-a-meeting-to-enable-it-online"></a><span data-ttu-id="da0fb-149">Atualizar uma reunião para habilitá-la online</span><span class="sxs-lookup"><span data-stu-id="da0fb-149">Update a meeting to enable it online</span></span>
<span data-ttu-id="da0fb-150">Você pode alterar um **evento** existente para disponibilizá-lo como uma reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores de reuniões online com suporte no calendário pai.</span><span class="sxs-lookup"><span data-stu-id="da0fb-150">You can change an existing **event** to make it available as an online meeting, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the online meeting providers supported by the parent calendar.</span></span> <span data-ttu-id="da0fb-151">A resposta inclui o **evento** atualizado com as informações de reunião online correspondentes especificadas na propriedade **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-151">The response includes the updated **event** with the corresponding online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="da0fb-152">Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="da0fb-152">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="da0fb-153">Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.</span><span class="sxs-lookup"><span data-stu-id="da0fb-153">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-update-a-meeting-to-make-it-available-as-an-online-meeting"></a><span data-ttu-id="da0fb-154">Exemplo: atualizar uma reunião para disponibilizá-la como uma reunião online</span><span class="sxs-lookup"><span data-stu-id="da0fb-154">Example: Update a meeting to make it available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="da0fb-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da0fb-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="da0fb-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="da0fb-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_meeting_online"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/events/AAMkADAGu0AABIGYDaAAA=

{
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="da0fb-157">C#</span><span class="sxs-lookup"><span data-stu-id="da0fb-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-meeting-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da0fb-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da0fb-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-meeting-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da0fb-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da0fb-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-meeting-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da0fb-160">Java</span><span class="sxs-lookup"><span data-stu-id="da0fb-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-meeting-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da0fb-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="da0fb-161">Response</span></span>
<!-- {
  "blockType": "response",
  "name": "update_meeting_online",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 Ok
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUFEA==\"",
    "id": "AAMkADAGu0AABIGYDaAAA=",
    "createdDateTime": "2019-11-15T02:13:38.5558455Z",
    "lastModifiedDateTime": "2019-11-15T02:15:00.0654529Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUFEA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000CD93094B5A9BD501000000000000000010000000A16AF77C6F6C254EA13F69C3B2808B4A",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Price strategy",
    "bodyPreview": "Let's define our strategy.\r\n________________________________________________________________________________\r\nJoin Microsoft Teams Meeting\r\n+1 323-555-0166   United States, Los Angeles (Toll)\r\nConference ID: 275 984 951#\r\nLocal numbers | Reset PIN | Learn",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADAGu0AABIGYDaAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Let's define our strategy.</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n<div class=\"me-email-text\" style=\"color:#252424; font-family:'Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif\">\r\n<div style=\"margin-top:24px; margin-bottom:10px\"><a class=\"me-email-headline\" href=\"https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d\" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:18px; font-family:'Segoe UI Semibold','Segoe UI','Helvetica Neue',Helvetica,Arial,sans-serif; text-decoration:underline; color:#6264a7\">Join\r\n Microsoft Teams Meeting</a> </div>\r\n<div>\r\n<div><a class=\"me-email-link\" href=\"tel:&#43;1 323-886-7531,,275984951# \" target=\"_blank\" rel=\"noreferrer noopener\" style=\"font-size:14px; text-decoration:none; color:#6264a7\">&#43;1 323-886-7531</a>\r\n<span style=\"font-size:12px\">&nbsp; United States, Los Angeles (Toll) </span></div>\r\n</div>\r\n<div style=\"margin-top:10px; margin-bottom:20px\"><span style=\"font-size:12px\">Conference ID:\r\n</span><span style=\"font-size:14px\">275 984 951# </span></div>\r\n<div style=\"margin-bottom:24px\"><a class=\"me-email-link\" target=\"_blank\" href=\"https://dialin.teams.microsoft.com/1f9a0550-737c-41bd-8c7d-4c81dc1c4070?id=275984951\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">Local\r\n numbers</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://mysettings.lync.com/pstnconferencing\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nReset PIN</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://aka.ms/JoinTeamsMeeting\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nLearn more about Teams</a> | <a class=\"me-email-link\" target=\"_blank\" href=\"https://teams.microsoft.com/meetingOptions/?organizerId=64339082-ed84-4b0b-b4ab-004ae54f3747&amp;tenantId=98a79ebe-74bf-4e07-a017-7b410848cb32&amp;threadId=19_meeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi@thread.v2&amp;messageId=0&amp;language=en-US\" rel=\"noreferrer noopener\" style=\"font-size:12px; text-decoration:none; color:#6264a7\">\r\nMeeting options</a> </div>\r\n<div style=\"font-size:14px; margin-bottom:4px\"></div>\r\n<div style=\"font-size:12px\"></div>\r\n</div>\r\n<div style=\"width:100%; height:20px\"><span style=\"white-space:nowrap; color:gray; opacity:.36\">________________________________________________________________________________</span>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-11-18T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-11-19T00:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room Baker",
        "locationType": "conferenceRoom",
        "uniqueId": "Baker@contoso.onmicrosoft.com",
        "uniqueIdType": "directory"
    },
    "locations": [
        {
            "displayName": "Conf Room Baker",
            "locationType": "conferenceRoom",
            "uniqueId": "Baker@contoso.onmicrosoft.com",
            "uniqueIdType": "directory"
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
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NTRkMWViMmEtNzcxNC00OTk3LWJjOTEtYTdhMDU3ZmJhYWFi%40thread.v2/0?context=%7b%22Tid%22%3a%2298a79ebe-74bf-4e07-a017-7b410848cb32%22%2c%22Oid%22%3a%2264339082-ed84-4b0b-b4ab-004ae54f3747%22%7d",
        "conferenceId": "275984951",
        "tollNumber": "+1 323-555-0166"
    }
}
```



## <a name="see-also"></a><span data-ttu-id="da0fb-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="da0fb-162">See also</span></span>
- <span data-ttu-id="da0fb-163">Para obter informações sobre a interoperabilidade do Microsoft Teams com o Office 365, consulte:</span><span class="sxs-lookup"><span data-stu-id="da0fb-163">For information on Microsoft Teams interoperability with Office 365, see:</span></span>
  - [<span data-ttu-id="da0fb-164">Como o Exchange e o Microsoft Teams interagem</span><span class="sxs-lookup"><span data-stu-id="da0fb-164">How Exchange and Microsoft Teams interact</span></span>](/microsoftteams/exchange-teams-interact)
  - [<span data-ttu-id="da0fb-165">Definir suas configurações de coexistência e atualização</span><span class="sxs-lookup"><span data-stu-id="da0fb-165">Setting your coexistence and upgrade settings</span></span>](/microsoftteams/setting-your-coexistence-and-upgrade-settings)
- [<span data-ttu-id="da0fb-166">Escolher uma API no Microsoft Graph para criar e ingressar em reuniões online</span><span class="sxs-lookup"><span data-stu-id="da0fb-166">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
- [<span data-ttu-id="da0fb-167">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="da0fb-167">Finding possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
- [<span data-ttu-id="da0fb-168">Obter informações de disponibilidade de usuários e recursos</span><span class="sxs-lookup"><span data-stu-id="da0fb-168">Getting the free/busy schedule for users and resources</span></span>](outlook-get-free-busy-schedule.md)
- [<span data-ttu-id="da0fb-169">Propor horários de reunião em um calendário do Outlook (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="da0fb-169">Propose meeting times in an Outlook calendar (preview)</span></span>](outlook-calendar-meeting-proposals.md)
- [<span data-ttu-id="da0fb-170">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="da0fb-170">Scheduling repeating appointments as recurring events in Outlook</span></span>](outlook-schedule-recurring-events.md)
