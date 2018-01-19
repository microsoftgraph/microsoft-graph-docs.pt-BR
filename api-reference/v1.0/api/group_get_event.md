# <a name="get-event"></a><span data-ttu-id="27d8d-101">Obter evento</span><span class="sxs-lookup"><span data-stu-id="27d8d-101">Get event</span></span>
<span data-ttu-id="27d8d-102">Obter um objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="27d8d-102">Get an [event](../resources/event.md) instance:</span></span>

## <a name="permissions"></a><span data-ttu-id="27d8d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="27d8d-103">Permissions</span></span>
<span data-ttu-id="27d8d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="27d8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27d8d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27d8d-106">Permission type</span></span>      | <span data-ttu-id="27d8d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27d8d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27d8d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27d8d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="27d8d-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27d8d-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="27d8d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27d8d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27d8d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27d8d-111">Not supported.</span></span>    |
|<span data-ttu-id="27d8d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27d8d-112">Application</span></span> | <span data-ttu-id="27d8d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27d8d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27d8d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27d8d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}
GET /groups/{id}/calendar/events/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="27d8d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27d8d-115">Optional query parameters</span></span>
<span data-ttu-id="27d8d-116">Este método dá suporte a [Parâmetros de consulta OData](../../../concepts/query_parameters.md) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27d8d-116">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27d8d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27d8d-117">Request headers</span></span>
| <span data-ttu-id="27d8d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="27d8d-118">Name</span></span>       | <span data-ttu-id="27d8d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="27d8d-119">Type</span></span> | <span data-ttu-id="27d8d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="27d8d-120">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="27d8d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="27d8d-121">Authorization</span></span>  | <span data-ttu-id="27d8d-122">string</span><span class="sxs-lookup"><span data-stu-id="27d8d-122">string</span></span> | <span data-ttu-id="27d8d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27d8d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27d8d-125">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="27d8d-125">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="27d8d-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27d8d-126">string</span></span> | <span data-ttu-id="27d8d-127">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="27d8d-127">outlook.timezone="Eastern Standard Time". Optional. Use this to specify the time zone for start and end times in the response. If not specified, the response are returned in UTC.</span></span> <span data-ttu-id="27d8d-128">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="27d8d-128">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="27d8d-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27d8d-129">Optional.</span></span> |
| <span data-ttu-id="27d8d-130">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="27d8d-130">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="27d8d-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27d8d-131">string</span></span> | <span data-ttu-id="27d8d-132">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="27d8d-132">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="27d8d-133">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="27d8d-133">Values can be "text" or "html".</span></span> <span data-ttu-id="27d8d-134">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="27d8d-134">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="27d8d-135">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="27d8d-135">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="27d8d-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="27d8d-136">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27d8d-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27d8d-137">Request body</span></span>
<span data-ttu-id="27d8d-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27d8d-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27d8d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d8d-139">Response</span></span>
<span data-ttu-id="27d8d-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27d8d-140">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27d8d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27d8d-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="27d8d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27d8d-142">Request</span></span>
<span data-ttu-id="27d8d-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="27d8d-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="27d8d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="27d8d-144">Response</span></span>
<span data-ttu-id="27d8d-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="27d8d-145">The following is an example of the response.</span></span>
><span data-ttu-id="27d8d-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="27d8d-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="27d8d-147">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27d8d-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1728

{
    "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==",
    "createdDateTime": "2017-07-31T18:58:31.011909Z",
    "lastModifiedDateTime": "2017-07-31T18:58:35.418473Z",
    "changeKey": "xPZF2y46pEiVBni87OnrpgAAAAAJTg==",
    "categories": [],
    "originalStartTimeZone": "Eastern Standard Time",
    "originalEndTimeZone": "Eastern Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B23663002F0AD301000000000000000010000000B7C936D4C2FEC749824EE24B2FD7DA62",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Continuing Education Sync",
    "bodyPreview": "Higher Education Planning.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "seriesMaster",
    "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA%3D%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Higher Education Planning.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3acc89e82c01e349d4998655891d93e12e%40thread.skype/1501527510806?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2017-08-15T14:30:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2017-08-15T15:30:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "HR Taskforce / Benefits"
    },
    "recurrence": {
        "pattern": {
            "type": "weekly",
            "interval": 1,
            "month": 0,
            "dayOfMonth": 0,
            "daysOfWeek": [
                "tuesday",
                "thursday"
            ],
            "firstDayOfWeek": "sunday",
            "index": "first"
        },
        "range": {
            "type": "noEnd",
            "startDate": "2017-08-15",
            "endDate": "0001-01-01",
            "recurrenceTimeZone": "Eastern Standard Time",
            "numberOfOccurrences": 0
        }
    },
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2017-07-31T18:58:34.3298022Z"
            },
            "emailAddress": {
                "name": "Lidia Holloway",
                "address": "LidiaH@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "HR Taskforce",
                "address": "HRTaskforce@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Diego Siciliani",
                "address": "DiegoS@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "HR Taskforce",
            "address": "HRTaskforce@contoso.com"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
