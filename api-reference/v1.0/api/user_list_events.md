# <a name="list-events"></a><span data-ttu-id="178d1-101">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="178d1-101">List events</span></span>

<span data-ttu-id="178d1-p101">Obtenha uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="178d1-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="178d1-104">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="178d1-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="178d1-105">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar_list_calendarview.md) ou [obtenha as instâncias de um evento](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="178d1-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="178d1-106">Obter eventos do calendário de outro usuário</span><span class="sxs-lookup"><span data-stu-id="178d1-106">Get events in another user's calendar</span></span>

<span data-ttu-id="178d1-107">Se você tiver permissões de aplicativo ou se tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter eventos de calendário de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="178d1-107">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="178d1-108">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="178d1-108">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="178d1-109">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="178d1-109">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="178d1-110">Suponha que outro usuário, Henrique, tenha um calendário compartilhado com Diogo.</span><span class="sxs-lookup"><span data-stu-id="178d1-110">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="178d1-111">Você pode obter os eventos desse calendário compartilhado especificando a ID de usuário de Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="178d1-111">You can get the events in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events
```

<span data-ttu-id="178d1-112">Esse recurso se aplica a todas as operações de eventos GET com suporte para usuários individuais, conforme listado na seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="178d1-112">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="178d1-113">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="178d1-113">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="178d1-114">Se Henrique não tiver compartilhado seu calendário com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="178d1-114">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="178d1-115">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter eventos nos próprios calendários do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="178d1-115">In such cases, specifying a user ID or user principal name only works for getting events in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events
```

<span data-ttu-id="178d1-116">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="178d1-116">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="178d1-117">Pastas de contatos compartilhadas</span><span class="sxs-lookup"><span data-stu-id="178d1-117">Shared contact folders</span></span>
- <span data-ttu-id="178d1-118">Calendários compartilhados</span><span class="sxs-lookup"><span data-stu-id="178d1-118">Shared calendars</span></span>
- <span data-ttu-id="178d1-119">Contatos e eventos em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="178d1-119">Contacts and events in shared folders</span></span>
- <span data-ttu-id="178d1-120">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="178d1-120">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="178d1-121">Esse recurso não está disponível em outras operações para contatos, eventos e suas pastas.</span><span class="sxs-lookup"><span data-stu-id="178d1-121">This capability is not available in other operations for contacts, events, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="178d1-122">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="178d1-122">Support various time zones</span></span>

<span data-ttu-id="178d1-123">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="178d1-123">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="178d1-124">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="178d1-124">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="178d1-p106">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="178d1-p106">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="178d1-128">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="178d1-128">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="178d1-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="178d1-129">Permissions</span></span>
<span data-ttu-id="178d1-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="178d1-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="178d1-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="178d1-132">Permission type</span></span>      | <span data-ttu-id="178d1-133">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="178d1-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="178d1-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="178d1-134">Delegated (work or school account)</span></span> | <span data-ttu-id="178d1-135">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178d1-135">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="178d1-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="178d1-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="178d1-137">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178d1-137">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="178d1-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="178d1-138">Application</span></span> | <span data-ttu-id="178d1-139">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="178d1-139">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="178d1-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="178d1-140">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="178d1-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="178d1-141">Optional query parameters</span></span>
<span data-ttu-id="178d1-142">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="178d1-142">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="178d1-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="178d1-143">Request headers</span></span>
| <span data-ttu-id="178d1-144">Nome</span><span class="sxs-lookup"><span data-stu-id="178d1-144">Name</span></span>       | <span data-ttu-id="178d1-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="178d1-145">Type</span></span> | <span data-ttu-id="178d1-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="178d1-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="178d1-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="178d1-147">Authorization</span></span>  | <span data-ttu-id="178d1-148">string</span><span class="sxs-lookup"><span data-stu-id="178d1-148">string</span></span>  | <span data-ttu-id="178d1-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="178d1-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="178d1-151">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="178d1-151">Prefer: outlook.timezone</span></span> | <span data-ttu-id="178d1-152">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="178d1-152">string</span></span> | <span data-ttu-id="178d1-p109">O fuso horário padrão para eventos na resposta. Opcional.</span><span class="sxs-lookup"><span data-stu-id="178d1-p109">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="178d1-155">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="178d1-155">Request body</span></span>
<span data-ttu-id="178d1-156">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="178d1-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="178d1-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="178d1-157">Response</span></span>

<span data-ttu-id="178d1-158">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="178d1-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="178d1-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="178d1-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="178d1-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="178d1-160">Request</span></span>
<span data-ttu-id="178d1-p110">Este é um exemplo da solicitação. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="178d1-p110">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="178d1-163">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="178d1-163">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="178d1-p111">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="178d1-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="178d1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="178d1-166">Response</span></span>
<span data-ttu-id="178d1-p112">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="178d1-p112">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
