---
title: Obter evento
description: Obtenha as propriedades e relacionamentos do objeto de evento especificado.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ae38881de1d485d9c747c4327da5cb40486cc3eb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719783"
---
# <a name="get-event"></a><span data-ttu-id="a131d-103">Obter evento</span><span class="sxs-lookup"><span data-stu-id="a131d-103">Get event</span></span>

<span data-ttu-id="a131d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a131d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a131d-105">Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="a131d-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="a131d-106">No momento, esta operação retorna corpos de eventos somente no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="a131d-106">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="a131d-107">Existem dois cenários em que um aplicativo pode obter um evento no calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="a131d-107">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="a131d-108">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="a131d-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a131d-109">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a131d-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a131d-110">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="a131d-110">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="a131d-111">Como o recurso **event** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **event**.</span><span class="sxs-lookup"><span data-stu-id="a131d-111">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="a131d-112">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="a131d-112">Support various time zones</span></span>

<span data-ttu-id="a131d-113">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="a131d-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a131d-114">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="a131d-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a131d-p102">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="a131d-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a131d-118">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="a131d-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="a131d-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="a131d-119">Permissions</span></span>
<span data-ttu-id="a131d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a131d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a131d-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a131d-122">Permission type</span></span>      | <span data-ttu-id="a131d-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a131d-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a131d-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a131d-124">Delegated (work or school account)</span></span> | <span data-ttu-id="a131d-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a131d-125">Calendars.Read</span></span>    |
|<span data-ttu-id="a131d-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a131d-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a131d-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a131d-127">Calendars.Read</span></span>    |
|<span data-ttu-id="a131d-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a131d-128">Application</span></span> | <span data-ttu-id="a131d-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a131d-129">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a131d-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a131d-130">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a131d-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a131d-131">Optional query parameters</span></span>
<span data-ttu-id="a131d-132">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a131d-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a131d-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a131d-133">Request headers</span></span>
| <span data-ttu-id="a131d-134">Nome</span><span class="sxs-lookup"><span data-stu-id="a131d-134">Name</span></span>       | <span data-ttu-id="a131d-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="a131d-135">Type</span></span> | <span data-ttu-id="a131d-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="a131d-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="a131d-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="a131d-137">Authorization</span></span>  | <span data-ttu-id="a131d-138">string</span><span class="sxs-lookup"><span data-stu-id="a131d-138">string</span></span> | <span data-ttu-id="a131d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a131d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a131d-141">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a131d-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="a131d-142">string</span><span class="sxs-lookup"><span data-stu-id="a131d-142">string</span></span> | <span data-ttu-id="a131d-143">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="a131d-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a131d-144">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="a131d-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a131d-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a131d-145">Optional.</span></span> |
| <span data-ttu-id="a131d-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a131d-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a131d-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a131d-147">string</span></span> | <span data-ttu-id="a131d-148">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="a131d-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a131d-149">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="a131d-149">Values can be "text" or "html".</span></span> <span data-ttu-id="a131d-150">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="a131d-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a131d-151">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="a131d-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a131d-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a131d-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a131d-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a131d-153">Request body</span></span>
<span data-ttu-id="a131d-154">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a131d-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a131d-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="a131d-155">Response</span></span>

<span data-ttu-id="a131d-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a131d-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a131d-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a131d-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a131d-158">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a131d-158">Request 1</span></span>
<span data-ttu-id="a131d-p107">O primeiro exemplo obtém o evento especificado. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a131d-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="a131d-161">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="a131d-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a131d-p108">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="a131d-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="a131d-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a131d-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGIAAAoZDOFAAA="],
  "name": "get_event"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGIAAAoZDOFAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="a131d-165">C#</span><span class="sxs-lookup"><span data-stu-id="a131d-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a131d-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a131d-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a131d-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a131d-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a131d-168">Java</span><span class="sxs-lookup"><span data-stu-id="a131d-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="a131d-169">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a131d-169">Response 1</span></span>

<span data-ttu-id="a131d-p109">Veja a seguir um exemplo da resposta. A propriedade **body** é retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="a131d-p109">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
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
                "response":"tentativelyAccepted",
                "time":"0001-01-01T00:00:00Z"
            },
            "proposedNewTime": {
                "start": {
                    "dateTime": "2019-08-16T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-08-16T14:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            },
            "emailAddress":{
                "name":"Dana Swope",
                "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
            }
        }
    ],
    "hideAttendees": false,
    "organizer":{
        "emailAddress":{
            "name":"Samantha Booth",
            "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
        }
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="a131d-172">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a131d-172">Request 2</span></span>

<span data-ttu-id="a131d-173">O segundo exemplo mostra como obter um evento que especifica mais de um local.</span><span class="sxs-lookup"><span data-stu-id="a131d-173">The second example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="a131d-174">Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="a131d-174">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="a131d-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="a131d-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADAGAADDdm4NAAA="],
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkADAGAADDdm4NAAA=?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="a131d-176">C#</span><span class="sxs-lookup"><span data-stu-id="a131d-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a131d-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a131d-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a131d-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a131d-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a131d-179">Java</span><span class="sxs-lookup"><span data-stu-id="a131d-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="a131d-180">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a131d-180">Response 2</span></span>
<span data-ttu-id="a131d-181">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a131d-181">Here is an example of the response.</span></span> <span data-ttu-id="a131d-182">A propriedade **locations** inclui detalhes dos três locais para os quais o evento é organizado.</span><span class="sxs-lookup"><span data-stu-id="a131d-182">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="a131d-183">Como a solicitação não especifica um cabeçalho `Prefer: outlook.timezone`, as propriedades **start** e **end** são exibidas no fuso horário UTC padrão.</span><span class="sxs-lookup"><span data-stu-id="a131d-183">Because the request does not specify any `Prefer: outlook.timezone` header, the **start** and **end** properties are displayed in the default UTC time zone.</span></span> 

<span data-ttu-id="a131d-184">O corpo do evento está no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="a131d-184">The event body is in the default HTML format.</span></span>  

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



## <a name="see-also"></a><span data-ttu-id="a131d-185">Confira também</span><span class="sxs-lookup"><span data-stu-id="a131d-185">See also</span></span>

- [<span data-ttu-id="a131d-186">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a131d-186">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a131d-187">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="a131d-187">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a131d-188">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="a131d-188">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
