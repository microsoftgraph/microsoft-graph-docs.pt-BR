---
title: 'evento: delta'
description: Obtém um conjunto de eventos que foram adicionados, excluídos ou atualizado em um **calendarView** (um intervalo de eventos)
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7499c8a8ffc5af6e03483a4448fb68c0509c26c6
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932385"
---
# <a name="event-delta"></a><span data-ttu-id="651dc-103">evento: delta</span><span class="sxs-lookup"><span data-stu-id="651dc-103">event: delta</span></span>

<span data-ttu-id="651dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="651dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="651dc-105">Obter um conjunto de recursos de [eventos](../resources/event.md) que foram adicionados, excluídos ou atualizados em um ou mais calendários.</span><span class="sxs-lookup"><span data-stu-id="651dc-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="651dc-106">Você pode obter tipos específicos dessas alterações incrementais nos eventos de todos os calendários de uma caixa de correio ou em um calendário específico ou em uma coleção de eventos de um **calendarView** (intervalo de eventos definido por datas de início e término) de um calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="651dc-107">O calendário pode ser o calendário padrão ou algum outro calendário especificado do.</span><span class="sxs-lookup"><span data-stu-id="651dc-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="651dc-108">No caso de obter alterações incrementais no **calendarView** , o calendário também pode ser um calendário de grupo.</span><span class="sxs-lookup"><span data-stu-id="651dc-108">In the case of getting incremental changes on **calendarView** , the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="651dc-109">Uma chamada de função **Delta** é semelhante a um `GET /events` ou `GET /calendarview` solicitação para o calendário especificado, exceto pelo fato de que, por meio da aplicação adequada de [tokens de estado](/graph/delta-query-overview#state-tokens) em uma ou mais dessas chamadas, você pode consultar alterações incrementais de eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="651dc-110">Isso permite que você mantenha e sincronize um repositório local de eventos no calendário especificado, sem ter que buscar todos os eventos desse calendário a cada vez.</span><span class="sxs-lookup"><span data-stu-id="651dc-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="651dc-111">A tabela a seguir lista as diferenças entre a função **Delta** em eventos e a função **Delta** em um **calendarView** em um calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="651dc-112">Função Delta em eventos</span><span class="sxs-lookup"><span data-stu-id="651dc-112">Delta function on events</span></span>  | <span data-ttu-id="651dc-113">Função Delta no calendarView</span><span class="sxs-lookup"><span data-stu-id="651dc-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="651dc-114">Obtém alterações incrementais de todos os eventos em um calendário não limitado por um intervalo de datas de início e de término.</span><span class="sxs-lookup"><span data-stu-id="651dc-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="651dc-115">Como alternativa, você pode obter alterações incrementais dos eventos em um calendário limitado por uma hora de início, a partir de ou após essa data/hora.</span><span class="sxs-lookup"><span data-stu-id="651dc-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="651dc-116">Obtém alterações incrementais de eventos dentro da data/hora inicial e final do **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="651dc-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="651dc-117">Retorna somente um conjunto limitado de propriedades de **evento** por motivos de desempenho.</span><span class="sxs-lookup"><span data-stu-id="651dc-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="651dc-118">Cliente a usar subseqüentemente `GET /events/{id}` para expandir qualquer evento.</span><span class="sxs-lookup"><span data-stu-id="651dc-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="651dc-119">A expansão do lado do servidor retorna um conjunto mais completo de propriedades de **evento** .</span><span class="sxs-lookup"><span data-stu-id="651dc-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="651dc-120">A resposta inclui instâncias únicas e mestre da série recorrente.</span><span class="sxs-lookup"><span data-stu-id="651dc-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="651dc-121">A resposta inclui instâncias únicas e ocorrências e exceções de série recorrente.</span><span class="sxs-lookup"><span data-stu-id="651dc-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="651dc-122">Aplica-se a eventos em calendários do usuário, mas não a calendários do grupo.</span><span class="sxs-lookup"><span data-stu-id="651dc-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="651dc-123">Aplica-se a eventos em calendários de usuário e de grupo.</span><span class="sxs-lookup"><span data-stu-id="651dc-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="651dc-124">Disponível atualmente somente na versão beta.</span><span class="sxs-lookup"><span data-stu-id="651dc-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="651dc-125">Disponível nas versões v 1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="651dc-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="651dc-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="651dc-126">Permissions</span></span>
<span data-ttu-id="651dc-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="651dc-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="651dc-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="651dc-129">Permission type</span></span>      | <span data-ttu-id="651dc-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="651dc-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="651dc-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="651dc-131">Delegated (work or school account)</span></span> | <span data-ttu-id="651dc-132">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651dc-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="651dc-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="651dc-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="651dc-134">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651dc-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="651dc-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="651dc-135">Application</span></span> | <span data-ttu-id="651dc-136">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="651dc-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="651dc-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="651dc-137">HTTP request</span></span>

<span data-ttu-id="651dc-138">Esta seção mostra a sintaxe de solicitação HTTP para a chamada de função **Delta** inicial para iniciar uma sincronização completa que recupera todos os eventos no calendário ou no modo de exibição de calendário especificado.</span><span class="sxs-lookup"><span data-stu-id="651dc-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="651dc-139">Esta sintaxe não contém nenhum [token de estado](/graph/delta-query-overview#state-tokens).</span><span class="sxs-lookup"><span data-stu-id="651dc-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="651dc-140">A URL de consulta retornada em `nextLink` uma `deltaLink` resposta bem-sucedida inclui um token de estado.</span><span class="sxs-lookup"><span data-stu-id="651dc-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="651dc-141">Para qualquer chamada de função **Delta** subsequente, use a URL de consulta em um `nextLink` ou `deltaLink` antes dela.</span><span class="sxs-lookup"><span data-stu-id="651dc-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="651dc-142">Função Delta em eventos em um calendário de usuário (visualização)</span><span class="sxs-lookup"><span data-stu-id="651dc-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="651dc-143">Aplicar a função **Delta** em todos os eventos ou eventos que começam em ou após uma data/hora específica, nos calendários de usuário especificados:</span><span class="sxs-lookup"><span data-stu-id="651dc-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="651dc-144">Para obter as alterações incrementais de todos os eventos, ou de eventos que começam na data/hora especificadas _na caixa de correio do usuário_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="651dc-145">Para obter as alterações incrementais de todos os eventos, ou de eventos a partir de ou após a data/hora especificada _no calendário padrão do usuário_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="651dc-146">Para obter as alterações incrementais de todos os eventos, ou de eventos a partir de ou após a data/hora especificada _no calendário do usuário especificado_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="651dc-147">Para obter alterações incrementais de todos os eventos, ou de eventos a partir de ou após a data/hora especificada _no calendário especificado do grupo de calendário padrão_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-147">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified calendar of the default calendar group_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroup/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta 

  GET /me/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="651dc-148">Para obter as alterações incrementais todos os eventos, ou de eventos que começam na data/hora especificadas no _grupo de calendários e no calendário especificado_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-148">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_ :</span></span>
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

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="651dc-149">Função Delta no calendarView em um calendário de usuário</span><span class="sxs-lookup"><span data-stu-id="651dc-149">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="651dc-150">Aplicar a função **Delta** em um intervalo de eventos delimitado por data e hora de início e término, no calendário de usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="651dc-150">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="651dc-151">Para obter alterações incrementais em um modo de exibição de calendário do _calendário padrão do usuário_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-151">To get incremental changes in a calendar view of _the user's default calendar_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="651dc-152">Para obter alterações incrementais em um modo de exibição de calendário do _calendário do usuário especificado_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-152">To get incremental changes in a calendar view of _the specified user calendar_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="651dc-153">Função Delta em calendarView em um calendário de grupo</span><span class="sxs-lookup"><span data-stu-id="651dc-153">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="651dc-154">Para obter alterações incrementais em um modo de exibição de calendário do _calendário de um grupo_ :</span><span class="sxs-lookup"><span data-stu-id="651dc-154">To get incremental changes in a calendar view of _a group's calendar_ :</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="651dc-155">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="651dc-155">Query parameters</span></span>

<span data-ttu-id="651dc-156">As alterações de controle provocam uma rodada de uma ou mais chamadas de função **Delta** .</span><span class="sxs-lookup"><span data-stu-id="651dc-156">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="651dc-157">Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**.</span><span class="sxs-lookup"><span data-stu-id="651dc-157">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="651dc-158">O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-158">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="651dc-159">Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente.</span><span class="sxs-lookup"><span data-stu-id="651dc-159">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="651dc-160">Em solicitações subsequentes, basta copiar e aplicar `nextLink` a `deltaLink` URL ou da resposta anterior, pois essa URL já inclui os parâmetros codificados e desejados.</span><span class="sxs-lookup"><span data-stu-id="651dc-160">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="651dc-161">Parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="651dc-161">Query parameter</span></span>      | <span data-ttu-id="651dc-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="651dc-162">Type</span></span>   |<span data-ttu-id="651dc-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="651dc-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="651dc-164">startDateTime</span><span class="sxs-lookup"><span data-stu-id="651dc-164">startDateTime</span></span>|<span data-ttu-id="651dc-165">String</span><span class="sxs-lookup"><span data-stu-id="651dc-165">String</span></span>|<span data-ttu-id="651dc-p109">A data e a hora de início do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="651dc-p109">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00". </span></span><br><span data-ttu-id="651dc-168">O fuso horário é especificado na parte de deslocamento de fuso horário do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` cabeçalho, se houver.</span><span class="sxs-lookup"><span data-stu-id="651dc-168">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="651dc-169">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="651dc-169">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="651dc-170">Opcional para **Delta** em eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-170">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="651dc-171">Obrigatório para **Delta** no **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="651dc-171">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="651dc-172">endDateTime</span><span class="sxs-lookup"><span data-stu-id="651dc-172">endDateTime</span></span>|<span data-ttu-id="651dc-173">String</span><span class="sxs-lookup"><span data-stu-id="651dc-173">String</span></span>|<span data-ttu-id="651dc-p111">A data e a hora de término do intervalo de tempo, representadas no formato ISO 8601. Por exemplo, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="651dc-p111">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00". </span></span><br><span data-ttu-id="651dc-176">O fuso horário é especificado na parte de deslocamento de fuso horário do valor do parâmetro e não é afetado pelo `Prefer: outlook.timezone` cabeçalho, se houver.</span><span class="sxs-lookup"><span data-stu-id="651dc-176">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="651dc-177">Se nenhum deslocamento de fuso horário estiver incluído no valor, ele será interpretado como UTC.</span><span class="sxs-lookup"><span data-stu-id="651dc-177">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="651dc-178">_Não há suporte para_ **Delta** em eventos em um calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-178">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="651dc-179">Obrigatório para **Delta** no **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="651dc-179">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="651dc-180">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="651dc-180">$deltatoken</span></span> | <span data-ttu-id="651dc-181">string</span><span class="sxs-lookup"><span data-stu-id="651dc-181">string</span></span> | <span data-ttu-id="651dc-p113">Um [token de estado](/graph/delta-query-overview) retornado na URL `deltaLink` da chamada de função **delta** anterior do mesmo modo de exibição de calendário, indicando a conclusão da série de controle de alterações. Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle do modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-p113">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="651dc-184">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="651dc-184">$skiptoken</span></span> | <span data-ttu-id="651dc-185">string</span><span class="sxs-lookup"><span data-stu-id="651dc-185">string</span></span> | <span data-ttu-id="651dc-186">Um [token de estado](/graph/delta-query-overview) retornado na URL `nextLink` da chamada de função **delta** anterior indicando que não há mais alterações a serem controladas no mesmo modo de exibição de calendário.</span><span class="sxs-lookup"><span data-stu-id="651dc-186">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="651dc-187">O não suporta `$expand` , `$filter` , `$orderby` , `$select` e `$search` .</span><span class="sxs-lookup"><span data-stu-id="651dc-187">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="651dc-188">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-188">Request headers</span></span>
| <span data-ttu-id="651dc-189">Nome</span><span class="sxs-lookup"><span data-stu-id="651dc-189">Name</span></span>       | <span data-ttu-id="651dc-190">Tipo</span><span class="sxs-lookup"><span data-stu-id="651dc-190">Type</span></span> | <span data-ttu-id="651dc-191">Descrição</span><span class="sxs-lookup"><span data-stu-id="651dc-191">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="651dc-192">Autorização</span><span class="sxs-lookup"><span data-stu-id="651dc-192">Authorization</span></span>  | <span data-ttu-id="651dc-193">string</span><span class="sxs-lookup"><span data-stu-id="651dc-193">string</span></span>  | <span data-ttu-id="651dc-p114">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651dc-p114">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="651dc-196">Content-Type</span><span class="sxs-lookup"><span data-stu-id="651dc-196">Content-Type</span></span>  | <span data-ttu-id="651dc-197">string</span><span class="sxs-lookup"><span data-stu-id="651dc-197">string</span></span>  | <span data-ttu-id="651dc-p115">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651dc-p115">application/json. Required.</span></span> |
| <span data-ttu-id="651dc-200">Preferir</span><span class="sxs-lookup"><span data-stu-id="651dc-200">Prefer</span></span> | <span data-ttu-id="651dc-201">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="651dc-201">string</span></span>  | <span data-ttu-id="651dc-p116">odata.maxpagesize={x}. Opcional.</span><span class="sxs-lookup"><span data-stu-id="651dc-p116">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="651dc-204">Preferir</span><span class="sxs-lookup"><span data-stu-id="651dc-204">Prefer</span></span> | <span data-ttu-id="651dc-205">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="651dc-205">string</span></span> | <span data-ttu-id="651dc-206">Outlook. TimeZone = {cadeia de caracteres de fuso horário}.</span><span class="sxs-lookup"><span data-stu-id="651dc-206">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="651dc-207">Opcional, supõe-se o UTC se estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="651dc-207">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="651dc-208">Resposta</span><span class="sxs-lookup"><span data-stu-id="651dc-208">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="651dc-209">Função Delta em eventos (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="651dc-209">Delta function on events (preview)</span></span>
<span data-ttu-id="651dc-210">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [eventos](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-210">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="651dc-211">Cada **evento** na resposta contém apenas as propriedades **ID** , **Type** , **Start** e **end** por motivos de desempenho.</span><span class="sxs-lookup"><span data-stu-id="651dc-211">Each **event** in the response contains only the **id** , **type** , **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="651dc-212">Use `GET /events/{id}` subsequentemente para expandir qualquer evento da resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-212">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="651dc-213">Função Delta no calendarView</span><span class="sxs-lookup"><span data-stu-id="651dc-213">Delta function on calendarView</span></span>
<span data-ttu-id="651dc-214">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de [eventos](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-214">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="651dc-215">Espere obter todas as propriedades que você normalmente receberia de uma `GET /calendarview` solicitação.</span><span class="sxs-lookup"><span data-stu-id="651dc-215">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="651dc-216">Exemplos</span><span class="sxs-lookup"><span data-stu-id="651dc-216">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="651dc-217">Exemplo 1: função Delta em eventos em um calendário (visualização)</span><span class="sxs-lookup"><span data-stu-id="651dc-217">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="651dc-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-218">Request</span></span>
<span data-ttu-id="651dc-219">O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário padrão do usuário conectado, que ocorre no ou após o parâmetro especificado `startDateTime` .</span><span class="sxs-lookup"><span data-stu-id="651dc-219">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="651dc-220">A solicitação inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="651dc-220">The initial request does not include any state token.</span></span> 

<span data-ttu-id="651dc-221">A solicitação usa o `Prefer: odata.maxpagesize` cabeçalho para limitar o número máximo de eventos em cada resposta a 1.</span><span class="sxs-lookup"><span data-stu-id="651dc-221">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="651dc-222">Continue chamando a `delta` função usando a consulta retornada no `@odata.nextLink` até obter um `@odata.deltaLink` na resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-222">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="651dc-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="651dc-223">Response</span></span>

<span data-ttu-id="651dc-224">Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que pode ser um _skipToken_ (em um cabeçalho de resposta _\@ OData. Nextlink_ ) ou um _deltaToken_ (em um cabeçalho de resposta _\@ OData. deltaLink_ ).</span><span class="sxs-lookup"><span data-stu-id="651dc-224">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="651dc-225">Respectivamente, eles indicam se você deve continuar com a rodada ou se concluiu a obter todas as alterações para essa rodada.</span><span class="sxs-lookup"><span data-stu-id="651dc-225">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="651dc-226">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _\@ OData. nextLink_ .</span><span class="sxs-lookup"><span data-stu-id="651dc-226">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

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


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="651dc-227">Exemplo 2: função Delta no calendarView</span><span class="sxs-lookup"><span data-stu-id="651dc-227">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="651dc-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-228">Request</span></span>

<span data-ttu-id="651dc-229">O exemplo a seguir mostra a solicitação de sincronização inicial para obter eventos no calendário especificado do usuário conectado, dentro do intervalo de datas indicado pelo **calendarView**.</span><span class="sxs-lookup"><span data-stu-id="651dc-229">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="651dc-230">A solicitação inicial não inclui nenhum token de estado.</span><span class="sxs-lookup"><span data-stu-id="651dc-230">The initial request does not include any state token.</span></span> 

<span data-ttu-id="651dc-231">A solicitação usa o `Prefer: odata.maxpagesize` cabeçalho para limitar o número máximo de eventos em cada resposta a 2.</span><span class="sxs-lookup"><span data-stu-id="651dc-231">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="651dc-232">Continue chamando a `delta` função usando a consulta retornada no `@odata.nextLink` até obter todos os eventos nesse modo de exibição de calendário e a `@odata.deltaLink` na resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-232">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="651dc-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="651dc-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="651dc-234">C#</span><span class="sxs-lookup"><span data-stu-id="651dc-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="651dc-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="651dc-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="651dc-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="651dc-236">Response</span></span>

<span data-ttu-id="651dc-237">Se a solicitação for bem-sucedida, a resposta incluirá um token de estado, que pode ser um _skipToken_ (em um cabeçalho de resposta _\@ OData. Nextlink_ ) ou um _deltaToken_ (em um cabeçalho de resposta _\@ OData. deltaLink_ ).</span><span class="sxs-lookup"><span data-stu-id="651dc-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="651dc-238">Respectivamente, eles indicam se você deve continuar com a rodada ou se concluiu a obter todas as alterações para essa rodada.</span><span class="sxs-lookup"><span data-stu-id="651dc-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="651dc-239">A resposta abaixo mostra um _skipToken_ em um cabeçalho de resposta _\@ OData. nextLink_ .</span><span class="sxs-lookup"><span data-stu-id="651dc-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="651dc-240">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="651dc-240">Note: The response object shown here may be truncated for brevity.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="651dc-241">Confira também</span><span class="sxs-lookup"><span data-stu-id="651dc-241">See also</span></span>

- [<span data-ttu-id="651dc-242">Consulta delta do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="651dc-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="651dc-243">Obter as alterações incrementais para os eventos em uma pasta</span><span class="sxs-lookup"><span data-stu-id="651dc-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

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


