# <a name="update-event"></a><span data-ttu-id="282b1-101">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="282b1-101">Update event</span></span>

<span data-ttu-id="282b1-102">Atualizar as propriedades do objeto event.</span><span class="sxs-lookup"><span data-stu-id="282b1-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="282b1-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="282b1-103">Permissions</span></span>
<span data-ttu-id="282b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="282b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="282b1-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="282b1-106">Permission type</span></span>      | <span data-ttu-id="282b1-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="282b1-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="282b1-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="282b1-108">Delegated (work or school account)</span></span> | <span data-ttu-id="282b1-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="282b1-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="282b1-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="282b1-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="282b1-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="282b1-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="282b1-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="282b1-112">Application</span></span> | <span data-ttu-id="282b1-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="282b1-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="282b1-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="282b1-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="282b1-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="282b1-115">Request headers</span></span>
| <span data-ttu-id="282b1-116">Nome</span><span class="sxs-lookup"><span data-stu-id="282b1-116">Name</span></span>       | <span data-ttu-id="282b1-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="282b1-117">Type</span></span> | <span data-ttu-id="282b1-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="282b1-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="282b1-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="282b1-119">Authorization</span></span>  | <span data-ttu-id="282b1-120">string</span><span class="sxs-lookup"><span data-stu-id="282b1-120">string</span></span>  | <span data-ttu-id="282b1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="282b1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="282b1-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="282b1-123">Request body</span></span>
<span data-ttu-id="282b1-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="282b1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="282b1-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="282b1-127">Property</span></span>     | <span data-ttu-id="282b1-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="282b1-128">Type</span></span>   |<span data-ttu-id="282b1-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="282b1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="282b1-130">attendees</span><span class="sxs-lookup"><span data-stu-id="282b1-130">attendees</span></span>|[<span data-ttu-id="282b1-131">Attendee</span><span class="sxs-lookup"><span data-stu-id="282b1-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="282b1-132">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="282b1-133">corpo</span><span class="sxs-lookup"><span data-stu-id="282b1-133">body</span></span>|[<span data-ttu-id="282b1-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="282b1-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="282b1-135">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="282b1-136">categories</span><span class="sxs-lookup"><span data-stu-id="282b1-136">categories</span></span>|<span data-ttu-id="282b1-137">String</span><span class="sxs-lookup"><span data-stu-id="282b1-137">String</span></span>|<span data-ttu-id="282b1-138">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="282b1-139">end</span><span class="sxs-lookup"><span data-stu-id="282b1-139">end</span></span>|[<span data-ttu-id="282b1-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="282b1-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="282b1-141">A data e a hora em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="282b1-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="282b1-p104">Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Observe que, se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="282b1-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="282b1-145">Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="282b1-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="282b1-146">importance</span><span class="sxs-lookup"><span data-stu-id="282b1-146">importance</span></span>|<span data-ttu-id="282b1-147">String</span><span class="sxs-lookup"><span data-stu-id="282b1-147">String</span></span>|<span data-ttu-id="282b1-p105">A importância do evento: Low = 0, Normal = 1, High = 2. Os valores possíveis são: `Low`, `Normal`, `High`.</span><span class="sxs-lookup"><span data-stu-id="282b1-p105">The importance of the event: Low = 0, Normal = 1, High = 2. Possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="282b1-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="282b1-150">isAllDay</span></span>|<span data-ttu-id="282b1-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="282b1-151">Boolean</span></span>|<span data-ttu-id="282b1-152">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="282b1-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="282b1-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="282b1-153">isReminderOn</span></span>|<span data-ttu-id="282b1-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="282b1-154">Boolean</span></span>|<span data-ttu-id="282b1-155">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="282b1-156">location</span><span class="sxs-lookup"><span data-stu-id="282b1-156">location</span></span>|[<span data-ttu-id="282b1-157">Location</span><span class="sxs-lookup"><span data-stu-id="282b1-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="282b1-158">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-158">The location of the event.</span></span>|
|<span data-ttu-id="282b1-159">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="282b1-159">onlineMeetingUrl</span></span>|<span data-ttu-id="282b1-160">String</span><span class="sxs-lookup"><span data-stu-id="282b1-160">String</span></span>|<span data-ttu-id="282b1-161">Uma URL para uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="282b1-161">A URL for an online meeting.</span></span>|
|<span data-ttu-id="282b1-162">recurrence</span><span class="sxs-lookup"><span data-stu-id="282b1-162">recurrence</span></span>|[<span data-ttu-id="282b1-163">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="282b1-163">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="282b1-164">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-164">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="282b1-165">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="282b1-165">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="282b1-166">Int32</span><span class="sxs-lookup"><span data-stu-id="282b1-166">Int32</span></span>|<span data-ttu-id="282b1-167">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="282b1-167">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="282b1-168">responseRequested</span><span class="sxs-lookup"><span data-stu-id="282b1-168">responseRequested</span></span>|<span data-ttu-id="282b1-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="282b1-169">Boolean</span></span>|<span data-ttu-id="282b1-170">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="282b1-170">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="282b1-171">sensitivity</span><span class="sxs-lookup"><span data-stu-id="282b1-171">sensitivity</span></span>|<span data-ttu-id="282b1-172">String</span><span class="sxs-lookup"><span data-stu-id="282b1-172">String</span></span>| <span data-ttu-id="282b1-173">Os valores possíveis são: `Normal`, `Personal`, `Private`, `Confidential`.</span><span class="sxs-lookup"><span data-stu-id="282b1-173">Possible values are: `Normal`, `Personal`, `Private`, `Confidential`.</span></span>|
|<span data-ttu-id="282b1-174">showAs</span><span class="sxs-lookup"><span data-stu-id="282b1-174">showAs</span></span>|<span data-ttu-id="282b1-175">String</span><span class="sxs-lookup"><span data-stu-id="282b1-175">String</span></span>|<span data-ttu-id="282b1-176">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="282b1-176">The status to show.</span></span> <span data-ttu-id="282b1-177">Os valores possíveis são: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere` e `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="282b1-177">Possible values are: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`.</span></span>|
|<span data-ttu-id="282b1-178">iniciar</span><span class="sxs-lookup"><span data-stu-id="282b1-178">start</span></span>|[<span data-ttu-id="282b1-179">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="282b1-179">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="282b1-180">A hora de início do evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-180">The start time of the event.</span></span> <br/><br/><span data-ttu-id="282b1-p107">Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Observe que, se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="282b1-p107">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="282b1-184">Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="282b1-184">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="282b1-185">subject</span><span class="sxs-lookup"><span data-stu-id="282b1-185">subject</span></span>|<span data-ttu-id="282b1-186">String</span><span class="sxs-lookup"><span data-stu-id="282b1-186">String</span></span>|<span data-ttu-id="282b1-187">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="282b1-187">The text of the event's subject line.</span></span>|

<span data-ttu-id="282b1-188">Como o recurso **event** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **event** existente.</span><span class="sxs-lookup"><span data-stu-id="282b1-188">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

## <a name="response"></a><span data-ttu-id="282b1-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="282b1-189">Response</span></span>

<span data-ttu-id="282b1-190">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="282b1-190">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="282b1-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="282b1-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="282b1-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="282b1-192">Request</span></span>

<span data-ttu-id="282b1-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="282b1-193">Here is an example of the request.</span></span>
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
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

##### <a name="response"></a><span data-ttu-id="282b1-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="282b1-194">Response</span></span>

<span data-ttu-id="282b1-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="282b1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```

## <a name="see-also"></a><span data-ttu-id="282b1-198">Confira também</span><span class="sxs-lookup"><span data-stu-id="282b1-198">See also</span></span>

- [<span data-ttu-id="282b1-199">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="282b1-199">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="282b1-200">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="282b1-200">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
