---
title: Usar o Outlook para organizar e participar de reuniões online
description: No Outlook, o organizador da reunião pode permitir que os convidados proponham horários alternativos.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b1d3a4d5d4f68e3ac28a695d7e832dfed6f1a4d7
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621618"
---
# <a name="use-outlook-to-organize-or-attend-meetings-online-preview"></a>Usar o Outlook para organizar e participar de reuniões online (versão prévia)

Em uma organização compatível com provedores de reuniões online, os administradores podem configurar os calendários do Outlook para oferecer suporte a reuniões que usam esses provedores, sendo um desses provedores o provedor padrão. Você pode [criar](#create-and-enable-a-meeting-online) ou [atualizar](#update-a-meeting-to-enable-it-online) um [evento](/graph/api/resources/event?view=graph-rest-beta) no Outlook e permitir que os participantes ingressem na reunião online usando um provedor com suporte. Você pode facilmente [obter as informações da reunião online](#get-information-to-join-meeting-online) do **evento**, incluindo a URL para participar da reunião. 

## <a name="calendars-and-online-meeting-providers"></a>Calendários e provedores de reuniões online

Uma organização compatível com qualquer um dos seguintes provedores de reuniões online pode configurar os calendários do Outlook e habilitar a organização de reuniões online:

- Microsoft Teams, adquirido como parte de um pacote Office 365 business ou corporativo
- Skype
- Skype for Business

Procure as propriedades **allowedOnlineMeetingProviders** e **defaultOnlineMeetingProvider** para verificar se um [calendário](/graph/api/resources/calendar?view=graph-rest-beta) do Outlook é compatível com os provedores de reuniões online. O exemplo a seguir mostra que o calendário padrão do usuário conectado é compatível com dois provedores, Microsoft Teams e Skype for Business, e usa o Microsoft Teams como o provedor de reuniões online padrão. 

### <a name="example-find-whether-a-calendar-supports-any-online-meeting-provider"></a>Exemplo: descobrir se um calendário é compatível com um provedor de reuniões online

#### <a name="request"></a>Solicitação

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_support_for_online_meeting_providers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-support-for-online-meeting-providers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-support-for-online-meeting-providers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-support-for-online-meeting-providers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAwAGVAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "isDefaultCalendar": true,
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": false,
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

## <a name="create-and-enable-a-meeting-online"></a>Criar e habilitar uma reunião online

Você pode criar uma reunião e permitir que os participantes ingressem na reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores com suporte no calendário pai. O exemplo a seguir criar uma reunião no calendário padrão do usuário conectado e permite que os participantes ingressem na reunião por meio do Microsoft Teams. A resposta inclui um **evento** com as informações da reunião online especificadas na propriedade **onlineMeeting**.

> [!NOTE]
> Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**. Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.

### <a name="example-create-and-make-meeting-available-as-an-online-meeting"></a>Exemplo: criar e disponibilizar uma reunião online

#### <a name="request"></a>Solicitação

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_meeting_enable_online"
}-->

```http
POST https://graph.microsoft.com/beta/me/events
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-meeting-enable-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-meeting-enable-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-meeting-enable-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUEsA==\"",
    "id": "AAMkADAAABIGYDZAAA=",
    "createdDateTime": "2019-11-15T01:55:54.8022848Z",
    "lastModifiedDateTime": "2019-11-15T01:55:56.5162924Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUEsA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E008000000006CF8FDD0579BD501000000000000000010000000A030302E234C194F90824DFA6A17FB61",
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

## <a name="get-information-to-join-meeting-online"></a>Obter informações para participar da reunião online

Os participantes e os organizadores podem usar a propriedade **isOnlineMeeting** para verificar se um [evento](/graph/api/resources/event?view=graph-rest-beta) está habilitado para a participação online. Eles podem usar a propriedade **onlineMeetingProvider** para determinar o provedor de reunião e a propriedade **onlineMeeting** de informações de conexão, incluindo **joinUrl**. 

> [!IMPORTANT]
> Acesse a URL para entrar em uma reunião usando **joinUrl**, disponível por meio da propriedade **onlineMeeting** do **evento**. Não use a propriedade **onlineMeetingUrl** do **evento** porque **onlineMeetingUrl** será preterido em breve.

### <a name="example-get-online-meeting-information"></a>Exemplo: obter informações sobre a reunião online

#### <a name="request"></a>Solicitação

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_online_meeting_info"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGu0AABIGYDZAAA=?$select=isOnlineMeeting,onlineMeetingProvider,onlineMeeting
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-online-meeting-info-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-online-meeting-info-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-online-meeting-info-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events(isOnlineMeeting,onlineMeetingProvider,onlineMeeting)/$entity",
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


## <a name="update-a-meeting-to-enable-it-online"></a>Atualizar uma reunião para habilitá-la online
Você pode alterar um **evento** existente para disponibilizá-lo como uma reunião online, configurando **isOnlineMeeting** para `true` e **onlineMeetingProvider** a um dos provedores de reuniões online com suporte no calendário pai. A resposta inclui o **evento** atualizado com as informações de reunião online correspondentes especificadas na propriedade **onlineMeeting**.

> [!NOTE]
> Depois de habilitar uma reunião online, o Microsoft Graph define as informações da reunião em **onlineMeeting**. Em seguida, você não pode alterar a propriedade **onlineMeetingProvider**, nem configurar **isOnlineMeeting** para `false` para desabilitar a reunião online.

### <a name="example-update-a-meeting-to-make-it-available-as-an-online-meeting"></a>Exemplo: atualizar uma reunião para disponibilizá-la como uma reunião online

#### <a name="request"></a>Solicitação

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_meeting_online"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/events/AAMkADAGu0AABIGYDaAAA=

{
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-meeting-online-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-meeting-online-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-meeting-online-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAASBUFEA==\"",
    "id": "AAMkADAGu0AABIGYDaAAA=",
    "createdDateTime": "2019-11-15T02:13:38.5558455Z",
    "lastModifiedDateTime": "2019-11-15T02:15:00.0654529Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAASBUFEA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000CD93094B5A9BD501000000000000000010000000A16AF77C6F6C254EA13F69C3B2808B4A",
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
        "locationUri": "Baker@contoso.onmicrosoft.com",
        "locationType": "conferenceRoom",
        "uniqueId": "Baker@contoso.onmicrosoft.com",
        "uniqueIdType": "directory",
        "address": {
            "type": "unknown",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {}
    },
    "locations": [
        {
            "displayName": "Conf Room Baker",
            "locationUri": "Baker@contoso.onmicrosoft.com",
            "locationType": "conferenceRoom",
            "uniqueId": "Baker@contoso.onmicrosoft.com",
            "uniqueIdType": "directory",
            "address": {
                "type": "unknown",
                "street": "",
                "city": "",
                "state": "",
                "countryOrRegion": "",
                "postalCode": ""
            },
            "coordinates": {}
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
        },
        {
            "type": "resource",
            "status": {
                "response": "accepted",
                "time": "2019-11-15T02:13:42.6568849Z"
            },
            "emailAddress": {
                "name": "Conf Room Baker",
                "address": "Baker@contoso.onmicrosoft.com"
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



## <a name="see-also"></a>Confira também
- Para saber mais sobre a interoperabilidade do Microsoft Teams com o Office 365, confira [configurações de coexistência e de atualização](https://docs.microsoft.com/microsoftteams/setting-your-coexistence-and-upgrade-settings).
- [Encontrar possíveis horários de reunião no calendário do Outlook](findmeetingtimes-example.md)
- [Obter informações de disponibilidade de usuários e recursos](outlook-get-free-busy-schedule.md)
- [Propor horários de reunião em um calendário do Outlook (versão prévia)](outlook-calendar-meeting-proposals.md)
- [Agendar compromissos repetidos como eventos recorrentes no Outlook](outlook-schedule-recurring-events.md)
