---
title: Listar eventos
description: 'Obter uma lista de objetos de evento na caixa de correio do usuário. A lista contém único '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 767a0f51878921d5d73ddb86d6b93a6704e5a310
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601868"
---
# <a name="list-events"></a><span data-ttu-id="5faa8-104">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="5faa8-104">List events</span></span>

<span data-ttu-id="5faa8-p102">Obtenha uma lista de objetos [event](../resources/event.md) na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres da série.</span><span class="sxs-lookup"><span data-stu-id="5faa8-p102">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="5faa8-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="5faa8-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="5faa8-108">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5faa8-108">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="5faa8-109">Há dois cenários em que um aplicativo pode encontrar eventos do calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="5faa8-109">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="5faa8-110">Se o aplicativo tem permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="5faa8-110">If the app has application permissions, or,</span></span>
* <span data-ttu-id="5faa8-111">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="5faa8-111">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="5faa8-112">Confira os [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="5faa8-112">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="5faa8-113">Suporte a vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="5faa8-113">Support various time zones</span></span>

<span data-ttu-id="5faa8-114">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="5faa8-114">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="5faa8-115">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="5faa8-115">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="5faa8-p104">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="5faa8-p104">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="5faa8-119">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="5faa8-119">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="5faa8-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="5faa8-120">Permissions</span></span>
<span data-ttu-id="5faa8-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5faa8-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5faa8-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5faa8-123">Permission type</span></span>      | <span data-ttu-id="5faa8-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5faa8-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5faa8-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5faa8-125">Delegated (work or school account)</span></span> | <span data-ttu-id="5faa8-126">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5faa8-126">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5faa8-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5faa8-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5faa8-128">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5faa8-128">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="5faa8-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5faa8-129">Application</span></span> | <span data-ttu-id="5faa8-130">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5faa8-130">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5faa8-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5faa8-131">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="5faa8-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5faa8-132">Optional query parameters</span></span>
<span data-ttu-id="5faa8-133">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5faa8-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5faa8-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5faa8-134">Request headers</span></span>
| <span data-ttu-id="5faa8-135">Nome</span><span class="sxs-lookup"><span data-stu-id="5faa8-135">Name</span></span>       | <span data-ttu-id="5faa8-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="5faa8-136">Type</span></span> | <span data-ttu-id="5faa8-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="5faa8-137">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="5faa8-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="5faa8-138">Authorization</span></span>  | <span data-ttu-id="5faa8-139">string</span><span class="sxs-lookup"><span data-stu-id="5faa8-139">string</span></span> | <span data-ttu-id="5faa8-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5faa8-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5faa8-142">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5faa8-142">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="5faa8-143">string</span><span class="sxs-lookup"><span data-stu-id="5faa8-143">string</span></span> | <span data-ttu-id="5faa8-144">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="5faa8-144">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="5faa8-145">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="5faa8-145">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="5faa8-146">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5faa8-146">Optional.</span></span> |
| <span data-ttu-id="5faa8-147">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="5faa8-147">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="5faa8-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5faa8-148">string</span></span> | <span data-ttu-id="5faa8-149">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="5faa8-149">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="5faa8-150">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="5faa8-150">Values can be "text" or "html".</span></span> <span data-ttu-id="5faa8-151">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="5faa8-151">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="5faa8-152">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="5faa8-152">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="5faa8-153">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5faa8-153">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5faa8-154">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5faa8-154">Request body</span></span>
<span data-ttu-id="5faa8-155">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5faa8-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5faa8-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="5faa8-156">Response</span></span>

<span data-ttu-id="5faa8-157">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5faa8-157">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5faa8-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5faa8-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5faa8-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5faa8-159">Request</span></span>
<span data-ttu-id="5faa8-p109">Este é um exemplo da solicitação. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="5faa8-p109">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="5faa8-162">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="5faa8-162">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="5faa8-p110">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="5faa8-p110">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="5faa8-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="5faa8-165">Response</span></span>
<span data-ttu-id="5faa8-p111">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="5faa8-p111">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5faa8-168">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="5faa8-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5faa8-169">C#</span><span class="sxs-lookup"><span data-stu-id="5faa8-169">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_events-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5faa8-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="5faa8-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_events-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-events.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
