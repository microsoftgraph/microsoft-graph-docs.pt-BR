---
title: 'evento: delta'
description: Obtém um conjunto de eventos que foram adicionados, excluídos ou atualizado em um **calendarView** (um intervalo de eventos)
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e76bf6cd10682717bebe9365afa14ced47d4c90
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042587"
---
# <a name="event-delta"></a><span data-ttu-id="bc431-103">evento: delta</span><span class="sxs-lookup"><span data-stu-id="bc431-103">event: delta</span></span>

<span data-ttu-id="bc431-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc431-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc431-105">Obter um conjunto de [recursos de](../resources/event.md) evento que foram adicionados, excluídos ou atualizados em um ou mais calendários.</span><span class="sxs-lookup"><span data-stu-id="bc431-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="bc431-106">Você pode obter tipos específicos dessas alterações incrementais nos eventos em todos os calendários de uma caixa de correio ou em um calendário específico ou em uma coleção de eventos de **um calendarView** (intervalo de eventos definidos por datas de início e término) de um calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="bc431-107">O calendário pode ser o calendário padrão ou algum outro calendário especificado do usuário.</span><span class="sxs-lookup"><span data-stu-id="bc431-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="bc431-108">No caso de obter alterações incrementais em **calendarView**, o calendário também pode ser um calendário de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc431-108">In the case of getting incremental changes on **calendarView**, the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="bc431-109">Uma **chamada** de função delta é semelhante a uma ou solicitação para o calendário especificado, exceto que, aplicando adequadamente `GET /events` `GET /calendarview` [tokens](/graph/delta-query-overview#state-tokens) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais de eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="bc431-110">Isso permite manter e sincronizar um armazenamento local de eventos no calendário especificado, sem precisar buscar todos os eventos desse calendário do servidor sempre.</span><span class="sxs-lookup"><span data-stu-id="bc431-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="bc431-111">A tabela a seguir lista as diferenças entre a **função delta** em eventos e a **função delta** em **um calendarView** em um calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="bc431-112">Função Delta em eventos</span><span class="sxs-lookup"><span data-stu-id="bc431-112">Delta function on events</span></span>  | <span data-ttu-id="bc431-113">Função Delta no calendarView</span><span class="sxs-lookup"><span data-stu-id="bc431-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="bc431-114">Obtém alterações incrementais de todos os eventos em um calendário não limitado por um intervalo de datas inicial e final.</span><span class="sxs-lookup"><span data-stu-id="bc431-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="bc431-115">Como alternativa, você pode obter alterações incrementais dos eventos em um calendário limitado por uma hora de início, começando em ou após essa data/hora.</span><span class="sxs-lookup"><span data-stu-id="bc431-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="bc431-116">Obtém alterações incrementais de eventos na data/hora inicial e final do **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="bc431-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="bc431-117">Retorna apenas um conjunto limitado de propriedades **de** evento por motivos de desempenho.</span><span class="sxs-lookup"><span data-stu-id="bc431-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="bc431-118">Cliente a ser usado posteriormente `GET /events/{id}` para expandir quaisquer eventos.</span><span class="sxs-lookup"><span data-stu-id="bc431-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="bc431-119">A expansão do lado do servidor retorna um conjunto mais completo de **propriedades de** evento.</span><span class="sxs-lookup"><span data-stu-id="bc431-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="bc431-120">A resposta inclui instâncias individuais e o mestre de série recorrente.</span><span class="sxs-lookup"><span data-stu-id="bc431-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="bc431-121">A resposta inclui instâncias únicas e ocorrências e exceções de séries recorrentes.</span><span class="sxs-lookup"><span data-stu-id="bc431-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="bc431-122">Aplica-se a eventos em calendários de usuários, mas não a calendários de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc431-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="bc431-123">Aplica-se a eventos em calendários de usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="bc431-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="bc431-124">Atualmente disponível apenas na versão beta.</span><span class="sxs-lookup"><span data-stu-id="bc431-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="bc431-125">Disponível nas versões v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="bc431-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="bc431-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc431-126">Permissions</span></span>
<span data-ttu-id="bc431-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc431-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc431-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc431-129">Permission type</span></span>      | <span data-ttu-id="bc431-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc431-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc431-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc431-131">Delegated (work or school account)</span></span> | <span data-ttu-id="bc431-132">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc431-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bc431-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc431-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc431-134">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc431-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bc431-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc431-135">Application</span></span> | <span data-ttu-id="bc431-136">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc431-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc431-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc431-137">HTTP request</span></span>

<span data-ttu-id="bc431-138">Esta seção mostra a sintaxe de solicitação HTTP para a chamada de função **delta** inicial para iniciar uma sincronização completa que recupera todos os eventos no calendário ou no visualização de calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="bc431-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="bc431-139">Essa sintaxe não contém [tokens de estado](/graph/delta-query-overview#state-tokens).</span><span class="sxs-lookup"><span data-stu-id="bc431-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="bc431-140">A URL de consulta retornada em uma `nextLink` ou de uma resposta `deltaLink` bem-sucedida inclui um token de estado.</span><span class="sxs-lookup"><span data-stu-id="bc431-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="bc431-141">Para qualquer chamada **de função delta** subsequente, use a URL de consulta em uma ou `nextLink` `deltaLink` precedindo-a.</span><span class="sxs-lookup"><span data-stu-id="bc431-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="bc431-142">Função Delta em eventos em um calendário do usuário (visualização)</span><span class="sxs-lookup"><span data-stu-id="bc431-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="bc431-143">Aplique a **função delta** em todos os eventos ou eventos que começam em ou após uma data/hora específica, nos calendários do usuário especificados:</span><span class="sxs-lookup"><span data-stu-id="bc431-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="bc431-144">Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada na caixa de correio _do usuário_:</span><span class="sxs-lookup"><span data-stu-id="bc431-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="bc431-145">Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no calendário padrão _do usuário:_</span><span class="sxs-lookup"><span data-stu-id="bc431-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="bc431-146">Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no _calendário do usuário especificado:_</span><span class="sxs-lookup"><span data-stu-id="bc431-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="bc431-147">Para obter alterações incrementais de todos os eventos ou de eventos que começam em ou após a data/hora especificada no grupo de calendários _especificado e no calendário_:</span><span class="sxs-lookup"><span data-stu-id="bc431-147">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="bc431-148">Função Delta no calendarView em um calendário do usuário</span><span class="sxs-lookup"><span data-stu-id="bc431-148">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="bc431-149">Aplique a **função delta** em um intervalo de eventos delimitados por data/hora inicial e final, no calendário do usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="bc431-149">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="bc431-150">Para obter alterações incrementais em um modo de exibição de calendário _do calendário padrão do usuário:_</span><span class="sxs-lookup"><span data-stu-id="bc431-150">To get incremental changes in a calendar view of _the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="bc431-151">Para obter alterações incrementais em uma exibição de calendário _do calendário de usuário especificado:_</span><span class="sxs-lookup"><span data-stu-id="bc431-151">To get incremental changes in a calendar view of _the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="bc431-152">Função Delta no calendarView em um calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="bc431-152">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="bc431-153">Para obter alterações incrementais em uma exibição de calendário do _calendário de um grupo:_</span><span class="sxs-lookup"><span data-stu-id="bc431-153">To get incremental changes in a calendar view of _a group's calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="bc431-154">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="bc431-154">Query parameters</span></span>

<span data-ttu-id="bc431-155">O controle de alterações incorre em uma rodada de uma ou mais chamadas **de função delta.**</span><span class="sxs-lookup"><span data-stu-id="bc431-155">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="bc431-156">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="bc431-156">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="bc431-157">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-157">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="bc431-158">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="bc431-158">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="bc431-159">Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.</span><span class="sxs-lookup"><span data-stu-id="bc431-159">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="bc431-160">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="bc431-160">Query parameter</span></span>      | <span data-ttu-id="bc431-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc431-161">Type</span></span>   |<span data-ttu-id="bc431-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc431-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc431-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bc431-163">startDateTime</span></span>|<span data-ttu-id="bc431-164">String</span><span class="sxs-lookup"><span data-stu-id="bc431-164">String</span></span>|<span data-ttu-id="bc431-p109">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="bc431-p109">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00". </span></span><br><span data-ttu-id="bc431-167">O timezone é especificado na parte de deslocamento de zona de tempo do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` header, se presente.</span><span class="sxs-lookup"><span data-stu-id="bc431-167">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="bc431-168">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="bc431-168">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="bc431-169">Opcional para **delta** em eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-169">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="bc431-170">Obrigatório para **delta em** **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="bc431-170">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="bc431-171">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bc431-171">endDateTime</span></span>|<span data-ttu-id="bc431-172">String</span><span class="sxs-lookup"><span data-stu-id="bc431-172">String</span></span>|<span data-ttu-id="bc431-p111">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="bc431-p111">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00". </span></span><br><span data-ttu-id="bc431-175">O timezone é especificado na parte de deslocamento de zona de tempo do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` header, se presente.</span><span class="sxs-lookup"><span data-stu-id="bc431-175">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="bc431-176">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="bc431-176">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="bc431-177">_Não há suporte para_ **delta** em eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-177">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="bc431-178">Obrigatório para **delta em** **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="bc431-178">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="bc431-179">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="bc431-179">$deltatoken</span></span> | <span data-ttu-id="bc431-180">string</span><span class="sxs-lookup"><span data-stu-id="bc431-180">string</span></span> | <span data-ttu-id="bc431-p113">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-p113">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="bc431-183">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="bc431-183">$skiptoken</span></span> | <span data-ttu-id="bc431-184">string</span><span class="sxs-lookup"><span data-stu-id="bc431-184">string</span></span> | <span data-ttu-id="bc431-185">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="bc431-185">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="bc431-186">Não suporta `$expand` , , , e `$filter` `$orderby` `$select` `$search` .</span><span class="sxs-lookup"><span data-stu-id="bc431-186">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="bc431-187">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc431-187">Request headers</span></span>
| <span data-ttu-id="bc431-188">Nome</span><span class="sxs-lookup"><span data-stu-id="bc431-188">Name</span></span>       | <span data-ttu-id="bc431-189">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc431-189">Type</span></span> | <span data-ttu-id="bc431-190">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc431-190">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="bc431-191">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc431-191">Authorization</span></span>  | <span data-ttu-id="bc431-192">string</span><span class="sxs-lookup"><span data-stu-id="bc431-192">string</span></span>  | <span data-ttu-id="bc431-p114">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc431-p114">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc431-195">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc431-195">Content-Type</span></span>  | <span data-ttu-id="bc431-196">string</span><span class="sxs-lookup"><span data-stu-id="bc431-196">string</span></span>  | <span data-ttu-id="bc431-p115">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc431-p115">application/json. Required.</span></span> |
| <span data-ttu-id="bc431-199">Preferir</span><span class="sxs-lookup"><span data-stu-id="bc431-199">Prefer</span></span> | <span data-ttu-id="bc431-200">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc431-200">string</span></span>  | <span data-ttu-id="bc431-p116">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="bc431-p116">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="bc431-203">Preferir</span><span class="sxs-lookup"><span data-stu-id="bc431-203">Prefer</span></span> | <span data-ttu-id="bc431-204">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc431-204">string</span></span> | <span data-ttu-id="bc431-205">outlook.timezone={Cadeia de caracteres de fuso horário}.</span><span class="sxs-lookup"><span data-stu-id="bc431-205">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="bc431-206">Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="bc431-206">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="bc431-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc431-207">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="bc431-208">Função Delta em eventos (visualização)</span><span class="sxs-lookup"><span data-stu-id="bc431-208">Delta function on events (preview)</span></span>
<span data-ttu-id="bc431-209">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de](../resources/event.md) eventos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-209">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="bc431-210">Cada **evento** na resposta contém apenas **as propriedades id**, **type**, **start** e **end** por motivos de desempenho.</span><span class="sxs-lookup"><span data-stu-id="bc431-210">Each **event** in the response contains only the **id**, **type**, **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="bc431-211">Use `GET /events/{id}` subsequentemente para expandir quaisquer eventos da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-211">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="bc431-212">Função Delta no calendarView</span><span class="sxs-lookup"><span data-stu-id="bc431-212">Delta function on calendarView</span></span>
<span data-ttu-id="bc431-213">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de](../resources/event.md) eventos no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-213">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="bc431-214">Espere obter todas as propriedades que você normalmente obteria de uma `GET /calendarview` solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc431-214">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="bc431-215">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bc431-215">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="bc431-216">Exemplo 1: função Delta em eventos em um calendário (visualização)</span><span class="sxs-lookup"><span data-stu-id="bc431-216">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="bc431-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc431-217">Request</span></span>
<span data-ttu-id="bc431-218">O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário padrão do usuário in-loco, que ocorrem em ou após o parâmetro `startDateTime` especificado.</span><span class="sxs-lookup"><span data-stu-id="bc431-218">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="bc431-219">A solicitação inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="bc431-219">The initial request does not include any state token.</span></span> 

<span data-ttu-id="bc431-220">A solicitação usa `Prefer: odata.maxpagesize` o header para limitar o número máximo de eventos em cada resposta a 1.</span><span class="sxs-lookup"><span data-stu-id="bc431-220">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="bc431-221">Continue chamando a `delta` função usando a consulta retornada até obter uma na `@odata.nextLink` `@odata.deltaLink` resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-221">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="bc431-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc431-222">Response</span></span>

<span data-ttu-id="bc431-223">Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que é _um skipToken_ (em um header de resposta _\@ odata.nextLink)_ ou _um deltaToken_ (em um header de resposta _\@ odata.deltaLink)._</span><span class="sxs-lookup"><span data-stu-id="bc431-223">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="bc431-224">Respectivamente, eles indicam se você deve continuar com a rodada ou se você concluiu todas as alterações para essa rodada.</span><span class="sxs-lookup"><span data-stu-id="bc431-224">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="bc431-225">A resposta a seguir mostra _um skipToken_ em um header de resposta _\@ odata.nextLink._</span><span class="sxs-lookup"><span data-stu-id="bc431-225">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="bc431-226">Exemplo 2: função Delta em calendarView</span><span class="sxs-lookup"><span data-stu-id="bc431-226">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="bc431-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc431-227">Request</span></span>

<span data-ttu-id="bc431-228">O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário especificado do usuário in-loco, dentro do intervalo de datas indicadas pelo **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="bc431-228">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="bc431-229">A solicitação inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="bc431-229">The initial request does not include any state token.</span></span> 

<span data-ttu-id="bc431-230">A solicitação usa `Prefer: odata.maxpagesize` o header para limitar o número máximo de eventos em cada resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="bc431-230">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="bc431-231">Continue chamando a função usando a consulta retornada até que você receba todos os eventos nesse `delta` `@odata.nextLink` exibição de calendário e `@odata.deltaLink` um na resposta.</span><span class="sxs-lookup"><span data-stu-id="bc431-231">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="bc431-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="bc431-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="bc431-233">C#</span><span class="sxs-lookup"><span data-stu-id="bc431-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bc431-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc431-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bc431-235">Java</span><span class="sxs-lookup"><span data-stu-id="bc431-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bc431-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc431-236">Response</span></span>

<span data-ttu-id="bc431-237">Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que é _um skipToken_ (em um header de resposta _\@ odata.nextLink)_ ou _um deltaToken_ (em um header de resposta _\@ odata.deltaLink)._</span><span class="sxs-lookup"><span data-stu-id="bc431-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="bc431-238">Respectivamente, eles indicam se você deve continuar com a rodada ou se você concluiu todas as alterações para essa rodada.</span><span class="sxs-lookup"><span data-stu-id="bc431-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="bc431-239">A resposta a seguir mostra _um skipToken_ em um header de resposta _\@ odata.nextLink._</span><span class="sxs-lookup"><span data-stu-id="bc431-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="bc431-240">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bc431-240">Note: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="bc431-241">Confira também</span><span class="sxs-lookup"><span data-stu-id="bc431-241">See also</span></span>

- [<span data-ttu-id="bc431-242">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bc431-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="bc431-243">Obter as alterações incrementais para os eventos em uma pasta</span><span class="sxs-lookup"><span data-stu-id="bc431-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

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
  ]
}
-->


