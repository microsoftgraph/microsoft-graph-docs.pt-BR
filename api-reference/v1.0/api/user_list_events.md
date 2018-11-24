# <a name="list-events"></a><span data-ttu-id="ea600-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="ea600-101">List events</span></span>

<span data-ttu-id="ea600-p101">Obtenha uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="ea600-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="ea600-104">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar_list_calendarview.md) ou [obtenha as instâncias de um evento](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="ea600-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

<span data-ttu-id="ea600-105">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="ea600-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="ea600-106">Há dois cenários onde um aplicativo pode obter eventos no calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="ea600-106">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="ea600-107">Se o aplicativo tem permissões de aplicativo, ou,</span><span class="sxs-lookup"><span data-stu-id="ea600-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="ea600-108">Se o aplicativo tiver apropriada [permissões](#permissions) delegadas de um usuário, e outro usuário compartilhou um calendário com que o usuário ou, tem acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="ea600-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="ea600-109">Consulte os [detalhes e um exemplo](../../../concepts/outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="ea600-109">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="ea600-110">Suporte a vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="ea600-110">Support various time zones</span></span>

<span data-ttu-id="ea600-111">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="ea600-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="ea600-112">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="ea600-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="ea600-p103">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="ea600-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="ea600-116">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="ea600-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea600-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="ea600-117">Permissions</span></span>
<span data-ttu-id="ea600-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ea600-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea600-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea600-120">Permission type</span></span>      | <span data-ttu-id="ea600-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea600-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea600-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea600-122">Delegated (work or school account)</span></span> | <span data-ttu-id="ea600-123">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea600-123">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ea600-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea600-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea600-125">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea600-125">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ea600-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea600-126">Application</span></span> | <span data-ttu-id="ea600-127">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea600-127">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea600-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea600-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea600-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ea600-129">Optional query parameters</span></span>
<span data-ttu-id="ea600-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ea600-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ea600-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea600-131">Request headers</span></span>
| <span data-ttu-id="ea600-132">Nome</span><span class="sxs-lookup"><span data-stu-id="ea600-132">Name</span></span>       | <span data-ttu-id="ea600-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea600-133">Type</span></span> | <span data-ttu-id="ea600-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea600-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="ea600-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea600-135">Authorization</span></span>  | <span data-ttu-id="ea600-136">string</span><span class="sxs-lookup"><span data-stu-id="ea600-136">string</span></span> | <span data-ttu-id="ea600-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea600-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea600-139">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="ea600-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="ea600-140">string</span><span class="sxs-lookup"><span data-stu-id="ea600-140">string</span></span> | <span data-ttu-id="ea600-141">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="ea600-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="ea600-142">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="ea600-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="ea600-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea600-143">Optional.</span></span> |
| <span data-ttu-id="ea600-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="ea600-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="ea600-145">string</span><span class="sxs-lookup"><span data-stu-id="ea600-145">string</span></span> | <span data-ttu-id="ea600-146">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="ea600-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="ea600-147">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="ea600-147">Values can be "text" or "html".</span></span> <span data-ttu-id="ea600-148">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="ea600-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="ea600-149">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="ea600-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="ea600-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea600-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea600-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea600-151">Request body</span></span>
<span data-ttu-id="ea600-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ea600-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea600-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea600-153">Response</span></span>

<span data-ttu-id="ea600-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea600-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea600-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea600-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea600-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea600-156">Request</span></span>
<span data-ttu-id="ea600-p108">Este é um exemplo da solicitação. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ea600-p108">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="ea600-159">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="ea600-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="ea600-p109">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="ea600-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="ea600-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea600-162">Response</span></span>
<span data-ttu-id="ea600-p110">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="ea600-p110">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location": {
                "displayName": "Assembly Hall",
                "locationType": "default",
                "uniqueId": "Assembly Hall",
                "uniqueIdType": "private"
            },
            "locations": [
                {
                    "displayName": "Assembly Hall",
                    "locationType": "default",
                    "uniqueIdType": "unknown"
                }
            ],
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Samantha Booth",
                        "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
