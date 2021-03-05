---
title: Habilitar um evento como reunião online no calendário do Outlook
description: Em uma organização que oferece suporte a provedores de reunião online, os administradores podem configurar calendários no Outlook para dar suporte a reuniões que utilizam estes provedores.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 44cdb700a59054fb1e339c080d8909a14cfa8ce3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472346"
---
# <a name="enable-an-event-as-an-online-meeting-in-an-outlook-calendar"></a><span data-ttu-id="3a7ae-103">Habilitar um evento como reunião online no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="3a7ae-103">Enable an event as an online meeting in an Outlook calendar</span></span> 

<span data-ttu-id="3a7ae-104">Utilize a API de calendário do Outlook para organizar um evento em que os convidados da reunião possam clicar em um URL de ingresso e participar da reunião online no Microsoft Teams ou no Skype.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-104">Use the Outlook calendar API to organize an event where meeting invitees can click a join URL, and attend the meeting online in Microsoft Teams or Skype.</span></span>

<span data-ttu-id="3a7ae-105">Em uma organização compatível com provedores de reuniões online, os administradores podem configurar os calendários do Outlook para oferecer suporte a reuniões que usam esses provedores, sendo um desses provedores o provedor padrão.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-105">In an organization that supports online meeting providers, administrators can set up Outlook calendars to support meetings that use these providers, with one of these providers being the default provider.</span></span> <span data-ttu-id="3a7ae-106">Você pode [criar](#create-and-enable-a-meeting-online) ou [atualizar](#update-a-meeting-to-enable-it-online) um [evento](/graph/api/resources/event) no Outlook e permitir que os participantes ingressem na reunião online usando um provedor com suporte.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-106">You can [create](#create-and-enable-a-meeting-online) or [update](#update-a-meeting-to-enable-it-online) an [event](/graph/api/resources/event) in Outlook and allow attendees to join the meeting online using a supported provider.</span></span> <span data-ttu-id="3a7ae-107">Você pode facilmente [obter as informações da reunião online](#get-information-to-join-meeting-online) do **evento**, incluindo a URL para participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-107">You can conveniently [get the online meeting information](#get-information-to-join-meeting-online) of the **event**, including the URL to join the meeting.</span></span> 

> <span data-ttu-id="3a7ae-108">**Observe** A API de calendário permite que você configure convenientemente uma reunião on-line em um calendário no Outlook, onde os participantes podem clicar para ingressar na reunião e continuar sua experiência no Teams ou no Skype.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-108">**Note** The calendar API lets you conveniently set up an online meeting in an Outlook calendar where attendees can click to join the meeting and continue their experience in Teams or Skype.</span></span> <span data-ttu-id="3a7ae-109">Para uma integração mais personalizada e rica com o Teams ou o Skype, use a API de comunicações em nuvem.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-109">For a more customized, richer integration with Teams or Skype, use the cloud communications API.</span></span> <span data-ttu-id="3a7ae-110">Consulte [Escolha uma API no Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-110">See [Choose an API in Microsoft Graph to create and join online meetings](choose-online-meeting-api.md) for more information.</span></span>

## <a name="calendars-and-online-meeting-providers"></a><span data-ttu-id="3a7ae-111">Calendários e provedores de reuniões online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-111">Calendars and online meeting providers</span></span>

<span data-ttu-id="3a7ae-112">Uma organização compatível com qualquer um dos seguintes provedores de reuniões online pode configurar os calendários do Outlook e habilitar a organização de reuniões online:</span><span class="sxs-lookup"><span data-stu-id="3a7ae-112">An organization that supports any of the following online meeting providers can set up Outlook calendars and enable organizing meetings online:</span></span>

- <span data-ttu-id="3a7ae-113">O Microsoft Teams foi adquirido como parte do conjunto Microsoft 365 business ou enterprise</span><span class="sxs-lookup"><span data-stu-id="3a7ae-113">Microsoft Teams, acquired as part of a Microsoft 365 business or enterprise suite</span></span>
- <span data-ttu-id="3a7ae-114">Skype</span><span class="sxs-lookup"><span data-stu-id="3a7ae-114">Skype</span></span>
- <span data-ttu-id="3a7ae-115">O Skype for Business (está sendo [substituído pelo Microsoft Teams](https://www.microsoft.com/microsoft-365/previous-versions/skype-for-business-online))</span><span class="sxs-lookup"><span data-stu-id="3a7ae-115">Skype for Business (which is being [superceded by Microsoft Teams](https://www.microsoft.com/microsoft-365/previous-versions/skype-for-business-online))</span></span>

<span data-ttu-id="3a7ae-116">Procure as propriedades **allowedOnlineMeetingProviders** e **defaultOnlineMeetingProvider** para verificar se um [calendário](/graph/api/resources/calendar) do Outlook é compatível com os provedores de reuniões online.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-116">Look for the **allowedOnlineMeetingProviders** and **defaultOnlineMeetingProvider** properties to verify if an Outlook [calendar](/graph/api/resources/calendar) supports any online meeting providers.</span></span> <span data-ttu-id="3a7ae-117">O exemplo a seguir mostra que o calendário padrão do usuário conectado é compatível com dois provedores, Microsoft Teams e Skype for Business, e usa o Microsoft Teams como o provedor de reuniões online padrão.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-117">The following example shows the signed-in user's default calendar supports two providers, Microsoft Teams and Skype for Business, and uses Microsoft Teams as the default online meeting provider.</span></span> 

### <a name="example-find-whether-a-calendar-supports-any-online-meeting-provider"></a><span data-ttu-id="3a7ae-118">Exemplo: descobrir se um calendário é compatível com um provedor de reuniões online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-118">Example: Find whether a calendar supports any online meeting provider</span></span>

#### <a name="request"></a><span data-ttu-id="3a7ae-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a7ae-119">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3a7ae-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a7ae-120">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_support_for_online_meeting_providers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar
```
# <a name="c"></a>[<span data-ttu-id="3a7ae-121">C#</span><span class="sxs-lookup"><span data-stu-id="3a7ae-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-support-for-online-meeting-providers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a7ae-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a7ae-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-support-for-online-meeting-providers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a7ae-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a7ae-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-support-for-online-meeting-providers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a7ae-124">Java</span><span class="sxs-lookup"><span data-stu-id="3a7ae-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendar-support-for-online-meeting-providers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a7ae-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a7ae-125">Response</span></span>
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

## <a name="create-and-enable-a-meeting-online"></a><span data-ttu-id="3a7ae-126">Criar e habilitar uma reunião online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-126">Create and enable a meeting online</span></span>

<span data-ttu-id="3a7ae-127">Você pode criar uma reunião e permitir que os participantes ingressem na reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores com suporte no calendário pai.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-127">You can create a meeting and allow attendees to join the meeting online, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the providers supported by the parent calendar.</span></span> <span data-ttu-id="3a7ae-128">O exemplo a seguir criar uma reunião no calendário padrão do usuário conectado e permite que os participantes ingressem na reunião por meio do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-128">The following example creates a meeting in the signed-in user's default calendar, and enables attendees to join the meeting via Microsoft Teams.</span></span> <span data-ttu-id="3a7ae-129">A resposta inclui um **evento** com as informações da reunião online especificadas na propriedade **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-129">The response includes an **event** with online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="3a7ae-130">Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-130">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="3a7ae-131">Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-131">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-create-and-make-meeting-available-as-an-online-meeting"></a><span data-ttu-id="3a7ae-132">Exemplo: criar e disponibilizar uma reunião online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-132">Example: Create and make meeting available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="3a7ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a7ae-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3a7ae-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a7ae-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a7ae-135">C#</span><span class="sxs-lookup"><span data-stu-id="3a7ae-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-meeting-enable-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a7ae-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a7ae-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-meeting-enable-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a7ae-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a7ae-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-meeting-enable-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a7ae-138">Java</span><span class="sxs-lookup"><span data-stu-id="3a7ae-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-meeting-enable-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a7ae-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a7ae-139">Response</span></span>
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

## <a name="get-information-to-join-meeting-online"></a><span data-ttu-id="3a7ae-140">Obter informações para participar da reunião online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-140">Get information to join meeting online</span></span>

<span data-ttu-id="3a7ae-141">Os participantes e os organizadores podem usar a propriedade **isOnlineMeeting** para verificar se um [evento](/graph/api/resources/event) está habilitado para a participação online.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-141">Attendees and organizers can use the **isOnlineMeeting** property to verify if an [event](/graph/api/resources/event) is enabled for online participation.</span></span> <span data-ttu-id="3a7ae-142">Eles podem usar a propriedade **onlineMeetingProvider** para determinar o provedor de reunião e a propriedade **onlineMeeting** de informações de conexão, incluindo **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-142">They can use the **onlineMeetingProvider** property to determine the meeting provider, and the **onlineMeeting** property for connection information including **joinUrl**.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="3a7ae-143">Acesse a URL para entrar em uma reunião usando **joinUrl**, disponível por meio da propriedade **onlineMeeting** do **evento**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-143">Access the URL to join a meeting using **joinUrl**, available via the **onlineMeeting** property of the **event**.</span></span> <span data-ttu-id="3a7ae-144">Não use a propriedade **onlineMeetingUrl** do **evento** porque **onlineMeetingUrl** será preterido em breve.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-144">Do not use the **onlineMeetingUrl** property of the **event** because **onlineMeetingUrl** will soon be deprecated.</span></span>

### <a name="example-get-online-meeting-information"></a><span data-ttu-id="3a7ae-145">Exemplo: obter informações sobre a reunião online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-145">Example: Get online meeting information</span></span>

#### <a name="request"></a><span data-ttu-id="3a7ae-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a7ae-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3a7ae-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a7ae-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_online_meeting_info"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGu0AABIGYDZAAA=?$select=isOnlineMeeting,onlineMeetingProvider,onlineMeeting
```
# <a name="c"></a>[<span data-ttu-id="3a7ae-148">C#</span><span class="sxs-lookup"><span data-stu-id="3a7ae-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-online-meeting-info-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a7ae-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a7ae-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-online-meeting-info-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a7ae-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a7ae-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-online-meeting-info-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a7ae-151">Java</span><span class="sxs-lookup"><span data-stu-id="3a7ae-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-online-meeting-info-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a7ae-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a7ae-152">Response</span></span>
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


## <a name="update-a-meeting-to-enable-it-online"></a><span data-ttu-id="3a7ae-153">Atualizar uma reunião para habilitá-la online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-153">Update a meeting to enable it online</span></span>
<span data-ttu-id="3a7ae-154">Você pode alterar um **evento** existente para disponibilizá-lo como uma reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores de reuniões online com suporte no calendário pai.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-154">You can change an existing **event** to make it available as an online meeting, by setting **isOnlineMeeting** to `true`, and **onlineMeetingProvider** to one of the online meeting providers supported by the parent calendar.</span></span> <span data-ttu-id="3a7ae-155">A resposta inclui o **evento** atualizado com as informações de reunião online correspondentes especificadas na propriedade **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-155">The response includes the updated **event** with the corresponding online meeting information specified in the **onlineMeeting** property.</span></span>

> [!NOTE]
> <span data-ttu-id="3a7ae-156">Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-156">Once you enable a meeting online, Microsoft Graph sets the meeting information in **onlineMeeting**.</span></span> <span data-ttu-id="3a7ae-157">Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.</span><span class="sxs-lookup"><span data-stu-id="3a7ae-157">Subsequently, you cannot change the **onlineMeetingProvider** property, nor set **isOnlineMeeting** to `false` to disable the meeting online.</span></span>

### <a name="example-update-a-meeting-to-make-it-available-as-an-online-meeting"></a><span data-ttu-id="3a7ae-158">Exemplo: atualizar uma reunião para disponibilizá-la como uma reunião online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-158">Example: Update a meeting to make it available as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="3a7ae-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a7ae-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3a7ae-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a7ae-160">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3a7ae-161">C#</span><span class="sxs-lookup"><span data-stu-id="3a7ae-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-meeting-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a7ae-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a7ae-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-meeting-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a7ae-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a7ae-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-meeting-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a7ae-164">Java</span><span class="sxs-lookup"><span data-stu-id="3a7ae-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-meeting-online-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a7ae-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a7ae-165">Response</span></span>
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



## <a name="see-also"></a><span data-ttu-id="3a7ae-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="3a7ae-166">See also</span></span>
- <span data-ttu-id="3a7ae-167">Para obter informações sobre a interoperabilidade do Microsoft Teams com o Microsoft 365, consulte:</span><span class="sxs-lookup"><span data-stu-id="3a7ae-167">For information on Microsoft Teams interoperability with Microsoft 365, see:</span></span>
  - [<span data-ttu-id="3a7ae-168">Como interagemo o Exchange e o Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="3a7ae-168">How Exchange and Microsoft Teams interact</span></span>](/microsoftteams/exchange-teams-interact)
  - [<span data-ttu-id="3a7ae-169">Defina suas configurações de coexistência e atualização</span><span class="sxs-lookup"><span data-stu-id="3a7ae-169">Setting your coexistence and upgrade settings</span></span>](/microsoftteams/setting-your-coexistence-and-upgrade-settings)
- [<span data-ttu-id="3a7ae-170">Escolha uma API do Microsoft Graph para criar e participar de reuniões online</span><span class="sxs-lookup"><span data-stu-id="3a7ae-170">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
- [<span data-ttu-id="3a7ae-171">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="3a7ae-171">Finding possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
- [<span data-ttu-id="3a7ae-172">Obter informações de disponibilidade de usuários e recursos</span><span class="sxs-lookup"><span data-stu-id="3a7ae-172">Getting the free/busy schedule for users and resources</span></span>](outlook-get-free-busy-schedule.md)
- [<span data-ttu-id="3a7ae-173">Propor horários de reunião em um calendário do Outlook (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="3a7ae-173">Propose meeting times in an Outlook calendar (preview)</span></span>](outlook-calendar-meeting-proposals.md)
- [<span data-ttu-id="3a7ae-174">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="3a7ae-174">Scheduling repeating appointments as recurring events in Outlook</span></span>](outlook-schedule-recurring-events.md)
