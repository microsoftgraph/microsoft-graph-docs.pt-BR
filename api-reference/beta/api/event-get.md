---
title: Obter evento
description: Obtenha as propriedades e relacionamentos do objeto de evento especificado.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 44007d0c4b8ad4feaf97cb3940fac388b9cca902
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436222"
---
# <a name="get-event"></a><span data-ttu-id="3d848-103">Obter evento</span><span class="sxs-lookup"><span data-stu-id="3d848-103">Get event</span></span>

<span data-ttu-id="3d848-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d848-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d848-105">Obtenha as propriedades e as relações do objeto [event](../resources/event.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="3d848-105">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="3d848-106">Um aplicativo pode obter um evento no calendário de outro usuário se:</span><span class="sxs-lookup"><span data-stu-id="3d848-106">An app can get an event in another user's calendar if:</span></span>

* <span data-ttu-id="3d848-107">O aplicativo tem permissões de aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d848-107">The app has application permissions</span></span>
* <span data-ttu-id="3d848-108">O aplicativo tem as permissões delegadas [apropriadas](#permissions) de um usuário e outro usuário compartilhou um calendário com esse usuário ou deu acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3d848-108">The app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or has given delegated access to that user.</span></span> <span data-ttu-id="3d848-109">Confira [detalhes e um exemplo](/graph/outlook-get-shared-events-calendars).</span><span class="sxs-lookup"><span data-stu-id="3d848-109">See [details and an example](/graph/outlook-get-shared-events-calendars).</span></span>

<span data-ttu-id="3d848-110">Como o **recurso event** dá suporte a [extensões,](/graph/extensibility-overview)você também pode usar a operação para obter propriedades personalizadas e dados de extensão em uma `GET` instância **de** evento.</span><span class="sxs-lookup"><span data-stu-id="3d848-110">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="3d848-111">Suporte para vários fusos horários</span><span class="sxs-lookup"><span data-stu-id="3d848-111">Support various time zones</span></span>

<span data-ttu-id="3d848-112">Para todas as operações GET que retornam eventos, você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e de término do evento na resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-112">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="3d848-113">Por exemplo, o seguinte cabeçalho `Prefer: outlook.timezone` define as horas de início e de término na resposta como Hora Padrão do Leste.</span><span class="sxs-lookup"><span data-stu-id="3d848-113">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="3d848-p102">Se o evento foi criado em um fuso horário diferente, as horas de início e de término serão ajustadas para o fuso horário especificado no cabeçalho `Prefer`. Veja esta [lista](../resources/datetimetimezone.md) para obter os nomes de fuso horário com suporte. Se o cabeçalho `Prefer: outlook.timezone` não for especificado, as horas de início e de término serão retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="3d848-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="3d848-117">Você pode usar as propriedades **OriginalStartTimeZone** e **OriginalEndTimeZone** no recurso **event** para descobrir o fuso horário usado quando o evento foi criado.</span><span class="sxs-lookup"><span data-stu-id="3d848-117">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d848-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d848-118">Permissions</span></span>
<span data-ttu-id="3d848-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d848-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d848-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d848-121">Permission type</span></span>      | <span data-ttu-id="3d848-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d848-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d848-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d848-123">Delegated (work or school account)</span></span> | <span data-ttu-id="3d848-124">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3d848-124">Calendars.Read</span></span>    |
|<span data-ttu-id="3d848-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d848-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d848-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3d848-126">Calendars.Read</span></span>    |
|<span data-ttu-id="3d848-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d848-127">Application</span></span> | <span data-ttu-id="3d848-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3d848-128">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d848-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d848-129">HTTP request</span></span>
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

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3d848-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d848-130">Optional query parameters</span></span>
<span data-ttu-id="3d848-131">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3d848-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-132">Request headers</span></span>
| <span data-ttu-id="3d848-133">Nome</span><span class="sxs-lookup"><span data-stu-id="3d848-133">Name</span></span>       | <span data-ttu-id="3d848-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d848-134">Type</span></span> | <span data-ttu-id="3d848-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d848-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d848-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d848-136">Authorization</span></span>  | <span data-ttu-id="3d848-137">string</span><span class="sxs-lookup"><span data-stu-id="3d848-137">string</span></span>  | <span data-ttu-id="3d848-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d848-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d848-140">Prefira: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3d848-140">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3d848-141">string</span><span class="sxs-lookup"><span data-stu-id="3d848-141">string</span></span> | <span data-ttu-id="3d848-142">Use isto para especificar o fuso horário para horas de início e término na resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="3d848-143">Se não especificado, esses valores de tempo serão retornados em UTC.</span><span class="sxs-lookup"><span data-stu-id="3d848-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="3d848-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d848-144">Optional.</span></span> |
| <span data-ttu-id="3d848-145">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="3d848-145">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="3d848-146">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d848-146">string</span></span> | <span data-ttu-id="3d848-147">O formato da propriedade **corpo** a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="3d848-147">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="3d848-148">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="3d848-148">Values can be "text" or "html".</span></span> <span data-ttu-id="3d848-149">Um cabeçalho `Preference-Applied` é retornado como confirmação se este cabeçalho `Prefer` for especificado.</span><span class="sxs-lookup"><span data-stu-id="3d848-149">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="3d848-150">Se o cabeçalho não for especificado, a propriedade **corpo** será retornada no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3d848-150">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="3d848-151">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3d848-151">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d848-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-152">Request body</span></span>
<span data-ttu-id="3d848-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d848-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d848-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d848-154">Response</span></span>

<span data-ttu-id="3d848-155">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-155">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="3d848-156">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3d848-156">Examples</span></span>

### <a name="example-1-get-a-specified-event"></a><span data-ttu-id="3d848-157">Exemplo 1: Obter um evento especificado</span><span class="sxs-lookup"><span data-stu-id="3d848-157">Example 1: Get a specified event</span></span>
#### <a name="request"></a><span data-ttu-id="3d848-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-158">Request</span></span>
<span data-ttu-id="3d848-159">O exemplo a seguir obtém o evento especificado.</span><span class="sxs-lookup"><span data-stu-id="3d848-159">The following example gets the specified event.</span></span> <span data-ttu-id="3d848-160">Especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="3d848-160">It specifies the following:</span></span>

- <span data-ttu-id="3d848-161">um cabeçalho `Prefer: outlook.timezone` para obter valores de data/hora retornados na Hora Oficial do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="3d848-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="3d848-p108">Um parâmetro de consulta `$select` para retornar propriedades específicas. Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="3d848-p108">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<span data-ttu-id="3d848-164">A solicitação não especifica nenhum cabeçalho `Prefer: outlook.body-content-type` para indicar um formato específico para o corpo do evento retornado.</span><span class="sxs-lookup"><span data-stu-id="3d848-164">The request does not specify any `Prefer: outlook.body-content-type` header to indicate a specific format for the returned event body.</span></span> 


# <a name="http"></a>[<span data-ttu-id="3d848-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d848-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGIAAAoZDOFAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees 
Prefer: outlook.timezone="Pacific Standard Time"
```
# <a name="c"></a>[<span data-ttu-id="3d848-166">C#</span><span class="sxs-lookup"><span data-stu-id="3d848-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d848-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d848-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d848-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d848-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d848-169">Java</span><span class="sxs-lookup"><span data-stu-id="3d848-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3d848-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d848-170">Response</span></span>
<span data-ttu-id="3d848-171">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-171">Here is an example of the response.</span></span> <span data-ttu-id="3d848-172">Como nenhum cabeçalho `Prefer: outlook.body-content-type` foi especificado, a propriedade **body** será retornada no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="3d848-172">Because no `Prefer: outlook.body-content-type` header was specified, the **body** property is returned in the default HTML format.</span></span> 

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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location,hideAttendees)/$entity",
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
### <a name="example-2-get-the-body-property-in-text-format"></a><span data-ttu-id="3d848-173">Exemplo 2: Obter a propriedade body no formato de texto</span><span class="sxs-lookup"><span data-stu-id="3d848-173">Example 2: Get the body property in text format</span></span>
#### <a name="request"></a><span data-ttu-id="3d848-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-174">Request</span></span>
<span data-ttu-id="3d848-175">O exemplo a seguir mostra como usar um header para obter a propriedade body do `Prefer: outlook.body-content-type="text"` evento especificado no formato de texto. </span><span class="sxs-lookup"><span data-stu-id="3d848-175">The following example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** property of the specified event in text format.</span></span>

<span data-ttu-id="3d848-176">A solicitação também usa um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="3d848-176">The request also uses a `$select` query parameter to return specific properties.</span></span> <span data-ttu-id="3d848-177">Sem um parâmetro `$select`, todas as propriedades do evento serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="3d848-177">Without a `$select` parameter, all of the event properties will be returned.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d848-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d848-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_in_text"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkAGI1AAAoZDOFAAA=/?$select=subject,body,bodyPreview
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="3d848-179">C#</span><span class="sxs-lookup"><span data-stu-id="3d848-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d848-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d848-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d848-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d848-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d848-182">Java</span><span class="sxs-lookup"><span data-stu-id="3d848-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3d848-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d848-183">Response</span></span>
<span data-ttu-id="3d848-184">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-184">Here is an example of the response.</span></span> <span data-ttu-id="3d848-185">A propriedade **body** é retornada no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="3d848-185">The **body** property is returned in text format.</span></span> 

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

### <a name="example-3-get-an-event-that-specifies-more-than-one-location"></a><span data-ttu-id="3d848-186">Exemplo 3: Obter um evento que especifica mais de um local</span><span class="sxs-lookup"><span data-stu-id="3d848-186">Example 3: Get an event that specifies more than one location</span></span>
#### <a name="request"></a><span data-ttu-id="3d848-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-187">Request</span></span>

<span data-ttu-id="3d848-188">O exemplo a seguir mostra como obter um evento que especifica mais de um local.</span><span class="sxs-lookup"><span data-stu-id="3d848-188">The following example shows getting an event that specifies more than one location.</span></span> <span data-ttu-id="3d848-189">Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="3d848-189">The request specifies a `$select` query parameter to return specific properties.</span></span> 


# <a name="http"></a>[<span data-ttu-id="3d848-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d848-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_event_multiple_locations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,body,bodyPreview,organizer,attendees,start,end,location,locations
```
# <a name="c"></a>[<span data-ttu-id="3d848-191">C#</span><span class="sxs-lookup"><span data-stu-id="3d848-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-event-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d848-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d848-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-event-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d848-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d848-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-event-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d848-194">Java</span><span class="sxs-lookup"><span data-stu-id="3d848-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-event-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="3d848-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d848-195">Response</span></span>
<span data-ttu-id="3d848-196">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d848-196">Here is an example of the response.</span></span> <span data-ttu-id="3d848-197">A propriedade **locations** inclui detalhes dos três locais para os quais o evento é organizado.</span><span class="sxs-lookup"><span data-stu-id="3d848-197">The **locations** property includes details for the 3 locations that the event is organized for.</span></span> 

<span data-ttu-id="3d848-198">Como a solicitação não especifica nenhum ou um header, as propriedades inicial e final são exibidas no fuso horário UTC padrão e o corpo está no `Prefer: outlook.timezone` `Prefer: outlook.body-content-type` formato HTML padrão.  </span><span class="sxs-lookup"><span data-stu-id="3d848-198">Because the request does not specify any `Prefer: outlook.timezone` or `Prefer: outlook.body-content-type` header, the **start** and **end** properties are displayed in the default UTC time zone, and the body is in the default HTML format.</span></span>  

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
### <a name="example-4-expand-a-series-master-event"></a><span data-ttu-id="3d848-199">Exemplo 4: Expandir um evento mestre de série</span><span class="sxs-lookup"><span data-stu-id="3d848-199">Example 4: Expand a series master event</span></span>
#### <a name="request"></a><span data-ttu-id="3d848-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d848-200">Request</span></span>

<span data-ttu-id="3d848-201">O exemplo a seguir mostra a expansão de um evento mestre de série de uma série recorrente com exceções e ocorrências canceladas.</span><span class="sxs-lookup"><span data-stu-id="3d848-201">The following example shows expanding a series master event of a recurring series with exceptions and cancelled occurences.</span></span> <span data-ttu-id="3d848-202">Uma solicitação especifica um parâmetro de consulta `$select` para retornar propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="3d848-202">The request specifies a `$select` query parameter to return specific properties.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_event_seriesMaster_expansion"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/events/AAMkADAGAADDdm4NAAA=/?$select=subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences$expand=exceptionOccurrences
```
#### <a name="response"></a><span data-ttu-id="3d848-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d848-203">Response</span></span>
<span data-ttu-id="3d848-204">A operação GET retorna as propriedades selecionadas para o evento mestre da série.</span><span class="sxs-lookup"><span data-stu-id="3d848-204">The GET operation returns the selected properties for the series master event.</span></span> <span data-ttu-id="3d848-205">Especificamente, para eventos na coleção **exceptionOccurrences,** a operação retorna a propriedade **id** e as propriedades selecionadas aplicáveis (**subject**, **start**, **end**, **occurrenceId**).</span><span class="sxs-lookup"><span data-stu-id="3d848-205">Specifically, for events in the **exceptionOccurrences** collection, the operation returns the **id** property, and the applicable, selected properties (**subject**, **start**, **end**, **occurrenceId**).</span></span> <span data-ttu-id="3d848-206">Quanto aos eventos na coleção **cancelledOccurrences,** como os eventos não existem mais, a operação retorna apenas seus valores de propriedade **occurrenceId.**</span><span class="sxs-lookup"><span data-stu-id="3d848-206">As for events in the **cancelledOccurrences** collection, because the events no longer exist, the operation returns only their **occurrenceId** property values.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_event_seriesMaster_expansion",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1992

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events(subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences)/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "subject": "Daily stand-up",
  "cancelledOccurrences": [
     "OID.AAMkADAGAADDdm4NAAA=.2020-04-30",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-07",
     "OID.AAMkADAGAADDdm4NAAA=.2020-05-14"
    ],
  "occurrenceId": null,
    "start": {
        "dateTime": "2020-04-23T11:30:00.0000000",
        "timeZone": "UTC"
    },
  "end": {
        "dateTime": "2020-04-23T12:00:00.0000000",
        "timeZone": "UTC"
    },
  "exceptionOccurrences": [
        {
            "id": "AAMkADM0ZGRhMjdjLTA==",
            "Subject": "SM update 24",
            "occurrenceId": "OID.AAMkADAGAADDdm4NAAA=.2020-05-21",
            "start": {
                "dateTime": "2020-05-21T11:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-05-21T12:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="3d848-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="3d848-207">See also</span></span>

- [<span data-ttu-id="3d848-208">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="3d848-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3d848-209">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="3d848-209">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3d848-210">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="3d848-210">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
  ]
}
-->


