# <a name="update-event"></a><span data-ttu-id="37630-101">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="37630-101">Update event</span></span>

<span data-ttu-id="37630-102">Atualizar as propriedades do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="37630-102">Update the properties of event object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37630-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="37630-103">Permissions</span></span>
<span data-ttu-id="37630-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="37630-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="37630-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37630-106">Permission type</span></span>      | <span data-ttu-id="37630-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37630-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37630-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37630-108">Delegated (work or school account)</span></span> | <span data-ttu-id="37630-109">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37630-109">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="37630-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37630-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37630-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37630-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="37630-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37630-112">Application</span></span> | <span data-ttu-id="37630-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="37630-113">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="37630-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37630-114">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="37630-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37630-115">Request headers</span></span>
| <span data-ttu-id="37630-116">Nome</span><span class="sxs-lookup"><span data-stu-id="37630-116">Name</span></span>       | <span data-ttu-id="37630-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="37630-117">Type</span></span> | <span data-ttu-id="37630-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="37630-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="37630-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="37630-119">Authorization</span></span>  | <span data-ttu-id="37630-120">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-120">string</span></span>  | <span data-ttu-id="37630-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37630-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37630-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37630-123">Request body</span></span>
<span data-ttu-id="37630-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="37630-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37630-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37630-127">Property</span></span>     | <span data-ttu-id="37630-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="37630-128">Type</span></span>   |<span data-ttu-id="37630-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="37630-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37630-130">attendees</span><span class="sxs-lookup"><span data-stu-id="37630-130">attendees</span></span>|[<span data-ttu-id="37630-131">Attendee</span><span class="sxs-lookup"><span data-stu-id="37630-131">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="37630-132">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-132">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="37630-133">corpo</span><span class="sxs-lookup"><span data-stu-id="37630-133">body</span></span>|[<span data-ttu-id="37630-134">ItemBody</span><span class="sxs-lookup"><span data-stu-id="37630-134">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="37630-135">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="37630-135">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="37630-136">categories</span><span class="sxs-lookup"><span data-stu-id="37630-136">categories</span></span>|<span data-ttu-id="37630-137">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-137">String</span></span>|<span data-ttu-id="37630-138">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="37630-138">The categories associated with the event.</span></span>|
|<span data-ttu-id="37630-139">end</span><span class="sxs-lookup"><span data-stu-id="37630-139">end</span></span>|[<span data-ttu-id="37630-140">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="37630-140">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="37630-141">A data e a hora em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="37630-141">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="37630-p104">Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="37630-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="37630-145">Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="37630-145">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
|<span data-ttu-id="37630-146">importance</span><span class="sxs-lookup"><span data-stu-id="37630-146">importance</span></span>|<span data-ttu-id="37630-147">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-147">String</span></span>|<span data-ttu-id="37630-148">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-148">The importance of the event.</span></span> <span data-ttu-id="37630-149">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="37630-149">The possible values are:</span></span>|
|<span data-ttu-id="37630-150">isAllDay</span><span class="sxs-lookup"><span data-stu-id="37630-150">isAllDay</span></span>|<span data-ttu-id="37630-151">Booleano</span><span class="sxs-lookup"><span data-stu-id="37630-151">Boolean</span></span>|<span data-ttu-id="37630-152">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="37630-152">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="37630-153">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="37630-153">isReminderOn</span></span>|<span data-ttu-id="37630-154">Booleano</span><span class="sxs-lookup"><span data-stu-id="37630-154">Boolean</span></span>|<span data-ttu-id="37630-155">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="37630-155">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="37630-156">location</span><span class="sxs-lookup"><span data-stu-id="37630-156">location</span></span>|[<span data-ttu-id="37630-157">Location</span><span class="sxs-lookup"><span data-stu-id="37630-157">Location</span></span>](../resources/location.md)|<span data-ttu-id="37630-158">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-158">The location of the event.</span></span>|
|<span data-ttu-id="37630-159">locations</span><span class="sxs-lookup"><span data-stu-id="37630-159">locations</span></span>|<span data-ttu-id="37630-160">Coleção [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="37630-160">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="37630-161">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="37630-161">The locations where the event is held or attended from.</span></span> <span data-ttu-id="37630-162">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="37630-162">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="37630-163">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="37630-163">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="37630-164">recurrence</span><span class="sxs-lookup"><span data-stu-id="37630-164">recurrence</span></span>|[<span data-ttu-id="37630-165">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="37630-165">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="37630-166">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-166">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="37630-167">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="37630-167">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="37630-168">Int32</span><span class="sxs-lookup"><span data-stu-id="37630-168">Int32</span></span>|<span data-ttu-id="37630-169">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="37630-169">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="37630-170">responseRequested</span><span class="sxs-lookup"><span data-stu-id="37630-170">responseRequested</span></span>|<span data-ttu-id="37630-171">Booleano</span><span class="sxs-lookup"><span data-stu-id="37630-171">Boolean</span></span>|<span data-ttu-id="37630-172">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="37630-172">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="37630-173">sensitivity</span><span class="sxs-lookup"><span data-stu-id="37630-173">sensitivity</span></span>|<span data-ttu-id="37630-174">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-174">String</span></span>| <span data-ttu-id="37630-175">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="37630-175">The possible values are `normal`, `personal`, `private`, `confidential`, , , , , , , , or .</span></span>|
|<span data-ttu-id="37630-176">showAs</span><span class="sxs-lookup"><span data-stu-id="37630-176">showAs</span></span>|<span data-ttu-id="37630-177">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-177">String</span></span>|<span data-ttu-id="37630-178">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="37630-178">The status to show.</span></span> <span data-ttu-id="37630-179">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="37630-179">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|
|<span data-ttu-id="37630-180">iniciar</span><span class="sxs-lookup"><span data-stu-id="37630-180">start</span></span>|[<span data-ttu-id="37630-181">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="37630-181">DateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="37630-182">A hora de início do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-182">The start time of the event.</span></span> <br/><br/><span data-ttu-id="37630-p108">Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="37630-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="37630-186">Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="37630-186">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
|<span data-ttu-id="37630-187">subject</span><span class="sxs-lookup"><span data-stu-id="37630-187">subject</span></span>|<span data-ttu-id="37630-188">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="37630-188">String</span></span>|<span data-ttu-id="37630-189">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="37630-189">The text of the event's subject line.</span></span>|

<span data-ttu-id="37630-190">Como o recurso **event** oferece suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **event** existente.</span><span class="sxs-lookup"><span data-stu-id="37630-190">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="37630-191">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, contém vários participantes e tem instâncias que foram atualizadas separadamente, várias notificações por email serão enviadas: uma para a série mestra e um para cada instância que tenha foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="37630-191">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="37630-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="37630-192">Response</span></span>

<span data-ttu-id="37630-193">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37630-193">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="37630-194">**Observação:** Este método pode retornar uma resposta de HTTP 400 Solicitação incorreta com um código de erro de `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: a ocorrência modificada é cruzada ou sobreposta à ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="37630-194">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="37630-195">Isso indica que a atualização viola a seguinte restrição do Outlook em exceções de recorrência: uma ocorrência não pode ser transferida para o dia ou antes da ocorrência anterior e não pode ser transferida para o dia ou depois da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="37630-195">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="37630-196">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37630-196">Example</span></span>

##### <a name="request"></a><span data-ttu-id="37630-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37630-197">Request</span></span>

<span data-ttu-id="37630-198">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37630-198">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="37630-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="37630-199">Response</span></span>

<span data-ttu-id="37630-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37630-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="37630-203">Confira também</span><span class="sxs-lookup"><span data-stu-id="37630-203">See also</span></span>

- [<span data-ttu-id="37630-204">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="37630-204">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="37630-205">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="37630-205">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="37630-206">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="37630-206">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
