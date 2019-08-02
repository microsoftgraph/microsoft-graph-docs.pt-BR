---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 564cea7760c7e91102ce47ab725b27871a3b6f86
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002801"
---
# <a name="update-event"></a><span data-ttu-id="92ed9-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="92ed9-103">Update event</span></span>

<span data-ttu-id="92ed9-104">Atualizar as propriedades do objeto [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="92ed9-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="92ed9-105">Ao atualizar o fuso horário da hora de início ou de término de um evento, primeiro [encontre os fusos horários com suporte](outlookuser-supportedtimezones.md) para garantir que você tenha definido apenas fusos horários que tenham sido configurados para o servidor de caixas de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="92ed9-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="92ed9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="92ed9-106">Permissions</span></span>
<span data-ttu-id="92ed9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92ed9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92ed9-109">Permission type</span></span>      | <span data-ttu-id="92ed9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92ed9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92ed9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92ed9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="92ed9-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92ed9-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="92ed9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92ed9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92ed9-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92ed9-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="92ed9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92ed9-115">Application</span></span> | <span data-ttu-id="92ed9-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="92ed9-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="92ed9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92ed9-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="92ed9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed9-118">Request headers</span></span>
| <span data-ttu-id="92ed9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="92ed9-119">Name</span></span>       | <span data-ttu-id="92ed9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ed9-120">Type</span></span> | <span data-ttu-id="92ed9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ed9-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="92ed9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="92ed9-122">Authorization</span></span>  | <span data-ttu-id="92ed9-123">string</span><span class="sxs-lookup"><span data-stu-id="92ed9-123">string</span></span>  | <span data-ttu-id="92ed9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92ed9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92ed9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed9-126">Request body</span></span>
<span data-ttu-id="92ed9-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="92ed9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="92ed9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92ed9-130">Property</span></span>     | <span data-ttu-id="92ed9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92ed9-131">Type</span></span>   |<span data-ttu-id="92ed9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92ed9-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92ed9-133">attendees</span><span class="sxs-lookup"><span data-stu-id="92ed9-133">attendees</span></span>|[<span data-ttu-id="92ed9-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="92ed9-134">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="92ed9-135">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-135">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="92ed9-136">corpo</span><span class="sxs-lookup"><span data-stu-id="92ed9-136">body</span></span>|[<span data-ttu-id="92ed9-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="92ed9-137">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="92ed9-138">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-138">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="92ed9-139">categories</span><span class="sxs-lookup"><span data-stu-id="92ed9-139">categories</span></span>|<span data-ttu-id="92ed9-140">String</span><span class="sxs-lookup"><span data-stu-id="92ed9-140">String</span></span>|<span data-ttu-id="92ed9-141">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="92ed9-142">end</span><span class="sxs-lookup"><span data-stu-id="92ed9-142">end</span></span>|<span data-ttu-id="92ed9-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="92ed9-143">DateTimeTimeZone</span></span>|<span data-ttu-id="92ed9-144">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="92ed9-144">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="92ed9-145">importância</span><span class="sxs-lookup"><span data-stu-id="92ed9-145">importance</span></span>|<span data-ttu-id="92ed9-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92ed9-146">String</span></span>|<span data-ttu-id="92ed9-147">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-147">The importance of the event.</span></span> <span data-ttu-id="92ed9-148">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="92ed9-148">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="92ed9-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="92ed9-149">isAllDay</span></span>|<span data-ttu-id="92ed9-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="92ed9-150">Boolean</span></span>|<span data-ttu-id="92ed9-151">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="92ed9-151">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="92ed9-152">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="92ed9-152">isReminderOn</span></span>|<span data-ttu-id="92ed9-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="92ed9-153">Boolean</span></span>|<span data-ttu-id="92ed9-154">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-154">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="92ed9-155">location</span><span class="sxs-lookup"><span data-stu-id="92ed9-155">location</span></span>|[<span data-ttu-id="92ed9-156">Location</span><span class="sxs-lookup"><span data-stu-id="92ed9-156">Location</span></span>](../resources/location.md)|<span data-ttu-id="92ed9-157">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-157">The location of the event.</span></span>|
|<span data-ttu-id="92ed9-158">locations</span><span class="sxs-lookup"><span data-stu-id="92ed9-158">locations</span></span>|<span data-ttu-id="92ed9-159">Coleção [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="92ed9-159">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="92ed9-160">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="92ed9-160">The locations where the event is held or attended from.</span></span> <span data-ttu-id="92ed9-161">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="92ed9-161">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="92ed9-162">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="92ed9-162">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="92ed9-163">recurrence</span><span class="sxs-lookup"><span data-stu-id="92ed9-163">recurrence</span></span>|[<span data-ttu-id="92ed9-164">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="92ed9-164">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="92ed9-165">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-165">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="92ed9-166">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="92ed9-166">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="92ed9-167">Int32</span><span class="sxs-lookup"><span data-stu-id="92ed9-167">Int32</span></span>|<span data-ttu-id="92ed9-168">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="92ed9-168">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="92ed9-169">responseRequested</span><span class="sxs-lookup"><span data-stu-id="92ed9-169">responseRequested</span></span>|<span data-ttu-id="92ed9-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="92ed9-170">Boolean</span></span>|<span data-ttu-id="92ed9-171">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="92ed9-171">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="92ed9-172">sensitivity</span><span class="sxs-lookup"><span data-stu-id="92ed9-172">sensitivity</span></span>|<span data-ttu-id="92ed9-173">String</span><span class="sxs-lookup"><span data-stu-id="92ed9-173">String</span></span>| <span data-ttu-id="92ed9-174">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="92ed9-174">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="92ed9-175">showAs</span><span class="sxs-lookup"><span data-stu-id="92ed9-175">showAs</span></span>|<span data-ttu-id="92ed9-176">String</span><span class="sxs-lookup"><span data-stu-id="92ed9-176">String</span></span>|<span data-ttu-id="92ed9-177">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="92ed9-177">The status to show.</span></span> <span data-ttu-id="92ed9-178">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="92ed9-178">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="92ed9-179">iniciar</span><span class="sxs-lookup"><span data-stu-id="92ed9-179">start</span></span>|<span data-ttu-id="92ed9-180">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="92ed9-180">DateTimeTimeZone</span></span>|<span data-ttu-id="92ed9-181">A data, a hora e o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-181">The date, time, and time zone that the event starts.</span></span> |
|<span data-ttu-id="92ed9-182">assunto</span><span class="sxs-lookup"><span data-stu-id="92ed9-182">subject</span></span>|<span data-ttu-id="92ed9-183">String</span><span class="sxs-lookup"><span data-stu-id="92ed9-183">String</span></span>|<span data-ttu-id="92ed9-184">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="92ed9-184">The text of the event's subject line.</span></span>|

<span data-ttu-id="92ed9-185">Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.</span><span class="sxs-lookup"><span data-stu-id="92ed9-185">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="92ed9-186">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="92ed9-186">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="92ed9-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ed9-187">Response</span></span>

<span data-ttu-id="92ed9-188">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92ed9-188">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="92ed9-189">**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="92ed9-189">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="92ed9-190">Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="92ed9-190">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="92ed9-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92ed9-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92ed9-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92ed9-192">Request</span></span>

<span data-ttu-id="92ed9-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92ed9-193">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="92ed9-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="92ed9-194">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="92ed9-195">C#</span><span class="sxs-lookup"><span data-stu-id="92ed9-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92ed9-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="92ed9-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92ed9-197">Java</span><span class="sxs-lookup"><span data-stu-id="92ed9-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92ed9-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="92ed9-198">Response</span></span>

<span data-ttu-id="92ed9-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92ed9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="92ed9-202">Confira também</span><span class="sxs-lookup"><span data-stu-id="92ed9-202">See also</span></span>

- [<span data-ttu-id="92ed9-203">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="92ed9-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="92ed9-204">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="92ed9-204">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="92ed9-205">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="92ed9-205">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
