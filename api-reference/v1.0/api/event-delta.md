---
title: 'evento: delta'
description: 'Obter um conjunto de eventos que foram adicionadas, excluídas ou atualizados em um **calendarView** (um intervalo de eventos) '
ms.openlocfilehash: be91eba577e1d00d638ff8a6d57ac5fb437b43d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003704"
---
# <a name="event-delta"></a><span data-ttu-id="8f222-103">evento: delta</span><span class="sxs-lookup"><span data-stu-id="8f222-103">event: delta</span></span>

<span data-ttu-id="8f222-104">Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="8f222-104">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="8f222-p101">A chamada de função **delta** para eventos é semelhante a uma solicitação `GET /calendarview` por um intervalo de dados no calendário principal do usuário, exceto ao aplicar [tokens de estado](/graph/delta-query-overview) de forma apropriada em uma ou mais dessas chamadas, você pode consultar alterações incrementais no modo de exibição de calendário. Isso permite manter e sincronizar um armazenamento local de eventos do usuário no calendário principal, sem precisar buscar todos os eventos do calendário do servidor de cada vez.</span><span class="sxs-lookup"><span data-stu-id="8f222-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f222-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f222-107">Permissions</span></span>
<span data-ttu-id="8f222-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f222-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f222-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f222-110">Permission type</span></span>      | <span data-ttu-id="8f222-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f222-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f222-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f222-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8f222-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f222-113">Calendars.Read</span></span>    |
|<span data-ttu-id="8f222-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f222-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f222-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f222-115">Calendars.Read</span></span>    |
|<span data-ttu-id="8f222-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f222-116">Application</span></span> | <span data-ttu-id="8f222-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8f222-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f222-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f222-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="8f222-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="8f222-119">Query parameters</span></span>

<span data-ttu-id="8f222-p103">O controle de alterações em eventos corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="8f222-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="8f222-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="8f222-125">Query parameter</span></span>      | <span data-ttu-id="8f222-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f222-126">Type</span></span>   |<span data-ttu-id="8f222-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f222-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f222-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8f222-128">startDateTime</span></span>|<span data-ttu-id="8f222-129">String</span><span class="sxs-lookup"><span data-stu-id="8f222-129">String</span></span>|<span data-ttu-id="8f222-p104">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="8f222-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="8f222-132">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8f222-132">endDateTime</span></span>|<span data-ttu-id="8f222-133">String</span><span class="sxs-lookup"><span data-stu-id="8f222-133">String</span></span>|<span data-ttu-id="8f222-p105">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="8f222-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="8f222-136">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="8f222-136">$deltatoken</span></span> | <span data-ttu-id="8f222-137">string</span><span class="sxs-lookup"><span data-stu-id="8f222-137">string</span></span> | <span data-ttu-id="8f222-p106">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="8f222-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="8f222-140">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="8f222-140">$skiptoken</span></span> | <span data-ttu-id="8f222-141">string</span><span class="sxs-lookup"><span data-stu-id="8f222-141">string</span></span> | <span data-ttu-id="8f222-142">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="8f222-142">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="8f222-p107">Quando você faz uma consulta delta em um modo de exibição de calendário, espera obter todas as propriedades que obteria normalmente de uma solicitação `GET /calendarview`. O `$select` não é compatível nesse caso.</span><span class="sxs-lookup"><span data-stu-id="8f222-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="8f222-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f222-145">Request headers</span></span>
| <span data-ttu-id="8f222-146">Nome</span><span class="sxs-lookup"><span data-stu-id="8f222-146">Name</span></span>       | <span data-ttu-id="8f222-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f222-147">Type</span></span> | <span data-ttu-id="8f222-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f222-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="8f222-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f222-149">Authorization</span></span>  | <span data-ttu-id="8f222-150">string</span><span class="sxs-lookup"><span data-stu-id="8f222-150">string</span></span>  | <span data-ttu-id="8f222-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f222-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f222-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f222-153">Content-Type</span></span>  | <span data-ttu-id="8f222-154">string</span><span class="sxs-lookup"><span data-stu-id="8f222-154">string</span></span>  | <span data-ttu-id="8f222-p109">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f222-p109">application/json. Required.</span></span> |
| <span data-ttu-id="8f222-157">Preferir</span><span class="sxs-lookup"><span data-stu-id="8f222-157">Prefer</span></span> | <span data-ttu-id="8f222-158">string</span><span class="sxs-lookup"><span data-stu-id="8f222-158">string</span></span>  | <span data-ttu-id="8f222-p110">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="8f222-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="8f222-161">Preferir</span><span class="sxs-lookup"><span data-stu-id="8f222-161">Prefer</span></span> | <span data-ttu-id="8f222-162">string</span><span class="sxs-lookup"><span data-stu-id="8f222-162">string</span></span> | <span data-ttu-id="8f222-p111">{Fuso horário}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="8f222-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="8f222-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f222-165">Response</span></span>

<span data-ttu-id="8f222-166">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f222-166">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f222-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f222-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f222-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f222-168">Request</span></span>

<span data-ttu-id="8f222-169">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de eventos no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="8f222-169">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="8f222-170">Para controlar as alterações em um modo de exibição de calendário, você faz uma ou mais chamadas de função **delta**, com os [tokens de estado](/graph/delta-query-overview) apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="8f222-170">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span> 

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="8f222-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f222-171">Response</span></span>
<span data-ttu-id="8f222-p112">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado, que é um _skipToken_ (em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="8f222-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="8f222-174">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="8f222-174">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="8f222-p113">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f222-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
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

### <a name="see-also"></a><span data-ttu-id="8f222-177">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f222-177">See also</span></span>

- [<span data-ttu-id="8f222-178">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8f222-178">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="8f222-179">Obter as alterações incrementais para os eventos em um calendário</span><span class="sxs-lookup"><span data-stu-id="8f222-179">Get incremental changes to events in a calendar</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->