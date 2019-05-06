---
title: Obter evento
description: Obtenha as propriedades e relacionamentos do objeto de evento especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f457c3392bda3d74c42f4d2340a088c00f2ccdb1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587607"
---
# <a name="get-event"></a><span data-ttu-id="a851a-103">Obter evento</span><span class="sxs-lookup"><span data-stu-id="a851a-103">Get event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a851a-104">Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="a851a-104">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="a851a-105">Existem dois cenários em que um aplicativo pode obter um evento no calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="a851a-105">There are two scenarios where an app can get an event in another user's calendar:</span></span>

* <span data-ttu-id="a851a-106">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="a851a-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a851a-107">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="a851a-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a851a-108">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="a851a-108">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="a851a-109">Como o recurso **event** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **event**.</span><span class="sxs-lookup"><span data-stu-id="a851a-109">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="a851a-110">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="a851a-110">Support various time zones</span></span>

<span data-ttu-id="a851a-111">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="a851a-112">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="a851a-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="a851a-p102">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="a851a-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="a851a-116">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="a851a-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="a851a-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="a851a-117">Permissions</span></span>
<span data-ttu-id="a851a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a851a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a851a-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a851a-120">Permission type</span></span>      | <span data-ttu-id="a851a-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a851a-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a851a-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a851a-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a851a-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a851a-123">Calendars.Read</span></span>    |
|<span data-ttu-id="a851a-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a851a-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a851a-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a851a-125">Calendars.Read</span></span>    |
|<span data-ttu-id="a851a-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a851a-126">Application</span></span> | <span data-ttu-id="a851a-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="a851a-127">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a851a-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a851a-128">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="a851a-129">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a851a-129">Optional query parameters</span></span>
<span data-ttu-id="a851a-130">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a851a-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a851a-131">Request headers</span></span>
| <span data-ttu-id="a851a-132">Nome</span><span class="sxs-lookup"><span data-stu-id="a851a-132">Name</span></span>       | <span data-ttu-id="a851a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a851a-133">Type</span></span> | <span data-ttu-id="a851a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a851a-134">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a851a-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="a851a-135">Authorization</span></span>  | <span data-ttu-id="a851a-136">string</span><span class="sxs-lookup"><span data-stu-id="a851a-136">string</span></span>  | <span data-ttu-id="a851a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a851a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a851a-139">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a851a-139">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a851a-140">string</span><span class="sxs-lookup"><span data-stu-id="a851a-140">string</span></span> | <span data-ttu-id="a851a-141">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a851a-142">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="a851a-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a851a-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a851a-143">Optional.</span></span> |
| <span data-ttu-id="a851a-144">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a851a-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a851a-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a851a-145">string</span></span> | <span data-ttu-id="a851a-146">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="a851a-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="a851a-147">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="a851a-147">Values can be "text" or "html".</span></span> <span data-ttu-id="a851a-148">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="a851a-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a851a-149">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="a851a-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="a851a-150">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a851a-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a851a-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a851a-151">Request body</span></span>
<span data-ttu-id="a851a-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a851a-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a851a-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="a851a-153">Response</span></span>

<span data-ttu-id="a851a-154">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-154">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a851a-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a851a-155">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a851a-156">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a851a-156">Request 1</span></span>
<span data-ttu-id="a851a-p107">O primeiro exemplo obtém o evento especificado. Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a851a-p107">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="a851a-159">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="a851a-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="a851a-p108">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="a851a-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="a851a-162">A solicitação não especifica nenhum cabeçalho `Prefer: outlook.body-content-type` para indicar um formato específico para o corpo do evento retornado.</span><span class="sxs-lookup"><span data-stu-id="a851a-162">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response-1"></a><span data-ttu-id="a851a-163">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a851a-163">Response 1</span></span>
<span data-ttu-id="a851a-164">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-164">Here is an example of the response.</span></span> <span data-ttu-id="a851a-165">Como nenhum cabeçalho `Prefer: outlook.body-content-type` foi especificado, a propriedade **body** será retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="a851a-165">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a851a-166">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a851a-166">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a851a-167">Basic</span><span class="sxs-lookup"><span data-stu-id="a851a-167">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a851a-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a851a-168">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="a851a-169">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a851a-169">Request 2</span></span>
<span data-ttu-id="a851a-170">O segundo exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter a propriedade **Body** do evento especificado no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="a851a-170">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="a851a-171">A solicitação também usa um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="a851a-171">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="a851a-172">Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="a851a-172">Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
##### <a name="response-2"></a><span data-ttu-id="a851a-173">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a851a-173">Response 2</span></span>
<span data-ttu-id="a851a-174">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-174">Here is an example of the response.</span></span> <span data-ttu-id="a851a-175">A propriedade **body** é retornada no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="a851a-175">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "name": "get_event_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 636

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
    "id":"AAMkAGI1AAAoZDOFAAA=",
    "subject":"Orientation ",
    "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
    "body":{
        "contentType":"text",
        "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a851a-176">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a851a-176">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a851a-177">Basic</span><span class="sxs-lookup"><span data-stu-id="a851a-177">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_in_text-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a851a-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a851a-178">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_in_text-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a><span data-ttu-id="a851a-179">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="a851a-179">Request 3</span></span>

<span data-ttu-id="a851a-180">O terceiro exemplo mostra obter um evento que especifica mais de um local.</span><span class="sxs-lookup"><span data-stu-id="a851a-180">The third example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="a851a-181">Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="a851a-181">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
##### <a name="response-3"></a><span data-ttu-id="a851a-182">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="a851a-182">Response 3</span></span>
<span data-ttu-id="a851a-183">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a851a-183">Here is an example of the response.</span></span> <span data-ttu-id="a851a-184">A propriedade **locations** inclui detalhes dos três locais para os quais o evento é organizado.</span><span class="sxs-lookup"><span data-stu-id="a851a-184">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="a851a-185">Como a `Prefer: outlook.timezone` solicitação não especifica nenhum cabeçalho ou `Prefer: outlook.body-content-type` , as propriedades **Start** e **end** são exibidas no fuso horário UTC padrão e o corpo está no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="a851a-185">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,locations)/$entity",
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
        "type":"unknown",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a851a-186">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a851a-186">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a851a-187">Basic</span><span class="sxs-lookup"><span data-stu-id="a851a-187">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_event_multiple_locations-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a851a-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a851a-188">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_event_multiple_locations-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="a851a-189">Confira também</span><span class="sxs-lookup"><span data-stu-id="a851a-189">See also</span></span>

- [<span data-ttu-id="a851a-190">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a851a-190">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a851a-191">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="a851a-191">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a851a-192">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="a851a-192">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
