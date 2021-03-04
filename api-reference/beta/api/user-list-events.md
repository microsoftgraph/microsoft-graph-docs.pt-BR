---
title: Listar eventos
description: 'Obtenha uma lista de objetos event no calendário padrão do usuário ou '
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 726fa26ce41571050c94c74165a2898ca767b8d3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433555"
---
# <a name="list-events"></a><span data-ttu-id="02ef6-103">Listar eventos</span><span class="sxs-lookup"><span data-stu-id="02ef6-103">List events</span></span>

<span data-ttu-id="02ef6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02ef6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02ef6-105">Obtenha uma lista de objetos [event](../resources/event.md) no calendário padrão do usuário ou de um calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="02ef6-105">Get a list of [event](../resources/event.md) objects from the user's default calendar or from a specified calendar.</span></span> <span data-ttu-id="02ef6-106">A lista contém reuniões de instância única e reuniões mestres em série.</span><span class="sxs-lookup"><span data-stu-id="02ef6-106">The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="02ef6-107">Para obter instâncias de evento expandidas, [obtenha a visualização de calendário](calendar-list-calendarview.md) ou [obtenha as instâncias de um evento](event-list-instances.md).</span><span class="sxs-lookup"><span data-stu-id="02ef6-107">To get expanded event instances, you can [get the calendar view](calendar-list-calendarview.md), or [get the instances of an event](event-list-instances.md).</span></span>

<span data-ttu-id="02ef6-108">Há dois cenários em que um aplicativo pode encontrar eventos do calendário de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="02ef6-108">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="02ef6-109">Se o aplicativo tem permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="02ef6-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="02ef6-110">Se o aplicativo tem as [permissões](#permissions) delegadas apropriadas de um usuário e o outro usuário compartilhou um calendário com esse usuário ou concedeu acesso delegado ao usuário.</span><span class="sxs-lookup"><span data-stu-id="02ef6-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="02ef6-111">Confira os [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="02ef6-111">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="02ef6-112">Suporte a vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="02ef6-112">Support various time zones</span></span>

<span data-ttu-id="02ef6-113">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-113">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="02ef6-114">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="02ef6-114">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="02ef6-p103">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="02ef6-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="02ef6-118">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="02ef6-118">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="02ef6-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="02ef6-119">Permissions</span></span>
<span data-ttu-id="02ef6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ef6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02ef6-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02ef6-122">Permission type</span></span>      | <span data-ttu-id="02ef6-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02ef6-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02ef6-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02ef6-124">Delegated (work or school account)</span></span> | <span data-ttu-id="02ef6-125">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02ef6-125">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="02ef6-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02ef6-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02ef6-127">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02ef6-127">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="02ef6-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02ef6-128">Application</span></span> | <span data-ttu-id="02ef6-129">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02ef6-129">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="02ef6-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02ef6-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="02ef6-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02ef6-131">Optional query parameters</span></span>
<span data-ttu-id="02ef6-132">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02ef6-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02ef6-133">Request headers</span></span>
| <span data-ttu-id="02ef6-134">Nome</span><span class="sxs-lookup"><span data-stu-id="02ef6-134">Name</span></span>       | <span data-ttu-id="02ef6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="02ef6-135">Type</span></span> | <span data-ttu-id="02ef6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="02ef6-136">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="02ef6-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="02ef6-137">Authorization</span></span>  | <span data-ttu-id="02ef6-138">string</span><span class="sxs-lookup"><span data-stu-id="02ef6-138">string</span></span>  | <span data-ttu-id="02ef6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02ef6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02ef6-141">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="02ef6-141">Prefer: outlook.timezone</span></span> | <span data-ttu-id="02ef6-142">string</span><span class="sxs-lookup"><span data-stu-id="02ef6-142">string</span></span> | <span data-ttu-id="02ef6-143">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="02ef6-144">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="02ef6-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="02ef6-145">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02ef6-145">Optional.</span></span> |
| <span data-ttu-id="02ef6-146">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="02ef6-146">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="02ef6-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="02ef6-147">string</span></span> | <span data-ttu-id="02ef6-148">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="02ef6-148">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="02ef6-149">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="02ef6-149">Values can be "text" or "html".</span></span> <span data-ttu-id="02ef6-150">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="02ef6-150">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="02ef6-151">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="02ef6-151">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="02ef6-152">Opcional.</span><span class="sxs-lookup"><span data-stu-id="02ef6-152">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02ef6-153">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02ef6-153">Request body</span></span>
<span data-ttu-id="02ef6-154">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02ef6-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02ef6-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="02ef6-155">Response</span></span>

<span data-ttu-id="02ef6-156">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-156">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="02ef6-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02ef6-157">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="02ef6-158">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="02ef6-158">Request 1</span></span>
<span data-ttu-id="02ef6-159">O primeiro exemplo obtém todos os eventos do usuário.</span><span class="sxs-lookup"><span data-stu-id="02ef6-159">The first example gets all the user's events.</span></span> <span data-ttu-id="02ef6-160">Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="02ef6-160">It specifies the following:</span></span>

- <span data-ttu-id="02ef6-161">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="02ef6-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="02ef6-p109">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="02ef6-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="02ef6-164">A solicitação não especifica nenhum cabeçalho `Prefer: outlook.body-content-type` para indicar um formato específico para o corpo do evento retornado.</span><span class="sxs-lookup"><span data-stu-id="02ef6-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="02ef6-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="02ef6-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="02ef6-166">C#</span><span class="sxs-lookup"><span data-stu-id="02ef6-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02ef6-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02ef6-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02ef6-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02ef6-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02ef6-169">Java</span><span class="sxs-lookup"><span data-stu-id="02ef6-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="02ef6-170">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="02ef6-170">Response 1</span></span>
<span data-ttu-id="02ef6-171">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-171">Here is an example of the response.</span></span> <span data-ttu-id="02ef6-172">Como nenhum cabeçalho `Prefer: outlook.body-content-type` foi especificado, a propriedade **body** será retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="02ef6-172">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_events",
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
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

##### <a name="request-2"></a><span data-ttu-id="02ef6-173">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="02ef6-173">Request 2</span></span>
<span data-ttu-id="02ef6-174">O segundo exemplo mostra como usar um cabeçalho `Prefer: outlook.body-content-type="text"` para obter a propriedade **body** da mensagem especificada no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="02ef6-174">The second example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified message in text format.</span></span>

<span data-ttu-id="02ef6-175">A solicitação também usa um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="02ef6-175">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="02ef6-176">Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="02ef6-176">Without a `$select` parameter, all of the event properties will be returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="02ef6-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="02ef6-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_events_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text" 
```
# <a name="c"></a>[<span data-ttu-id="02ef6-178">C#</span><span class="sxs-lookup"><span data-stu-id="02ef6-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-events-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02ef6-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02ef6-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-events-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02ef6-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02ef6-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-events-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02ef6-181">Java</span><span class="sxs-lookup"><span data-stu-id="02ef6-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-events-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-2"></a><span data-ttu-id="02ef6-182">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="02ef6-182">Response 2</span></span>
<span data-ttu-id="02ef6-183">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ef6-183">Here is an example of the response.</span></span> <span data-ttu-id="02ef6-184">A propriedade **body** é retornada no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="02ef6-184">The **body** property is returned in text format.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 640

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
