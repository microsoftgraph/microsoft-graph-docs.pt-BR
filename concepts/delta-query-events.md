---
title: 'Obter as alterações incrementais para os eventos em um modo de exibição de calendário '
description: 'O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário do calendário-padrão (../me/calendarview) '
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 5b5e41a689a62157bb686ca6bb97ef63af9ac02a
ms.sourcegitcommit: b469176f49aacbd02cd06838cc7c8d36cf5bc768
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "45165041"
---
# <a name="get-incremental-changes-to-events-in-a-calendar-view"></a><span data-ttu-id="f9001-103">Obter as alterações incrementais para os eventos em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="f9001-103">Get incremental changes to events in a calendar view</span></span> 

<span data-ttu-id="f9001-104">Usando a consulta delta, você pode obter eventos novos, atualizados ou excluídos em um calendário especificado, ou dentro de uma coleção de eventos definida (como um modo de exibição de calendário) no calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-104">By using delta query, you can get new, updated, or deleted events in a specified calendar(s), or within a defined collection of events (as a calendar view) in the calendar.</span></span> <span data-ttu-id="f9001-105">Este artigo descreve o último - obter essas alterações incrementais nos eventos em um modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-105">This article describes the latter - getting such incremental changes to events in a calendar view.</span></span> 

> <span data-ttu-id="f9001-106">**Observação** O recurso para o primeiro - obter alterações incrementais nos eventos em um calendário não vinculado a um período fixo de datas de início e de término - está disponível atualmente apenas na versão beta.</span><span class="sxs-lookup"><span data-stu-id="f9001-106">**Note** The capability for the former - getting incremental changes to events in a calendar not bound to a fixed start and end date range - is currently available only in the beta version.</span></span> <span data-ttu-id="f9001-107">Para saber mais, confira a função[delta](/graph/api/event-delta?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="f9001-107">For more information, see [delta](/graph/api/event-delta?view=graph-rest-beta) function.</span></span>

<span data-ttu-id="f9001-108">O modo de visualização de calendário em um conjunto de eventos em um intervalo de data/horário (../me/calendarview) do calendário-padrão, ou de outro calendário especificado ou de um calendário de grupo.</span><span class="sxs-lookup"><span data-stu-id="f9001-108">A calendar view is a collection of events in a date/time range (../me/calendarview) from the default calendar or some other specified calendar of a user, or from a group calendar.</span></span> <span data-ttu-id="f9001-109">Os eventos retornados podem incluir instâncias únicas, ou ocorrências e exceções de uma série recorrente.</span><span class="sxs-lookup"><span data-stu-id="f9001-109">The returned events may include single instances, or occurrences and exceptions of a recurring series.</span></span> <span data-ttu-id="f9001-110">Os dados-delta permitem manter e sincronizar o armazenamento local de eventos do usuário, sem ter de buscar todo o conjunto de eventos do usuário no servidor a cada vez que precise deles.</span><span class="sxs-lookup"><span data-stu-id="f9001-110">The delta data enables you to maintain and synchronize a local store of a user's events, without having to fetch the entire set of the user's events from the server every time.</span></span>

<span data-ttu-id="f9001-p104">A consulta delta oferece suporte à sincronização completa que recupera todos os eventos no modo de exibição calendário especificado e a sincronização incremental que recupera os eventos ocorridos no modo de exibição de calendário desde a última sincronização. Normalmente, você faria uma sincronização completa inicial e, logo após, obteria, periodicamente, as alterações incrementais para esse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-p104">Delta query supports both full synchronization that retrieves all the events in the specified calendar view, and incremental synchronization that retrieves those events that have changed in the calendar view since the last synchronization. Typically, you would do an initial full synchronization, and subsequently, get incremental changes to that calendar view periodically.</span></span> 

## <a name="track-event-changes-in-a-calendar-view"></a><span data-ttu-id="f9001-113">Rastrear alterações de evento em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="f9001-113">Track event changes in a calendar view</span></span>

<span data-ttu-id="f9001-114">A consulta delta para eventos em um modo de exibição de calendário é específica de um intervalo de calendário e data/hora que você especificar.</span><span class="sxs-lookup"><span data-stu-id="f9001-114">Delta query for events in a calendar view is specific to a calendar and date/time range that you specify.</span></span> <span data-ttu-id="f9001-115">Para controlar as alterações em vários calendários, você precisa controlar cada calendário individualmente.</span><span class="sxs-lookup"><span data-stu-id="f9001-115">To track the changes in multiple calendars, you need to track each calendar individually.</span></span> 

<span data-ttu-id="f9001-116">O rastreamento de alterações de evento em um modo de exibição de calendário normalmente corresponde a uma série de eventos de uma ou mais solicitações GET com a função [delta](/graph/api/event-delta?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9001-116">Tracking event changes in a calendar view typically is a round of one or more GET requests with the [delta](/graph/api/event-delta?view=graph-rest-1.0) function.</span></span> <span data-ttu-id="f9001-117">A solicitação GET inicial é muito semelhante à maneira como você [lista uma calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), exceto se você incluir a função **delta**.</span><span class="sxs-lookup"><span data-stu-id="f9001-117">The initial GET request is very much like the way you [list a calendarView](/graph/api/calendar-list-calendarview?view=graph-rest-1.0), except that you include the **delta** function.</span></span> <span data-ttu-id="f9001-118">A seguir está a solicitação delta GET inicial de um modo de exibição de calendário no calendário padrão do usuário conectado:</span><span class="sxs-lookup"><span data-stu-id="f9001-118">The following is the initial GET delta request of a calendar view in the signed-in user's default calendar:</span></span>

```
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
```

<span data-ttu-id="f9001-119">Uma solicitação GET com a função **delta** retorna:</span><span class="sxs-lookup"><span data-stu-id="f9001-119">A GET request with the **delta** function returns either:</span></span>

- <span data-ttu-id="f9001-120">Uma `nextLink` (que contém uma URL com chamada de função **delta** e um _skipToken_) ou</span><span class="sxs-lookup"><span data-stu-id="f9001-120">A `nextLink` (that contains a URL with a **delta** function call and a _skipToken_), or</span></span> 
- <span data-ttu-id="f9001-121">Uma `deltaLink` (que contém uma URL com chamada de função **delta** e _deltaToken_).</span><span class="sxs-lookup"><span data-stu-id="f9001-121">A `deltaLink` (that contains a URL with a **delta** function call and _deltaToken_).</span></span>

<span data-ttu-id="f9001-122">Esses tokens são [tokens de estado](delta-query-overview.md#state-tokens) que codificam os parâmetros _startDateTime_ e _endDateTime_, bem como qualquer outro parâmetro de consulta em sua solicitação GET de consulta delta inicial.</span><span class="sxs-lookup"><span data-stu-id="f9001-122">These tokens are [state tokens](delta-query-overview.md#state-tokens) which encode the _startDateTime_ and _endDateTime_ parameters, and any other query parameter in your initial delta query GET request.</span></span> <span data-ttu-id="f9001-123">Não é necessário incluir esses parâmetros em solicitações subsequentes, uma vez que eles são codificados nos tokens.</span><span class="sxs-lookup"><span data-stu-id="f9001-123">You do not need to include these parameters in subsequent requests as they are encoded in the tokens.</span></span>

<span data-ttu-id="f9001-p108">Estabeleça tokens de estado que sejam completamente opacos para o cliente. Para prosseguir com uma fase de controle de alterações, basta copiar e aplicar a URL `nextLink` ou `deltaLink` retornada da última solicitação GET para a próxima chamada de função **delta** do mesmo modo de exibição de calendário. Uma `deltaLink` retornada em uma resposta significa que a fase atual do rastreamento de alterações está concluída. Você pode salvar e usar a URL `deltaLink` quando começar a próxima fase.</span><span class="sxs-lookup"><span data-stu-id="f9001-p108">State tokens are completely opaque to the client. To proceed with a round of change tracking, simply copy and apply the `nextLink` or `deltaLink` URL returned from the last GET request to the next **delta** function call for that same calendar view. A `deltaLink` returned in a response signifies that the current round of change tracking is complete. You can save and use the `deltaLink` URL when you begin the next round.</span></span>

<span data-ttu-id="f9001-128">Verifique o [exemplo](#example-to-synchronize-events-in-a-calendar-view) abaixo para aprender a usar essas URLs `nextLink` e `deltaLink`.</span><span class="sxs-lookup"><span data-stu-id="f9001-128">See the [example](#example-to-synchronize-events-in-a-calendar-view) below to learn how to use these `nextLink` and `deltaLink` URLs.</span></span>

### <a name="use-query-parameters-in-a-delta-query-for-calendar-view"></a><span data-ttu-id="f9001-129">Use os parâmetros de consulta de uma consulta delta para a visualização de calendário</span><span class="sxs-lookup"><span data-stu-id="f9001-129">Use query parameters in a delta query for calendar view</span></span>

- <span data-ttu-id="f9001-130">Inclua os parâmetros _startDateTime_ e _endDateTime_ para definir um intervalo de data/hora para o modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-130">Include the _startDateTime_ and _endDateTime_ parameters to define a date/time range for your calendar view.</span></span>
- <span data-ttu-id="f9001-131">Não há suporte para `$select`.</span><span class="sxs-lookup"><span data-stu-id="f9001-131">`$select` is not supported.</span></span>


### <a name="optional-request-header"></a><span data-ttu-id="f9001-132">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f9001-132">Optional request header</span></span>

<span data-ttu-id="f9001-133">Cada solicitação GET de consulta delta retorna um conjunto de um ou mais eventos na resposta.</span><span class="sxs-lookup"><span data-stu-id="f9001-133">Each delta query GET request returns a collection of one or more events in the response.</span></span> <span data-ttu-id="f9001-134">Como alternativa, você pode especificar o cabeçalho de solicitação, `Prefer: odata.maxpagesize={x}`, para configurar o número máximo de eventos em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="f9001-134">You can optionally specify the request header, `Prefer: odata.maxpagesize={x}`, to set the maximum number of events in a response.</span></span>


## <a name="example-to-synchronize-events-in-a-calendar-view"></a><span data-ttu-id="f9001-135">Exemplo de sincronização de eventos em um modo de exibição de calendário</span><span class="sxs-lookup"><span data-stu-id="f9001-135">Example to synchronize events in a calendar view</span></span>

<span data-ttu-id="f9001-p110">O exemplo a seguir mostra uma série de 3 solicitações para sincronizar o calendário de padrão do usuário em um intervalo de tempo específico. Há 5 eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-p110">The following example shows a series of 3 requests to synchronize the user's default calendar in a specific time range. There are 5 events in that calendar view.</span></span>

- <span data-ttu-id="f9001-138">[Etapa 1: exemplo inicial de solicitação](#step-1-sample-initial-request) e [resposta](#sample-initial-response)</span><span class="sxs-lookup"><span data-stu-id="f9001-138">[Step 1: sample initial request](#step-1-sample-initial-request) and [response](#sample-initial-response)</span></span>
- <span data-ttu-id="f9001-139">[Etapa 2: segundo exemplo de solicitação](#step-2-sample-second-request) e [resposta](#sample-second-response)</span><span class="sxs-lookup"><span data-stu-id="f9001-139">[Step 2: sample second request](#step-2-sample-second-request) and [response](#sample-second-response)</span></span>
- <span data-ttu-id="f9001-140">[Etapa 3: terceiro exemplo de solicitação](#step-3-sample-third-request) e [resposta](#sample-third-and-final-response)</span><span class="sxs-lookup"><span data-stu-id="f9001-140">[Step 3: sample third request](#step-3-sample-third-request) and [final response](#sample-third-and-final-response)</span></span>

<span data-ttu-id="f9001-p111">Para economizar tempo, as respostas de exemplo exibem apenas um subconjunto das propriedades para um evento. Em uma chamada real, a maior parte das propriedades dos eventos são retornadas.</span><span class="sxs-lookup"><span data-stu-id="f9001-p111">For brevity, the sample responses show only a subset of the properties for an event. In an actual call, most event properties are returned.</span></span> 

<span data-ttu-id="f9001-143">Confira também o que você vai fazer na [próxima fase](#the-next-round-sample-first-response).</span><span class="sxs-lookup"><span data-stu-id="f9001-143">See also what you'll do in the [next round](#the-next-round-sample-first-response).</span></span>


### <a name="step-1-sample-initial-request"></a><span data-ttu-id="f9001-144">Passo 1: solicitação inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-144">Step 1: sample initial request</span></span>

<span data-ttu-id="f9001-145">Neste exemplo, o modo de exibição de calendário especificado no calendário padrão do usuário conectado está sendo sincronizado pela primeira vez, para que a solicitação de sincronização inicial não inclua nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="f9001-145">In this example, the specified calendar view in the signed-in user's default calendar is being synchronized for the first time, so the initial sync request does not include any state token.</span></span> <span data-ttu-id="f9001-146">Essa rodada mostrará todos os eventos nesse modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-146">This round will return all the events in that calendar view.</span></span>

<span data-ttu-id="f9001-147">A primeira solicitação especifica o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f9001-147">The first request specifies the following:</span></span>

- <span data-ttu-id="f9001-148">Data/horário valores para os parâmetros _startDateTime_ e _endDateTime_.</span><span class="sxs-lookup"><span data-stu-id="f9001-148">Date/time values for the _startDateTime_ and _endDateTime_ parameters.</span></span>
- <span data-ttu-id="f9001-149">O [cabeçalho de solicitação opcional](#optional-request-header), _odata.maxpagesize_, retornando 2 eventos de cada vez.</span><span class="sxs-lookup"><span data-stu-id="f9001-149">The [optional request header](#optional-request-header), _odata.maxpagesize_, returning 2 events at a time.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9001-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9001-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime=2016-12-01T00:00:00Z&enddatetime=2016-12-30T00:00:00Z HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="f9001-151">C#</span><span class="sxs-lookup"><span data-stu-id="f9001-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9001-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9001-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9001-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9001-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9001-154">Java</span><span class="sxs-lookup"><span data-stu-id="f9001-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="sample-initial-response"></a><span data-ttu-id="f9001-155">Resposta inicial de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-155">Sample initial response</span></span>

<span data-ttu-id="f9001-p113">A resposta inclui dois eventos e um `@odata.nextLink`cabeçalho de resposta com um `skipToken`. A URL `nextLink` indica que há mais eventos no modo de exibição de calendário a ser obtidos.</span><span class="sxs-lookup"><span data-stu-id="f9001-p113">The response includes two events and a `@odata.nextLink` response header with a `skipToken`. The `nextLink` URL indicates there are more events in the calendar view to get.</span></span>

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

### <a name="step-2-sample-second-request"></a><span data-ttu-id="f9001-158">Etapa 2: segundo exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9001-158">Step 2: sample second request</span></span>

<span data-ttu-id="f9001-p114">A segunda solicitação especifica a URL `nextLink` retornada da resposta anterior. Observe que não é mais necessário especificar os mesmos parâmetros _startDateTime_ e _endDateTime_ como na solicitação inicial, conforme o `skipToken` na URL `nextLink` os codifica e inclui.</span><span class="sxs-lookup"><span data-stu-id="f9001-p114">The second request specifies the `nextLink` URL returned from the previous response. Notice that it no longer has to specify the same _startDateTime_ and _endDateTime_ parameters as in the initial request, as the `skipToken` in the `nextLink` URL encodes and includes them.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9001-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9001-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmcCM996atia_s HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="f9001-162">C#</span><span class="sxs-lookup"><span data-stu-id="f9001-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9001-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9001-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9001-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9001-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9001-165">Java</span><span class="sxs-lookup"><span data-stu-id="f9001-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-second-response"></a><span data-ttu-id="f9001-166">Segunda resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-166">Sample second response</span></span> 

<span data-ttu-id="f9001-167">A segunda resposta retorna os 2 próximos eventos no modo de visualização de calendário e outro `nextLink`, indicando que há mais eventos a ser obtidos no modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="f9001-167">The second response returns the next 2 events in the calendar view and another `nextLink`, indicating there are more events to get from the calendar view.</span></span>

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


### <a name="step-3-sample-third-request"></a><span data-ttu-id="f9001-168">Etapa 3: terceira solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-168">Step 3: sample third request</span></span>

<span data-ttu-id="f9001-169">A terceira solicitação continua a usar as últimas `nextLink` retornadas da última solicitação de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f9001-169">The third request continues to use the latest `nextLink` returned from the last sync request.</span></span> 
 


# <a name="http"></a>[<span data-ttu-id="f9001-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9001-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken=R0usmci39OQxqJrxK4 HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="f9001-171">C#</span><span class="sxs-lookup"><span data-stu-id="f9001-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9001-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9001-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9001-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9001-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9001-174">Java</span><span class="sxs-lookup"><span data-stu-id="f9001-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="sample-third-and-final-response"></a><span data-ttu-id="f9001-175">Terceira e última resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-175">Sample third and final response</span></span>

<span data-ttu-id="f9001-p115">A terceira resposta retorna o único evento restante no modo de exibição calendário e uma URL `deltaLink` a indicar que a sincronização está concluída para esse modo de exibição de calendário. Salvar e usar a URL `deltaLink` para [sincronizar esse modo de exibição de calendário na próxima fase](#the-next-round-sample-first-request).</span><span class="sxs-lookup"><span data-stu-id="f9001-p115">The third response returns the only remaining event in the calendar view, and a `deltaLink` URL which indicates synchronization is complete for this calendar view. Save and use the `deltaLink` URL to [synchronize that calendar view in the next round](#the-next-round-sample-first-request).</span></span>


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


### <a name="the-next-round-sample-first-request"></a><span data-ttu-id="f9001-178">A próxima fase: primeira solicitação de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-178">The next round: sample first request</span></span>

<span data-ttu-id="f9001-p116">Usando o `deltaLink` da [última solicitação](#step-3-sample-third-request) na última fase, você poderá obter somente os eventos que sofreram alteração (por serem adicionados, excluídos ou atualizados) nesse modo de exibição de calendário desde então. Sua primeira solicitação na próxima fase terá aparência semelhante à seguinte, supondo que você prefira manter o mesmo tamanho máximo de página na resposta:</span><span class="sxs-lookup"><span data-stu-id="f9001-p116">Using the `deltaLink` from the [last request](#step-3-sample-third-request) in the last round, you will be able to get only those events that have changed (by being added, deleted, or updated) in that calendar view since then. Your first request in the next round will look like the following, assuming you prefer to keep the same maximum page size in the response:</span></span>


# <a name="http"></a>[<span data-ttu-id="f9001-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9001-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarview_delta_next"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E HTTP/1.1
Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="f9001-182">C#</span><span class="sxs-lookup"><span data-stu-id="f9001-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarview-delta-next-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9001-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9001-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarview-delta-next-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9001-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9001-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarview-delta-next-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9001-185">Java</span><span class="sxs-lookup"><span data-stu-id="f9001-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-calendarview-delta-next-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="the-next-round-sample-first-response"></a><span data-ttu-id="f9001-186">A próxima fase: primeira resposta de exemplo</span><span class="sxs-lookup"><span data-stu-id="f9001-186">The next round: sample first response</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f9001-187">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9001-187">See also</span></span>

- [<span data-ttu-id="f9001-188">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9001-188">Microsoft Graph delta query</span></span>](delta-query-overview.md)
- [<span data-ttu-id="f9001-189">Obter as alterações incrementais para mensagens</span><span class="sxs-lookup"><span data-stu-id="f9001-189">Get incremental changes to messages</span></span>](delta-query-messages.md)
- [<span data-ttu-id="f9001-190">Obter as alterações incrementais para grupos</span><span class="sxs-lookup"><span data-stu-id="f9001-190">Get incremental changes to groups</span></span>](delta-query-groups.md)
- [<span data-ttu-id="f9001-191">Obter as alterações incrementais para usuários</span><span class="sxs-lookup"><span data-stu-id="f9001-191">Get incremental changes to users</span></span>](delta-query-users.md)
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
