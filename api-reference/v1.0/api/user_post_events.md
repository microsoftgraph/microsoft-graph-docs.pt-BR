# <a name="create-event"></a><span data-ttu-id="b1a16-101">Criar Evento</span><span class="sxs-lookup"><span data-stu-id="b1a16-101">Create Event</span></span>

<span data-ttu-id="b1a16-102">Criar um [evento](../resources/event.md) no calendário padrão do usuário ou em um calendário específico.</span><span class="sxs-lookup"><span data-stu-id="b1a16-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="b1a16-103">É possível especificar o fuso horário para cada hora de início e fim do evento como parte desses valores, já que as propriedades **start** e **end** são do tipo [dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="b1a16-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="b1a16-104">Ao criar o evento, o servidor envia convites para todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="b1a16-104">When the event is created, the server send invitations to all attendees.</span></span>


## <a name="permissions"></a><span data-ttu-id="b1a16-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1a16-105">Permissions</span></span>
<span data-ttu-id="b1a16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b1a16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b1a16-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1a16-108">Permission type</span></span>      | <span data-ttu-id="b1a16-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1a16-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1a16-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1a16-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1a16-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1a16-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1a16-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1a16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1a16-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1a16-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b1a16-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1a16-114">Application</span></span> | <span data-ttu-id="b1a16-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1a16-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1a16-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a16-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="b1a16-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a16-117">Request headers</span></span>
| <span data-ttu-id="b1a16-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1a16-118">Header</span></span>       | <span data-ttu-id="b1a16-119">Valor</span><span class="sxs-lookup"><span data-stu-id="b1a16-119">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="b1a16-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1a16-120">Authorization</span></span>  | <span data-ttu-id="b1a16-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1a16-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1a16-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1a16-123">Content-Type</span></span>  | <span data-ttu-id="b1a16-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1a16-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1a16-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a16-126">Request body</span></span>
<span data-ttu-id="b1a16-127">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b1a16-127">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b1a16-128">Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o evento ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="b1a16-128">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="b1a16-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a16-129">Response</span></span>

<span data-ttu-id="b1a16-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a16-130">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a16-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1a16-131">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b1a16-132">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b1a16-132">Request 1</span></span>
<span data-ttu-id="b1a16-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1a16-133">Here is an example of the request.</span></span> <span data-ttu-id="b1a16-134">Ela usa o cabeçalho da solicitação `Prefer: outlook.timezone` para especificar o fuso horário para as horas de **início** e **fim** na resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a16-134">Here is an example of the request. It uses the `Prefer: outlook.timezone` request header to specify the **start** and **end** times in the response should use that time zone.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="b1a16-135">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b1a16-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="b1a16-136">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b1a16-136">Response 1</span></span>
<span data-ttu-id="b1a16-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1a16-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="b1a16-140">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b1a16-140">Request 2</span></span>
<span data-ttu-id="b1a16-141">O segundo exemplo mostra como criar um evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="b1a16-141">The second example shows how to create a recurring event.</span></span> <span data-ttu-id="b1a16-142">O evento ocorre das 10:00 às 11:00 da manhã, todas as segundas-feiras a partir de 4 de setembro de 2017 até o final do ano.</span><span class="sxs-lookup"><span data-stu-id="b1a16-142">The event occurs from 10:00am to 11:00am, every Monday starting September 4, 2017, through the end of the year.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json

{
  "subject": "Let's go for coffee",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T10:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="b1a16-143">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="b1a16-143">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="b1a16-144">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b1a16-144">Response 2</span></span>
<span data-ttu-id="b1a16-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1a16-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==\"",
    "id":"AAMkADQwMDI5YT",
    "createdDateTime":"2017-10-14T07:37:39.0083072Z",
    "lastModifiedDateTime":"2017-10-14T07:37:40.0239406Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E008000000000068AD4FBF44D301000000000000000010000000CA802EEBDE19CB4AB552714F48C7EEFB",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for coffee",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMDI5YT&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    }
}
```


## <a name="see-also"></a><span data-ttu-id="b1a16-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="b1a16-148">See also</span></span>

- [<span data-ttu-id="b1a16-149">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b1a16-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b1a16-150">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="b1a16-150">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
