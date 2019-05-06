---
title: 'evento: delta'
description: Obtém um conjunto de eventos que foram adicionados, excluídos ou atualizado em um**calendarView** (um intervalo de eventos)
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ec03f37346d67c7c52128d8db146882a06d1e3f5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587245"
---
# <a name="event-delta"></a><span data-ttu-id="ad16e-103">evento: delta</span><span class="sxs-lookup"><span data-stu-id="ad16e-103">event: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad16e-104">Obtenha um conjunto de eventos que foram adicionados, excluídos ou atualizados em um **calendarView** (um intervalo de eventos) do calendário principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="ad16e-104">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="ad16e-p101">A chamada de função **delta** para eventos é semelhante a uma solicitação `GET /calendarview` por um intervalo de dados no calendário principal do usuário, exceto ao aplicar [tokens de estado](/graph/delta-query-overview) de forma apropriada em uma ou mais dessas chamadas, você pode consultar alterações incrementais no modo de exibição de calendário. Isso permite manter e sincronizar um armazenamento local de eventos do usuário no calendário principal, sem precisar buscar todos os eventos do calendário do servidor de cada vez.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad16e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad16e-107">Permissions</span></span>
<span data-ttu-id="ad16e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad16e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ad16e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad16e-110">Permission type</span></span>      | <span data-ttu-id="ad16e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad16e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad16e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad16e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad16e-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad16e-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ad16e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad16e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad16e-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad16e-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="ad16e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad16e-116">Application</span></span> | <span data-ttu-id="ad16e-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad16e-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad16e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad16e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/<id>/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="ad16e-119">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="ad16e-119">Query parameters</span></span>

<span data-ttu-id="ad16e-p103">O controle de alterações em eventos corresponde a uma série de uma ou mais chamadas de função **delta**. Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na porção do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar os parâmetros de consulta desejados uma vez antecipados. Em solicitações subsequentes, basta copiar e aplicar a URL `nextLink` ou `deltaLink` da resposta anterior já que essa URL inclui os parâmetros codificados desejados.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="ad16e-125">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="ad16e-125">Query parameter</span></span>      | <span data-ttu-id="ad16e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad16e-126">Type</span></span>   |<span data-ttu-id="ad16e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad16e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad16e-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ad16e-128">startDateTime</span></span>|<span data-ttu-id="ad16e-129">String</span><span class="sxs-lookup"><span data-stu-id="ad16e-129">String</span></span>|<span data-ttu-id="ad16e-p104">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T19:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ad16e-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="ad16e-132">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ad16e-132">endDateTime</span></span>|<span data-ttu-id="ad16e-133">String</span><span class="sxs-lookup"><span data-stu-id="ad16e-133">String</span></span>|<span data-ttu-id="ad16e-p105">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2015-11-08T20:00:00.0000000".</span><span class="sxs-lookup"><span data-stu-id="ad16e-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="ad16e-136">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="ad16e-136">$deltatoken</span></span> | <span data-ttu-id="ad16e-137">string</span><span class="sxs-lookup"><span data-stu-id="ad16e-137">string</span></span> | <span data-ttu-id="ad16e-p106">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="ad16e-140">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="ad16e-140">$skiptoken</span></span> | <span data-ttu-id="ad16e-141">string</span><span class="sxs-lookup"><span data-stu-id="ad16e-141">string</span></span> | <span data-ttu-id="ad16e-142">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="ad16e-142">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="ad16e-p107">Quando você faz uma consulta delta em um modo de exibição de calendário, espera obter todas as propriedades que obteria normalmente de uma solicitação `GET /calendarview`. O `$select` não é compatível nesse caso.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ad16e-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad16e-145">Request headers</span></span>
| <span data-ttu-id="ad16e-146">Nome</span><span class="sxs-lookup"><span data-stu-id="ad16e-146">Name</span></span>       | <span data-ttu-id="ad16e-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad16e-147">Type</span></span> | <span data-ttu-id="ad16e-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad16e-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="ad16e-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad16e-149">Authorization</span></span>  | <span data-ttu-id="ad16e-150">string</span><span class="sxs-lookup"><span data-stu-id="ad16e-150">string</span></span>  | <span data-ttu-id="ad16e-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ad16e-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad16e-153">Content-Type</span></span>  | <span data-ttu-id="ad16e-154">string</span><span class="sxs-lookup"><span data-stu-id="ad16e-154">string</span></span>  | <span data-ttu-id="ad16e-p109">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p109">application/json. Required.</span></span> |
| <span data-ttu-id="ad16e-157">Preferir</span><span class="sxs-lookup"><span data-stu-id="ad16e-157">Prefer</span></span> | <span data-ttu-id="ad16e-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ad16e-158">string</span></span>  | <span data-ttu-id="ad16e-p110">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="ad16e-161">Preferir</span><span class="sxs-lookup"><span data-stu-id="ad16e-161">Prefer</span></span> | <span data-ttu-id="ad16e-162">string</span><span class="sxs-lookup"><span data-stu-id="ad16e-162">string</span></span> | <span data-ttu-id="ad16e-p111">{Fuso horário}. Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="ad16e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad16e-165">Response</span></span>

<span data-ttu-id="ad16e-166">Se bem-sucedido, este método retorna o código de resposta `200 OK` e uma coleção de objetos [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad16e-166">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad16e-167">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad16e-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad16e-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad16e-168">Request</span></span>

<span data-ttu-id="ad16e-169">O exemplo a seguir mostra como fazer uma única chamada de função **delta** e limitar o número máximo de eventos no corpo da resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="ad16e-169">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="ad16e-170">Para controlar as alterações em um modo de exibição de calendário, você faz uma ou mais chamadas de função **delta**, com os [tokens de estado](/graph/delta-query-overview) apropriados, para obter o conjunto de alterações incrementais desde a última consulta delta.</span><span class="sxs-lookup"><span data-stu-id="ad16e-170">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarview/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="ad16e-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad16e-171">Response</span></span>
<span data-ttu-id="ad16e-p112">Se a solicitação for bem-sucedida, a resposta incluiria um token de estado, que é um _skipToken_ (em um cabeçalho de resposta _@odata.nextLink_) ou um _deltaToken_ (em um cabeçalho de resposta _@odata.deltaLink_). Respectivamente, elas indicam se você deverá continuar com a série ou se já concluiu a obtenção de todas as alterações dessa série.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="ad16e-174">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _@odata.nextLink_.</span><span class="sxs-lookup"><span data-stu-id="ad16e-174">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="ad16e-p113">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad16e-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ad16e-177">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ad16e-177">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ad16e-178">Basic</span><span class="sxs-lookup"><span data-stu-id="ad16e-178">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/event_delta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad16e-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad16e-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/event_delta-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="see-also"></a><span data-ttu-id="ad16e-180">Confira também</span><span class="sxs-lookup"><span data-stu-id="ad16e-180">See also</span></span>

- [<span data-ttu-id="ad16e-181">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ad16e-181">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="ad16e-182">Obter as alterações incrementais para os eventos em uma pasta</span><span class="sxs-lookup"><span data-stu-id="ad16e-182">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
