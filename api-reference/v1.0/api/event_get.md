# <a name="get-event"></a><span data-ttu-id="b95ee-101">Obter evento</span><span class="sxs-lookup"><span data-stu-id="b95ee-101">Get event</span></span>

<span data-ttu-id="b95ee-102">Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="b95ee-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="b95ee-103">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="b95ee-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="b95ee-104">Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **event**.</span><span class="sxs-lookup"><span data-stu-id="b95ee-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="b95ee-105">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="b95ee-105">Support various time zones</span></span>

<span data-ttu-id="b95ee-106">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="b95ee-106">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="b95ee-107">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="b95ee-107">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="b95ee-p101">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="b95ee-p101">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="b95ee-111">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="b95ee-111">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="b95ee-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="b95ee-112">Permissions</span></span>
<span data-ttu-id="b95ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b95ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b95ee-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b95ee-115">Permission type</span></span>      | <span data-ttu-id="b95ee-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b95ee-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b95ee-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b95ee-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b95ee-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b95ee-118">Calendars.Read</span></span>    |
|<span data-ttu-id="b95ee-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b95ee-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b95ee-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b95ee-120">Calendars.Read</span></span>    |
|<span data-ttu-id="b95ee-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b95ee-121">Application</span></span> | <span data-ttu-id="b95ee-122">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="b95ee-122">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b95ee-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b95ee-123">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="b95ee-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b95ee-124">Optional query parameters</span></span>
<span data-ttu-id="b95ee-125">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b95ee-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b95ee-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ee-126">Request headers</span></span>
| <span data-ttu-id="b95ee-127">Nome</span><span class="sxs-lookup"><span data-stu-id="b95ee-127">Name</span></span>       | <span data-ttu-id="b95ee-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="b95ee-128">Type</span></span> | <span data-ttu-id="b95ee-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="b95ee-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b95ee-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b95ee-130">Authorization</span></span>  | <span data-ttu-id="b95ee-131">string</span><span class="sxs-lookup"><span data-stu-id="b95ee-131">string</span></span>  | <span data-ttu-id="b95ee-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b95ee-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b95ee-134">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="b95ee-134">Prefer: outlook.timezone</span></span> | <span data-ttu-id="b95ee-135">string</span><span class="sxs-lookup"><span data-stu-id="b95ee-135">string</span></span> | <span data-ttu-id="b95ee-136">O fuso horário padrão para eventos na resposta.</span><span class="sxs-lookup"><span data-stu-id="b95ee-136">The default time zone for events in the response.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b95ee-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ee-137">Request body</span></span>
<span data-ttu-id="b95ee-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b95ee-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b95ee-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95ee-139">Response</span></span>

<span data-ttu-id="b95ee-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b95ee-140">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b95ee-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b95ee-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b95ee-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b95ee-142">Request</span></span>
<span data-ttu-id="b95ee-p104">O primeiro exemplo obtém o evento especificado. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="b95ee-p104">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="b95ee-145">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="b95ee-145">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="b95ee-p105">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="b95ee-p105">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="b95ee-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b95ee-148">Response</span></span>

<span data-ttu-id="b95ee-p106">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="b95ee-p106">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
```

## <a name="see-also"></a><span data-ttu-id="b95ee-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="b95ee-151">See also</span></span>

- [<span data-ttu-id="b95ee-152">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="b95ee-152">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="b95ee-153">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="b95ee-153">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
