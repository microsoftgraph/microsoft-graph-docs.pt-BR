# <a name="update-event"></a><span data-ttu-id="2e9a2-101">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="2e9a2-101">Update event</span></span>

<span data-ttu-id="2e9a2-102">Atualize as propriedades do objeto event.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-102">Update the properties of event object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e9a2-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e9a2-103">Prerequisites</span></span>
<span data-ttu-id="2e9a2-104">Um dos seguintes **escopos** é necessário para executar esta API: *Calendars.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="2e9a2-104">One of the following **scopes** is required to execute this API: *Calendars.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="2e9a2-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e9a2-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2e9a2-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9a2-106">Request headers</span></span>
| <span data-ttu-id="2e9a2-107">Nome</span><span class="sxs-lookup"><span data-stu-id="2e9a2-107">Name</span></span>       | <span data-ttu-id="2e9a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e9a2-108">Type</span></span> | <span data-ttu-id="2e9a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e9a2-109">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e9a2-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e9a2-110">Authorization</span></span>  | <span data-ttu-id="2e9a2-111">string</span><span class="sxs-lookup"><span data-stu-id="2e9a2-111">string</span></span>  | <span data-ttu-id="2e9a2-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e9a2-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9a2-114">Request body</span></span>
<span data-ttu-id="2e9a2-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2e9a2-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e9a2-118">Property</span></span>     | <span data-ttu-id="2e9a2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e9a2-119">Type</span></span>   |<span data-ttu-id="2e9a2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e9a2-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e9a2-121">attendees</span><span class="sxs-lookup"><span data-stu-id="2e9a2-121">attendees</span></span>|[<span data-ttu-id="2e9a2-122">Attendee</span><span class="sxs-lookup"><span data-stu-id="2e9a2-122">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="2e9a2-123">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-123">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="2e9a2-124">corpo</span><span class="sxs-lookup"><span data-stu-id="2e9a2-124">body</span></span>|[<span data-ttu-id="2e9a2-125">ItemBody</span><span class="sxs-lookup"><span data-stu-id="2e9a2-125">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="2e9a2-126">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-126">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="2e9a2-127">categories</span><span class="sxs-lookup"><span data-stu-id="2e9a2-127">categories</span></span>|<span data-ttu-id="2e9a2-128">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-128">String</span></span>|<span data-ttu-id="2e9a2-129">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-129">The categories associated with the event.</span></span>|
|<span data-ttu-id="2e9a2-130">end</span><span class="sxs-lookup"><span data-stu-id="2e9a2-130">end</span></span>|[<span data-ttu-id="2e9a2-131">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e9a2-131">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2e9a2-132">A data e a hora em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-132">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="2e9a2-p103">Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Observe que, se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p103">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="2e9a2-136">Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="2e9a2-136">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="2e9a2-137">importance</span><span class="sxs-lookup"><span data-stu-id="2e9a2-137">importance</span></span>|<span data-ttu-id="2e9a2-138">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-138">String</span></span>|<span data-ttu-id="2e9a2-p104">A importância do evento: Low = 0, Normal = 1, High = 2. Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p104">The importance of the event: Low = 0, Normal = 1, High = 2. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2e9a2-141">isAllDay</span><span class="sxs-lookup"><span data-stu-id="2e9a2-141">isAllDay</span></span>|<span data-ttu-id="2e9a2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e9a2-142">Boolean</span></span>|<span data-ttu-id="2e9a2-143">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-143">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="2e9a2-144">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="2e9a2-144">isReminderOn</span></span>|<span data-ttu-id="2e9a2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e9a2-145">Boolean</span></span>|<span data-ttu-id="2e9a2-146">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-146">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="2e9a2-147">location</span><span class="sxs-lookup"><span data-stu-id="2e9a2-147">location</span></span>|[<span data-ttu-id="2e9a2-148">Location</span><span class="sxs-lookup"><span data-stu-id="2e9a2-148">Location</span></span>](../resources/location.md)|<span data-ttu-id="2e9a2-149">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-149">The location of the event.</span></span>|
|<span data-ttu-id="2e9a2-150">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="2e9a2-150">onlineMeetingUrl</span></span>|<span data-ttu-id="2e9a2-151">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-151">String</span></span>|<span data-ttu-id="2e9a2-152">Uma URL para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-152">A URL for an online meeting.</span></span>|
|<span data-ttu-id="2e9a2-153">recurrence</span><span class="sxs-lookup"><span data-stu-id="2e9a2-153">recurrence</span></span>|[<span data-ttu-id="2e9a2-154">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="2e9a2-154">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="2e9a2-155">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-155">The recurrence patern for the event.</span></span>|
|<span data-ttu-id="2e9a2-156">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="2e9a2-156">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="2e9a2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="2e9a2-157">Int32</span></span>|<span data-ttu-id="2e9a2-158">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-158">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="2e9a2-159">responseRequested</span><span class="sxs-lookup"><span data-stu-id="2e9a2-159">responseRequested</span></span>|<span data-ttu-id="2e9a2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e9a2-160">Boolean</span></span>|<span data-ttu-id="2e9a2-161">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-161">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="2e9a2-162">sensitivity</span><span class="sxs-lookup"><span data-stu-id="2e9a2-162">sensitivity</span></span>|<span data-ttu-id="2e9a2-163">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-163">String</span></span>| <span data-ttu-id="2e9a2-164">Os valores possíveis são: `Normal`, `Personal`, `Private`, `Confidential`.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-164">Possible values are: `Normal`, `Personal`, `Private`, `Confidential`.</span></span>|
|<span data-ttu-id="2e9a2-165">showAs</span><span class="sxs-lookup"><span data-stu-id="2e9a2-165">showAs</span></span>|<span data-ttu-id="2e9a2-166">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-166">String</span></span>|<span data-ttu-id="2e9a2-p105">O status a ser exibido: Free = 0, Tentative = 1, Busy = 2, Oof = 3, WorkingElsewhere = 4, Unknown = -1. Os valores possíveis são: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p105">The status to show: Free = 0, Tentative = 1, Busy = 2, Oof = 3, WorkingElsewhere = 4, Unknown = -1. Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.</span></span>|
|<span data-ttu-id="2e9a2-169">iniciar</span><span class="sxs-lookup"><span data-stu-id="2e9a2-169">start</span></span>|[<span data-ttu-id="2e9a2-170">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e9a2-170">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="2e9a2-171">A hora de início do evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-171">The start time of the event.</span></span> <br/><br/><span data-ttu-id="2e9a2-p106">Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Observe que, se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p106">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="2e9a2-175">Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="2e9a2-175">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="2e9a2-176">subject</span><span class="sxs-lookup"><span data-stu-id="2e9a2-176">subject</span></span>|<span data-ttu-id="2e9a2-177">String</span><span class="sxs-lookup"><span data-stu-id="2e9a2-177">String</span></span>|<span data-ttu-id="2e9a2-178">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-178">The text of the event's subject line.</span></span>|

<span data-ttu-id="2e9a2-179">Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **event** existente.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-179">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="2e9a2-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9a2-180">Response</span></span>

<span data-ttu-id="2e9a2-181">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-181">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2e9a2-182">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e9a2-182">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e9a2-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9a2-183">Request</span></span>
<span data-ttu-id="2e9a2-184">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-184">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
##### <a name="response"></a><span data-ttu-id="2e9a2-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9a2-185">Response</span></span>
<span data-ttu-id="2e9a2-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e9a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="2e9a2-189">Ver também</span><span class="sxs-lookup"><span data-stu-id="2e9a2-189">See also</span></span>

- [<span data-ttu-id="2e9a2-190">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="2e9a2-190">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2e9a2-191">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="2e9a2-191">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
