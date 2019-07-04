---
title: 'Obter as alterações incrementais para os eventos em um modo de exibição de calendário '
description: 'O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário do calendário-padrão (../me/calendarview) '
author: piotrci
localization_priority: Priority
ms.openlocfilehash: fa759b233aafaf03322d416ef9f686c4315b5a9f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455158"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="ede0f-103">Obter as alterações incrementais para os eventos em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="ede0f-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="ede0f-p101">O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário do calendário-padrão (../me/calendarview) ou algum outro calendário do usuário. Usando a consulta de delta, você pode obter eventos novos, atualizados ou excluídos em um modo de exibição de calendário. Os eventos retornados podem incluir ocorrências e exceções de uma série recorrente e instâncias únicas. Os dados-delta permitem manter e sincronizar o armazenamento local de eventos do usuário, sem ter de buscar todo o conjunto de eventos do usuário no servidor a cada vez que precise deles.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p101">A calendar view is a collection of events in a date/time range from the default calendar (../me/calendarview) or some other calendar of the user's. By using delta query, you can get new, updated, or deleted events in a calendar view. The returned events may include occurrences and exceptions of a recurring series, and single instances. The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="ede0f-p102">A consulta delta oferece suporte à sincronização completa que recupera todos os eventos no modo de exibição calendário especificado e a sincronização incremental que recupera os eventos ocorridos no modo de exibição de calendário desde a última sincronização. Normalmente, você faria uma sincronização completa inicial e, logo após, obteria, periodicamente, as alterações incrementais para esse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p102">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="ede0f-110">Rastrear alterações de evento em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="ede0f-110">Track event changes in a calendar view</span></span>

<span data-ttu-id="ede0f-p103">A consulta delta para eventos é específica de um intervalo de calendário e data/hora que você especificar (ou seja, um modo de exibição de calendário). Para controlar as alterações em vários calendários, você precisa controlar cada calendário individualmente.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p103">Delta query for events is specific to a calendar and date/time range that you specify (i.e., a calendar view). To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="ede0f-p104">O rastreamento de alterações de evento em um modo de exibição de calendário normalmente corresponde a uma série de eventos de uma ou mais solicitações GET com a função [delta](/graph/api/event-delta?view=graph-rest-1.0). A solicitação GET inicial é muito semelhante à maneira como você [lista uma calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), exceto se você incluir a função **delta**:</span><span class="sxs-lookup"><span data-stu-id="ede0f-p104">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function. The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="ede0f-115">Uma solicitação GET com a função **delta** retorna:</span><span class="sxs-lookup"><span data-stu-id="ede0f-115">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="ede0f-116">Uma `nextLink` (que contém uma URL com chamada de função **delta** e um _skipToken_) ou</span><span class="sxs-lookup"><span data-stu-id="ede0f-116">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="ede0f-117">Uma `deltaLink` (que contém uma URL com chamada de função **delta** e _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="ede0f-117">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="ede0f-118">Esses tokens são [tokens de estado](delta-query-overview.md#state-tokens) que codificam os parâmetros refs/remotes/microsoftgraph/master _startDateTime_ e _endDateTime_, bem como qualquer outro parâmetro de consulta em sua solicitação GET de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="ede0f-118">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the refs/remotes/microsoftgraph/master _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> 

<span data-ttu-id="ede0f-p105">Estabeleça tokens de estado que sejam completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função **delta** do mesmo modo de exibição de calendário. Uma `deltaLink` retornada em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p105">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="ede0f-123">Verifique o [exemplo](#example-to-synchronize-events-in-a-calendar-view) abaixo para aprender a usar essas URLs `nextLink` e `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="ede0f-123">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="ede0f-124">Use os parâmetros de consulta de uma consulta delta para a visualização de calendário</span><span class="sxs-lookup"><span data-stu-id="ede0f-124">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="ede0f-125">Inclua os parâmetros _startDateTime_ e _endDateTime_ para definir um intervalo de data/hora para o modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ede0f-125">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="ede0f-126">Não há suporte para `$select`.</span><span class="sxs-lookup"><span data-stu-id="ede0f-126">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="ede0f-127">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="ede0f-127">Optional request header</span></span>

<span data-ttu-id="ede0f-128">Cada solicitação GET de consulta delta retorna um conjunto de um ou mais eventos na resposta.</span><span class="sxs-lookup"><span data-stu-id="ede0f-128">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="ede0f-129">Como alternativa, você pode especificar o cabeçalho de solicitação, `Prefer: odata.maxpagesize={x}`, para configurar o número máximo de eventos em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ede0f-129">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="ede0f-130">Exemplo de sincronização de eventos em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="ede0f-130">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="ede0f-p107">O exemplo a seguir mostra uma série de 3 solicitações para sincronizar o calendário de padrão do usuário em um intervalo de tempo específico. Há 5 eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p107">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="ede0f-133">[Etapa 1: exemplo inicial de solicitação](#step-1-sample-initial-request) e [resposta](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="ede0f-133">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="ede0f-134">[Etapa 2: segundo exemplo de solicitação](#step-2-sample-second-request) e [resposta](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="ede0f-134">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="ede0f-135">[Etapa 3: terceiro exemplo de solicitação](#step-3-sample-third-request) e [resposta](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="ede0f-135">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="ede0f-p108">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p108">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="ede0f-138">Confira também o que você vai fazer na [próxima fase](#the-next-round-sample-first-response).</span><span class="sxs-lookup"><span data-stu-id="ede0f-138">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="ede0f-139">Passo 1: solicitação inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-139">Step 1: sample initial request</span></span>

<span data-ttu-id="ede0f-p109">Neste exemplo, o modo de exibição de calendário especificado está sendo sincronizado pela primeira vez, para que a solicitação de sincronização inicial não inclua nenhum token de estado. Esta fase retornará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p109">In this example, the specified calendar view is being synchronized for the first time, so the initial sync request does not include any state token. This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="ede0f-142">A primeira solicitação especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="ede0f-142">The first request specifies the following:</span></span>

- <span data-ttu-id="ede0f-143">Data/horário valores para os parâmetros _startDateTime_ e _endDateTime_.</span><span class="sxs-lookup"><span data-stu-id="ede0f-143">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="ede0f-144">O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="ede0f-144">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ede0f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="ede0f-145">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ede0f-146">C#</span><span class="sxs-lookup"><span data-stu-id="ede0f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ede0f-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="ede0f-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ede0f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ede0f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a><span data-ttu-id="ede0f-149">Resposta inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-149">Sample initial response</span></span>

<span data-ttu-id="ede0f-p110">A resposta inclui dois eventos e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`. A URL `nextLink` indica que há mais eventos no modo de exibição de calendário a ser obtidos.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p110">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIQ==\"",
            "subject":"Plan shopping list",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-09T20:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-09T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },      
            "id":"AAMkADNVxRAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIg==\"",
            "subject":"Pick up car",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T01:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxSAAA="
        }
    ]
}
```

### <a name="step-2-sample-second-request"></a><span data-ttu-id="ede0f-152">Etapa 2: segundo exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="ede0f-152">Step 2: sample second request</span></span>

<span data-ttu-id="ede0f-p111">A segunda solicitação especifica a URL `nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros _startDateTime_ e _endDateTime_ como na solicitação inicial, conforme o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="ede0f-p111">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ede0f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="ede0f-155">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ede0f-156">C#</span><span class="sxs-lookup"><span data-stu-id="ede0f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ede0f-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="ede0f-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ede0f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ede0f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a><span data-ttu-id="ede0f-159">Segunda resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-159">Sample second response</span></span> 

<span data-ttu-id="ede0f-160">A segunda resposta retorna os 2 próximos eventos no modo de visualização de calendário e outro `nextLink`, indicando que há mais eventos a ser obtidos no modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ede0f-160">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvIw==\"",
            "subject":"Get food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T19:30:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-10T21:30:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxTAAA="
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAAFXcvJA==\"",
            "subject":"Prepare food",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-10T22:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-11T00:00:00.0000000",
                "timeZone":"UTC"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADVxUAAA="
        }
    ]
}
```


### <a name="step-3-sample-third-request"></a><span data-ttu-id="ede0f-161">Etapa 3: terceira solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-161">Step 3: sample third request</span></span>

<span data-ttu-id="ede0f-162">A terceira solicitação continua a usar as últimas `nextLink` retornadas da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="ede0f-162">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 


# <a name="httptabhttp"></a>[<span data-ttu-id="ede0f-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="ede0f-163">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ede0f-164">C#</span><span class="sxs-lookup"><span data-stu-id="ede0f-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ede0f-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="ede0f-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ede0f-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ede0f-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a><span data-ttu-id="ede0f-167">Terceira e última resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-167">Sample third and final response</span></span>

<span data-ttu-id="ede0f-p112">A terceira resposta retorna o único evento restante no modo de exibição calendário e uma URL `deltaLink` a indicar que a sincronização está concluída para esse modo de exibição de calendário. Salvar e usar a URL `deltaLink` para [sincronizar esse modo de exibição de calendário na próxima fase](#the-next-round-sample-first-request).</span><span class="sxs-lookup"><span data-stu-id="ede0f-p112">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E",
    "value":[
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97g==\"",
            "subject":"Rest!",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-12T02:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-12T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Home"
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HuAAA="
        }
    ]
}
```


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="ede0f-170">A próxima fase: primeira solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-170">The next round: sample first request</span></span>

<span data-ttu-id="ede0f-p113">Usando o `deltaLink` da [última solicitação](#step-3-sample-third-request) na última fase, você poderá obter somente os eventos que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse modo de exibição de calendário desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:</span><span class="sxs-lookup"><span data-stu-id="ede0f-p113">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ede0f-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="ede0f-173">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ede0f-174">C#</span><span class="sxs-lookup"><span data-stu-id="ede0f-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ede0f-175">Javascript</span><span class="sxs-lookup"><span data-stu-id="ede0f-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ede0f-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ede0f-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="ede0f-177">A próxima fase: primeira resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="ede0f-177">The next round: sample first response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(event)",
    "@odata.deltaLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcFuQtZdtpk4",
    "value":[
        {
            "@odata.type": "#microsoft.graph.event",
            "id": "AAMkADk0MGFkODE3LWE4MmYtNDRhOS04OGQLkRkXbBznTvAADb6ytyAAA=",
            "@removed": {
                "reason": "deleted"
            }
        },
        {
            "@odata.type":"#microsoft.graph.event",
            "@odata.etag":"W/\"EZ9r3czxY0m2jz8c45czkwAALZu97w==\"",
            "subject":"Attend service",
            "body":{
                "contentType":"html",
                "content":""
            },
            "start":{
                "dateTime":"2016-12-25T06:00:00.0000000",
                "timeZone":"UTC"
            },
            "end":{
                "dateTime":"2016-12-25T07:30:00.0000000",
                "timeZone":"UTC"
            },
            "location":{
                "displayName":"Chapel of Saint Ignatius",
                "address":{
                    "street":"900 Broadway",
                    "city":"Seattle",
                    "state":"WA",
                    "countryOrRegion":"United States",
                    "postalCode":""
                },
                "coordinates":{
                    "latitude":47.6105,
                    "longitude":-122.321
                }
            },
            "attendees":[

            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@contoso.onmicrosoft.com"
                }
            },
            "id":"AAMkADj1HvAAA="
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="ede0f-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="ede0f-178">See also</span></span>

- [<span data-ttu-id="ede0f-179">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ede0f-179">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="ede0f-180">Obter as alterações incrementais para mensagens</span><span class="sxs-lookup"><span data-stu-id="ede0f-180">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="ede0f-181">Obter as alterações incrementais para grupos</span><span class="sxs-lookup"><span data-stu-id="ede0f-181">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="ede0f-182">Obter as alterações incrementais para usuários</span><span class="sxs-lookup"><span data-stu-id="ede0f-182">Get incremental changes to users</span></span>](delta-query-users.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example to synchronize events in a calendar view",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
