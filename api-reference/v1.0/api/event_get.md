# <a name="get-event"></a><span data-ttu-id="18aba-101">Obter evento</span><span class="sxs-lookup"><span data-stu-id="18aba-101">Get event</span></span>

<span data-ttu-id="18aba-102">Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="18aba-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="18aba-103">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="18aba-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="18aba-104">Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **event**.</span><span class="sxs-lookup"><span data-stu-id="18aba-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="18aba-105">Obter eventos do calendário de outro usuário</span><span class="sxs-lookup"><span data-stu-id="18aba-105">Get events in another user's calendar</span></span>

<span data-ttu-id="18aba-106">Se você tiver permissões de aplicativo ou se tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter eventos de calendário de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="18aba-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="18aba-107">Esta seção se concentra em cenários que envolvem permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="18aba-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="18aba-108">Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo.</span><span class="sxs-lookup"><span data-stu-id="18aba-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="18aba-109">Suponha que outro usuário, Henrique, tenha um calendário compartilhado com Diogo.</span><span class="sxs-lookup"><span data-stu-id="18aba-109">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="18aba-110">Você pode obter um evento no calendário compartilhado especificando a ID de usuário de Henrique (ou nome de entidade de segurança) na consulta de exemplo mostrada abaixo.</span><span class="sxs-lookup"><span data-stu-id="18aba-110">You can get an event in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events/{id}
```

<span data-ttu-id="18aba-111">Esse recurso se aplica a todas as operações de eventos GET com suporte para usuários individuais, conforme listado na seção [Solicitação HTTP](#http-request) abaixo.</span><span class="sxs-lookup"><span data-stu-id="18aba-111">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below .</span></span> <span data-ttu-id="18aba-112">Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.</span><span class="sxs-lookup"><span data-stu-id="18aba-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="18aba-113">Se Henrique não tiver compartilhado seu calendário com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="18aba-113">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="18aba-114">Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter um evento nos próprios calendários do usuário conectado, e a consulta será equivalente a usar o atalho /me:</span><span class="sxs-lookup"><span data-stu-id="18aba-114">In such cases, specifying a user ID or user principal name only works for getting an event in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
```

<span data-ttu-id="18aba-115">Esse recurso só está disponível nas operações GET de:</span><span class="sxs-lookup"><span data-stu-id="18aba-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="18aba-116">Pastas de contatos, calendários e pastas de mensagens compartilhados</span><span class="sxs-lookup"><span data-stu-id="18aba-116">Shared contact folders, calendars, and message folders</span></span> 
- <span data-ttu-id="18aba-117">Contatos, eventos e mensagens em pastas compartilhadas</span><span class="sxs-lookup"><span data-stu-id="18aba-117">Contacts, events, and messages in shared folders</span></span>
- <span data-ttu-id="18aba-118">Os recursos acima em caixas de correio delegadas</span><span class="sxs-lookup"><span data-stu-id="18aba-118">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="18aba-119">Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.</span><span class="sxs-lookup"><span data-stu-id="18aba-119">This capability is not available in other operations for contacts, events, messages, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="18aba-120">Suporte a vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="18aba-120">Support various time zones</span></span>

<span data-ttu-id="18aba-121">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="18aba-121">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="18aba-122">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="18aba-122">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="18aba-p105">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="18aba-p105">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="18aba-126">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="18aba-126">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="18aba-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="18aba-127">Permissions</span></span>
<span data-ttu-id="18aba-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="18aba-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="18aba-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18aba-130">Permission type</span></span>      | <span data-ttu-id="18aba-131">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18aba-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18aba-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18aba-132">Delegated (work or school account)</span></span> | <span data-ttu-id="18aba-133">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18aba-133">Calendars.Read</span></span>    |
|<span data-ttu-id="18aba-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18aba-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18aba-135">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18aba-135">Calendars.Read</span></span>    |
|<span data-ttu-id="18aba-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18aba-136">Application</span></span> | <span data-ttu-id="18aba-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="18aba-137">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="18aba-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18aba-138">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18aba-139">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="18aba-139">Optional query parameters</span></span>
<span data-ttu-id="18aba-140">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="18aba-140">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="18aba-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18aba-141">Request headers</span></span>
| <span data-ttu-id="18aba-142">Nome</span><span class="sxs-lookup"><span data-stu-id="18aba-142">Name</span></span>       | <span data-ttu-id="18aba-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="18aba-143">Type</span></span> | <span data-ttu-id="18aba-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="18aba-144">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="18aba-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="18aba-145">Authorization</span></span>  | <span data-ttu-id="18aba-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18aba-146">string</span></span> | <span data-ttu-id="18aba-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18aba-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18aba-149">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="18aba-149">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="18aba-150">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18aba-150">string</span></span> | <span data-ttu-id="18aba-151">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="18aba-151">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="18aba-152">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="18aba-152">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="18aba-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18aba-153">Optional.</span></span> |
| <span data-ttu-id="18aba-154">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="18aba-154">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="18aba-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18aba-155">string</span></span> | <span data-ttu-id="18aba-156">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="18aba-156">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="18aba-157">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="18aba-157">Values can be "text" or "html".</span></span> <span data-ttu-id="18aba-158">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="18aba-158">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="18aba-159">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="18aba-159">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="18aba-160">Opcional.</span><span class="sxs-lookup"><span data-stu-id="18aba-160">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18aba-161">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18aba-161">Request body</span></span>
<span data-ttu-id="18aba-162">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18aba-162">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18aba-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aba-163">Response</span></span>

<span data-ttu-id="18aba-164">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aba-164">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18aba-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="18aba-165">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="18aba-166">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="18aba-166">Request 1</span></span>
<span data-ttu-id="18aba-p110">O primeiro exemplo obtém o evento especificado. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="18aba-p110">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="18aba-169">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="18aba-169">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="18aba-p111">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="18aba-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response-1"></a><span data-ttu-id="18aba-172">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="18aba-172">Response 1</span></span>

<span data-ttu-id="18aba-p112">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="18aba-p112">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
```


##### <a name="request-2"></a><span data-ttu-id="18aba-175">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="18aba-175">Request 2</span></span>

<span data-ttu-id="18aba-176">O segundo exemplo mostra como obter um evento que especifica mais de um local.</span><span class="sxs-lookup"><span data-stu-id="18aba-176">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="18aba-177">Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="18aba-177">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-2"></a><span data-ttu-id="18aba-178">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="18aba-178">Response 2</span></span>
<span data-ttu-id="18aba-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aba-179">Here is an example of the response.</span></span> <span data-ttu-id="18aba-180">A propriedade **locations** inclui detalhes dos três locais para os quais o evento é organizado.</span><span class="sxs-lookup"><span data-stu-id="18aba-180">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="18aba-181">Como a solicitação não especifica um cabeçalho `Prefer: outlook.timezone`, as propriedades **start** e **end** são exibidas no fuso horário UTC padrão.</span><span class="sxs-lookup"><span data-stu-id="18aba-181">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="18aba-182">O corpo do evento está no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="18aba-182">The event body is in the default HTML format.</span></span>  

<!-- {
  "blockType": "response",
  "name": "get_event_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"UTC"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"UTC"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
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
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```



## <a name="see-also"></a><span data-ttu-id="18aba-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="18aba-183">See also</span></span>

- [<span data-ttu-id="18aba-184">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="18aba-184">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="18aba-185">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="18aba-185">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="18aba-186">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="18aba-186">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
