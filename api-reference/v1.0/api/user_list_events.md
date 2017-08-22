# <a name="list-events"></a><span data-ttu-id="562f6-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="562f6-101">List events</span></span>

<span data-ttu-id="562f6-p101">Obtenha uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.</span><span class="sxs-lookup"><span data-stu-id="562f6-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="562f6-104">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="562f6-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="562f6-105">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar_list_calendarview.md) ou [obtenha as instâncias de um evento](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="562f6-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="562f6-106">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="562f6-106">Support various time zones</span></span>

<span data-ttu-id="562f6-107">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="562f6-107">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="562f6-108">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="562f6-108">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="562f6-p102">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="562f6-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="562f6-112">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="562f6-112">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="562f6-113">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="562f6-113">Prerequisites</span></span>
<span data-ttu-id="562f6-114">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.Read; Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="562f6-114">One of the following scopes is required to execute this API: Calendars.Read; Calendars.ReadWrite</span></span>
## <a name="http-request"></a><span data-ttu-id="562f6-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="562f6-115">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="562f6-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="562f6-116">Optional query parameters</span></span>
<span data-ttu-id="562f6-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="562f6-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="562f6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="562f6-118">Request headers</span></span>
| <span data-ttu-id="562f6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="562f6-119">Name</span></span>       | <span data-ttu-id="562f6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="562f6-120">Type</span></span> | <span data-ttu-id="562f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="562f6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="562f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="562f6-122">Authorization</span></span>  | <span data-ttu-id="562f6-123">string</span><span class="sxs-lookup"><span data-stu-id="562f6-123">string</span></span>  | <span data-ttu-id="562f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="562f6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="562f6-126">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="562f6-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="562f6-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="562f6-127">string</span></span> | <span data-ttu-id="562f6-p104">O fuso horário padrão para eventos na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="562f6-p104">The default time zone for events in the response. Optional.</span></span> | 

## <a name="request-body"></a><span data-ttu-id="562f6-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="562f6-130">Request body</span></span>
<span data-ttu-id="562f6-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="562f6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="562f6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="562f6-132">Response</span></span>

<span data-ttu-id="562f6-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="562f6-133">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="562f6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="562f6-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="562f6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="562f6-135">Request</span></span>
<span data-ttu-id="562f6-p105">Veja a seguir um exemplo da solicitação. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="562f6-p105">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="562f6-138">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="562f6-138">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="562f6-p106">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="562f6-p106">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="562f6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="562f6-141">Response</span></span>
<span data-ttu-id="562f6-p107">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="562f6-p107">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
            "location":{
                "displayName":"Assembly Hall"
            },
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Fanny Downs",
                        "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
                    "name":"Fanny Downs",
                    "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
