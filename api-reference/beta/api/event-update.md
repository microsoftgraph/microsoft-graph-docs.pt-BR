---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2393751cf7157cc807241f817080745a0aa49fa5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954428"
---
# <a name="update-event"></a><span data-ttu-id="af944-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="af944-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af944-104">Atualizar as propriedades do objeto [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="af944-104">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="af944-105">Ao atualizar o fuso horário da hora de início ou de término de um evento, primeiro [encontre os fusos horários com suporte](outlookuser-supportedtimezones.md) para certificar-se de que você definiu somente os fusos horários que foram configurados para o servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="af944-105">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="af944-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="af944-106">Permissions</span></span>
<span data-ttu-id="af944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af944-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="af944-109">Permission type</span></span>      | <span data-ttu-id="af944-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="af944-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af944-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="af944-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af944-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af944-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="af944-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="af944-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af944-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af944-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="af944-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="af944-115">Application</span></span> | <span data-ttu-id="af944-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="af944-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="af944-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="af944-117">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="af944-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="af944-118">Request headers</span></span>
| <span data-ttu-id="af944-119">Nome</span><span class="sxs-lookup"><span data-stu-id="af944-119">Name</span></span>       | <span data-ttu-id="af944-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="af944-120">Type</span></span> | <span data-ttu-id="af944-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="af944-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="af944-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="af944-122">Authorization</span></span>  | <span data-ttu-id="af944-123">string</span><span class="sxs-lookup"><span data-stu-id="af944-123">string</span></span>  | <span data-ttu-id="af944-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af944-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af944-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="af944-126">Request body</span></span>
<span data-ttu-id="af944-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="af944-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="af944-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af944-130">Property</span></span>       | <span data-ttu-id="af944-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="af944-131">Type</span></span>    | <span data-ttu-id="af944-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="af944-132">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="af944-133">attendees</span><span class="sxs-lookup"><span data-stu-id="af944-133">attendees</span></span>|<span data-ttu-id="af944-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="af944-134">Attendee</span></span>|<span data-ttu-id="af944-135">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-135">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="af944-136">corpo</span><span class="sxs-lookup"><span data-stu-id="af944-136">body</span></span>|<span data-ttu-id="af944-137">ItemBody</span><span class="sxs-lookup"><span data-stu-id="af944-137">ItemBody</span></span>|<span data-ttu-id="af944-138">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="af944-138">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="af944-139">categories</span><span class="sxs-lookup"><span data-stu-id="af944-139">categories</span></span>|<span data-ttu-id="af944-140">String</span><span class="sxs-lookup"><span data-stu-id="af944-140">String</span></span>|<span data-ttu-id="af944-141">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="af944-141">The categories associated with the event.</span></span>|
| <span data-ttu-id="af944-142">end</span><span class="sxs-lookup"><span data-stu-id="af944-142">end</span></span>|<span data-ttu-id="af944-143">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="af944-143">DateTimeTimeZone</span></span>|<span data-ttu-id="af944-144">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="af944-144">The date, time, and time zone that the event ends.</span></span> |
| <span data-ttu-id="af944-145">importance</span><span class="sxs-lookup"><span data-stu-id="af944-145">importance</span></span>|<span data-ttu-id="af944-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af944-146">String</span></span>|<span data-ttu-id="af944-147">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-147">The importance of the event.</span></span> <span data-ttu-id="af944-148">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="af944-148">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="af944-149">isAllDay</span><span class="sxs-lookup"><span data-stu-id="af944-149">isAllDay</span></span>|<span data-ttu-id="af944-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="af944-150">Boolean</span></span>|<span data-ttu-id="af944-151">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="af944-151">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="af944-152">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="af944-152">isReminderOn</span></span>|<span data-ttu-id="af944-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="af944-153">Boolean</span></span>|<span data-ttu-id="af944-154">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="af944-154">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="af944-155">location</span><span class="sxs-lookup"><span data-stu-id="af944-155">location</span></span>|<span data-ttu-id="af944-156">Locais</span><span class="sxs-lookup"><span data-stu-id="af944-156">Location</span></span>|<span data-ttu-id="af944-157">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-157">The location of the event.</span></span>|
|<span data-ttu-id="af944-158">locations</span><span class="sxs-lookup"><span data-stu-id="af944-158">locations</span></span>|<span data-ttu-id="af944-159">[location](../resources/location.md) collection</span><span class="sxs-lookup"><span data-stu-id="af944-159">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="af944-160">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="af944-160">The locations where the event is held or attended from.</span></span> <span data-ttu-id="af944-161">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="af944-161">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="af944-162">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="af944-162">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="af944-163">recurrence</span><span class="sxs-lookup"><span data-stu-id="af944-163">recurrence</span></span>|<span data-ttu-id="af944-164">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="af944-164">PatternedRecurrence</span></span>|<span data-ttu-id="af944-165">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-165">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="af944-166">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="af944-166">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="af944-167">Int32</span><span class="sxs-lookup"><span data-stu-id="af944-167">Int32</span></span>|<span data-ttu-id="af944-168">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="af944-168">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="af944-169">responseRequested</span><span class="sxs-lookup"><span data-stu-id="af944-169">responseRequested</span></span>|<span data-ttu-id="af944-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="af944-170">Boolean</span></span>|<span data-ttu-id="af944-171">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="af944-171">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="af944-172">sensitivity</span><span class="sxs-lookup"><span data-stu-id="af944-172">sensitivity</span></span>|<span data-ttu-id="af944-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af944-173">String</span></span>| <span data-ttu-id="af944-174">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="af944-174">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="af944-175">showAs</span><span class="sxs-lookup"><span data-stu-id="af944-175">showAs</span></span>|<span data-ttu-id="af944-176">String</span><span class="sxs-lookup"><span data-stu-id="af944-176">String</span></span>|<span data-ttu-id="af944-177">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="af944-177">The status to show.</span></span> <span data-ttu-id="af944-178">Os valores possíveis são `free` : `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`,.</span><span class="sxs-lookup"><span data-stu-id="af944-178">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="af944-179">iniciar</span><span class="sxs-lookup"><span data-stu-id="af944-179">start</span></span>|<span data-ttu-id="af944-180">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="af944-180">DateTimeTimeZone</span></span>|<span data-ttu-id="af944-181">A data de início, a hora e o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-181">The start date, time, and time zone of the event.</span></span> |
| <span data-ttu-id="af944-182">subject</span><span class="sxs-lookup"><span data-stu-id="af944-182">subject</span></span>|<span data-ttu-id="af944-183">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af944-183">String</span></span>|<span data-ttu-id="af944-184">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="af944-184">The text of the event's subject line.</span></span>|

<span data-ttu-id="af944-185">Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.</span><span class="sxs-lookup"><span data-stu-id="af944-185">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="af944-186">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="af944-186">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="af944-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="af944-187">Response</span></span>

<span data-ttu-id="af944-188">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="af944-188">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="af944-189">**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="af944-189">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="af944-190">Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="af944-190">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="af944-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="af944-191">Example</span></span>

##### <a name="request"></a><span data-ttu-id="af944-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="af944-192">Request</span></span>

<span data-ttu-id="af944-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="af944-193">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af944-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="af944-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af944-195">C#</span><span class="sxs-lookup"><span data-stu-id="af944-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af944-196">Javascript</span><span class="sxs-lookup"><span data-stu-id="af944-196">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="af944-197">Java</span><span class="sxs-lookup"><span data-stu-id="af944-197">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af944-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="af944-198">Response</span></span>
<span data-ttu-id="af944-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="af944-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a><span data-ttu-id="af944-202">Confira também</span><span class="sxs-lookup"><span data-stu-id="af944-202">See also</span></span>

- [<span data-ttu-id="af944-203">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="af944-203">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="af944-204">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="af944-204">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="af944-205">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="af944-205">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
