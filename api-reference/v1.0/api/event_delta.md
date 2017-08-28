# <a name="event-delta"></a><span data-ttu-id="bb52f-101">evento: delta</span><span class="sxs-lookup"><span data-stu-id="bb52f-101">event: delta</span></span>

<span data-ttu-id="bb52f-102">Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="bb52f-102">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="bb52f-p101">A chamada de função **delta** para eventos é semelhante a uma solicitação `GET /calendarview` por um intervalo de dados no calendário principal do usuário, exceto ao aplicar [tokens de estado](../../../concepts/delta_query_overview.md) de forma apropriada em uma ou mais dessas chamadas, você pode consultar alterações incrementais no modo de exibição de calendário. Isso permite manter e sincronizar um armazenamento local de eventos do usuário no calendário principal, sem precisar buscar todos os eventos do calendário do servidor de cada vez.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb52f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb52f-105">Permissions</span></span>
<span data-ttu-id="bb52f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb52f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="bb52f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb52f-108">Permission type</span></span>      | <span data-ttu-id="bb52f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb52f-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="bb52f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb52f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bb52f-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb52f-111">Calendars.Read</span></span>    | 
|<span data-ttu-id="bb52f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb52f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb52f-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb52f-113">Calendars.Read</span></span>    | 
|<span data-ttu-id="bb52f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb52f-114">Application</span></span> | <span data-ttu-id="bb52f-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bb52f-115">Calendars.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bb52f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb52f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/<id>/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

### <a name="query-parameters"></a><span data-ttu-id="bb52f-117">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="bb52f-117">Query parameters</span></span>

<span data-ttu-id="bb52f-p103">O controle de alterações em eventos corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="bb52f-123">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bb52f-123">Query parameter</span></span>      | <span data-ttu-id="bb52f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb52f-124">Type</span></span>   |<span data-ttu-id="bb52f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb52f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb52f-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bb52f-126">startDateTime</span></span>|<span data-ttu-id="bb52f-127">String</span><span class="sxs-lookup"><span data-stu-id="bb52f-127">String</span></span>|<span data-ttu-id="bb52f-p104">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="bb52f-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="bb52f-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bb52f-130">endDateTime</span></span>|<span data-ttu-id="bb52f-131">String</span><span class="sxs-lookup"><span data-stu-id="bb52f-131">String</span></span>|<span data-ttu-id="bb52f-p105">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="bb52f-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="bb52f-134">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="bb52f-134">$deltatoken</span></span> | <span data-ttu-id="bb52f-135">string</span><span class="sxs-lookup"><span data-stu-id="bb52f-135">string</span></span> | <span data-ttu-id="bb52f-p106">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p106">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="bb52f-138">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="bb52f-138">$skiptoken</span></span> | <span data-ttu-id="bb52f-139">string</span><span class="sxs-lookup"><span data-stu-id="bb52f-139">string</span></span> | <span data-ttu-id="bb52f-140">Um [token de estado](../../../concepts/delta_query_overview.md) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="bb52f-140">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="bb52f-p107">Quando você faz uma consulta delta em um modo de exibição de calendário, espera obter todas as propriedades que obteria normalmente de uma solicitação `GET /calendarview`. O `$select` não é compatível nesse caso.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="bb52f-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb52f-143">Request headers</span></span>
| <span data-ttu-id="bb52f-144">Nome</span><span class="sxs-lookup"><span data-stu-id="bb52f-144">Name</span></span>       | <span data-ttu-id="bb52f-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb52f-145">Type</span></span> | <span data-ttu-id="bb52f-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb52f-146">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="bb52f-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb52f-147">Authorization</span></span>  | <span data-ttu-id="bb52f-148">string</span><span class="sxs-lookup"><span data-stu-id="bb52f-148">string</span></span>  | <span data-ttu-id="bb52f-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bb52f-151">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb52f-151">Content-Type</span></span>  | <span data-ttu-id="bb52f-152">string</span><span class="sxs-lookup"><span data-stu-id="bb52f-152">string</span></span>  | <span data-ttu-id="bb52f-p109">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p109">application/json. Required.</span></span> |
| <span data-ttu-id="bb52f-155">Preferir</span><span class="sxs-lookup"><span data-stu-id="bb52f-155">Prefer</span></span> | <span data-ttu-id="bb52f-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb52f-156">string</span></span>  | <span data-ttu-id="bb52f-p110">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="bb52f-159">Preferir</span><span class="sxs-lookup"><span data-stu-id="bb52f-159">Prefer</span></span> | <span data-ttu-id="bb52f-160">string</span><span class="sxs-lookup"><span data-stu-id="bb52f-160">string</span></span> | <span data-ttu-id="bb52f-p111">{Fuso horário}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="bb52f-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb52f-163">Response</span></span>

<span data-ttu-id="bb52f-164">Se bem-sucedido, este método retorna o código de resposta `200, OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb52f-164">If successful, this method returns a `200, OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb52f-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb52f-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb52f-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb52f-166">Request</span></span>

<span data-ttu-id="bb52f-167">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de eventos no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="bb52f-167">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="bb52f-168">Para controlar as alterações em um modo de exibição de calendário, você faz uma ou mais chamadas de função **delta**, com os [tokens de estado](../../../concepts/delta_query_overview.md) apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="bb52f-168">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](../../../concepts/delta_query_overview.md), to get the set of incremental changes since the last delta query.</span></span> 

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarview/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="bb52f-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb52f-169">Response</span></span>
<span data-ttu-id="bb52f-p112">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado, que é um _skipToken_ (em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="bb52f-172">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="bb52f-172">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="bb52f-p113">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb52f-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="bb52f-175">Confira também</span><span class="sxs-lookup"><span data-stu-id="bb52f-175">See also</span></span>

- [<span data-ttu-id="bb52f-176">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bb52f-176">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="bb52f-177">Obter as alterações incrementais para os eventos em um calendário</span><span class="sxs-lookup"><span data-stu-id="bb52f-177">Get incremental changes to events in a calendar</span></span>](../../../concepts/delta_query_events.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->