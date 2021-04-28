---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8ff929216fa15859744a686090c522d810d3a8c3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054025"
---
# <a name="update-event"></a><span data-ttu-id="71fd3-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="71fd3-103">Update event</span></span>

<span data-ttu-id="71fd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71fd3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71fd3-105">Atualizar as propriedades do objeto [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="71fd3-105">Update the properties of the [event](../resources/event.md) object.</span></span>

<span data-ttu-id="71fd3-106">Ao atualizar o fuso horário da hora de início ou de término de um evento, primeiro [encontre os fusos horários com suporte](outlookuser-supportedtimezones.md) para garantir que você tenha definido apenas fusos horários que tenham sido configurados para o servidor de caixas de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="71fd3-106">When updating the time zone of the start or end time of an event, first [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

## <a name="permissions"></a><span data-ttu-id="71fd3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="71fd3-107">Permissions</span></span>
<span data-ttu-id="71fd3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71fd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71fd3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71fd3-110">Permission type</span></span>      | <span data-ttu-id="71fd3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71fd3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71fd3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71fd3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71fd3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71fd3-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="71fd3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71fd3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71fd3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71fd3-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="71fd3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71fd3-116">Application</span></span> | <span data-ttu-id="71fd3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71fd3-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="71fd3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71fd3-118">HTTP request</span></span>
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

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a><span data-ttu-id="71fd3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd3-119">Request headers</span></span>
| <span data-ttu-id="71fd3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71fd3-120">Name</span></span>       | <span data-ttu-id="71fd3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fd3-121">Type</span></span> | <span data-ttu-id="71fd3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fd3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71fd3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71fd3-123">Authorization</span></span>  | <span data-ttu-id="71fd3-124">string</span><span class="sxs-lookup"><span data-stu-id="71fd3-124">string</span></span>  | <span data-ttu-id="71fd3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71fd3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71fd3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd3-127">Request body</span></span>
<span data-ttu-id="71fd3-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="71fd3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="71fd3-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71fd3-131">Property</span></span>     | <span data-ttu-id="71fd3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="71fd3-132">Type</span></span>   |<span data-ttu-id="71fd3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="71fd3-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71fd3-134">attendees</span><span class="sxs-lookup"><span data-stu-id="71fd3-134">attendees</span></span>|[<span data-ttu-id="71fd3-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="71fd3-135">Attendee</span></span>](../resources/attendee.md)|<span data-ttu-id="71fd3-136">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-136">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="71fd3-137">corpo</span><span class="sxs-lookup"><span data-stu-id="71fd3-137">body</span></span>|[<span data-ttu-id="71fd3-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="71fd3-138">ItemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="71fd3-139">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-139">The body of the message associated with the event.</span></span>|
|<span data-ttu-id="71fd3-140">categories</span><span class="sxs-lookup"><span data-stu-id="71fd3-140">categories</span></span>|<span data-ttu-id="71fd3-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="71fd3-141">String collection</span></span>|<span data-ttu-id="71fd3-142">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="71fd3-143">end</span><span class="sxs-lookup"><span data-stu-id="71fd3-143">end</span></span>|<span data-ttu-id="71fd3-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="71fd3-144">DateTimeTimeZone</span></span>|<span data-ttu-id="71fd3-145">A data, a hora e o fuso horário em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="71fd3-145">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="71fd3-146">hideAttendees</span><span class="sxs-lookup"><span data-stu-id="71fd3-146">hideAttendees</span></span>|<span data-ttu-id="71fd3-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="71fd3-147">Boolean</span></span>|<span data-ttu-id="71fd3-148">Quando definido como `true`, cada participante só se vê na solicitação de reunião e na lista de **Rastreamento** da reunião.</span><span class="sxs-lookup"><span data-stu-id="71fd3-148">When set to `true`, each attendee only sees themselves in the meeting request and meeting **Tracking** list.</span></span> <span data-ttu-id="71fd3-149">O padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="71fd3-149">Default is false.</span></span>|
|<span data-ttu-id="71fd3-150">importance</span><span class="sxs-lookup"><span data-stu-id="71fd3-150">importance</span></span>|<span data-ttu-id="71fd3-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="71fd3-151">String</span></span>|<span data-ttu-id="71fd3-152">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-152">The importance of the event.</span></span> <span data-ttu-id="71fd3-153">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="71fd3-153">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="71fd3-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="71fd3-154">isAllDay</span></span>|<span data-ttu-id="71fd3-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="71fd3-155">Boolean</span></span>|<span data-ttu-id="71fd3-156">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="71fd3-156">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="71fd3-157">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="71fd3-157">isOnlineMeeting</span></span>|<span data-ttu-id="71fd3-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="71fd3-158">Boolean</span></span>| <span data-ttu-id="71fd3-159">`True` se o evento tem informações sobre a reunião online, caso contrário, `false`.</span><span class="sxs-lookup"><span data-stu-id="71fd3-159">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="71fd3-160">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="71fd3-160">Default is false.</span></span> <span data-ttu-id="71fd3-161">Opcional.</span><span class="sxs-lookup"><span data-stu-id="71fd3-161">Optional.</span></span>|
|<span data-ttu-id="71fd3-162">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="71fd3-162">isReminderOn</span></span>|<span data-ttu-id="71fd3-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="71fd3-163">Boolean</span></span>|<span data-ttu-id="71fd3-164">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-164">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="71fd3-165">location</span><span class="sxs-lookup"><span data-stu-id="71fd3-165">location</span></span>|[<span data-ttu-id="71fd3-166">Location</span><span class="sxs-lookup"><span data-stu-id="71fd3-166">Location</span></span>](../resources/location.md)|<span data-ttu-id="71fd3-167">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-167">The location of the event.</span></span>|
|<span data-ttu-id="71fd3-168">locations</span><span class="sxs-lookup"><span data-stu-id="71fd3-168">locations</span></span>|<span data-ttu-id="71fd3-169">Coleção [location](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="71fd3-169">[location](../resources/location.md) collection</span></span>|<span data-ttu-id="71fd3-170">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="71fd3-170">The locations where the event is held or attended from.</span></span> <span data-ttu-id="71fd3-171">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="71fd3-171">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="71fd3-172">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="71fd3-172">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="71fd3-173">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="71fd3-173">onlineMeetingProvider</span></span>|<span data-ttu-id="71fd3-174">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="71fd3-174">onlineMeetingProviderType</span></span>| <span data-ttu-id="71fd3-175">Representa o provedor de serviços de reunião online.</span><span class="sxs-lookup"><span data-stu-id="71fd3-175">Represents the online meeting service provider.</span></span> <span data-ttu-id="71fd3-176">Os valores possíveis são `teamsForBusiness`, `skypeForBusiness` e `skypeForConsumer`.</span><span class="sxs-lookup"><span data-stu-id="71fd3-176">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="71fd3-177">Opcional.</span><span class="sxs-lookup"><span data-stu-id="71fd3-177">Optional.</span></span> |
|<span data-ttu-id="71fd3-178">recurrence</span><span class="sxs-lookup"><span data-stu-id="71fd3-178">recurrence</span></span>|[<span data-ttu-id="71fd3-179">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="71fd3-179">PatternedRecurrence</span></span>](../resources/patternedrecurrence.md)|<span data-ttu-id="71fd3-180">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-180">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="71fd3-181">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="71fd3-181">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="71fd3-182">Int32</span><span class="sxs-lookup"><span data-stu-id="71fd3-182">Int32</span></span>|<span data-ttu-id="71fd3-183">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="71fd3-183">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="71fd3-184">responseRequested</span><span class="sxs-lookup"><span data-stu-id="71fd3-184">responseRequested</span></span>|<span data-ttu-id="71fd3-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="71fd3-185">Boolean</span></span>|<span data-ttu-id="71fd3-186">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="71fd3-186">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="71fd3-187">sensitivity</span><span class="sxs-lookup"><span data-stu-id="71fd3-187">sensitivity</span></span>|<span data-ttu-id="71fd3-188">String</span><span class="sxs-lookup"><span data-stu-id="71fd3-188">String</span></span>| <span data-ttu-id="71fd3-189">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="71fd3-189">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="71fd3-190">showAs</span><span class="sxs-lookup"><span data-stu-id="71fd3-190">showAs</span></span>|<span data-ttu-id="71fd3-191">String</span><span class="sxs-lookup"><span data-stu-id="71fd3-191">String</span></span>|<span data-ttu-id="71fd3-192">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="71fd3-192">The status to show.</span></span> <span data-ttu-id="71fd3-193">Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="71fd3-193">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="71fd3-194">iniciar</span><span class="sxs-lookup"><span data-stu-id="71fd3-194">start</span></span>|<span data-ttu-id="71fd3-195">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="71fd3-195">DateTimeTimeZone</span></span>|<span data-ttu-id="71fd3-196">A data, a hora e o fuso horário do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-196">The start date, time, and time zone of the event.</span></span> |
|<span data-ttu-id="71fd3-197">assunto</span><span class="sxs-lookup"><span data-stu-id="71fd3-197">subject</span></span>|<span data-ttu-id="71fd3-198">String</span><span class="sxs-lookup"><span data-stu-id="71fd3-198">String</span></span>|<span data-ttu-id="71fd3-199">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="71fd3-199">The text of the event's subject line.</span></span>|

<span data-ttu-id="71fd3-200">Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.</span><span class="sxs-lookup"><span data-stu-id="71fd3-200">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>  
  
<span data-ttu-id="71fd3-201">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="71fd3-201">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>  

## <a name="response"></a><span data-ttu-id="71fd3-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fd3-202">Response</span></span>

<span data-ttu-id="71fd3-203">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71fd3-203">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>  

><span data-ttu-id="71fd3-204">**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="71fd3-204">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="71fd3-205">Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="71fd3-205">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="71fd3-206">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71fd3-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="71fd3-207">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71fd3-207">Request</span></span>

<span data-ttu-id="71fd3-208">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71fd3-208">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71fd3-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="71fd3-209">HTTP</span></span>](#tab/http)
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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "categories": ["Red category"]
}
```
# <a name="c"></a>[<span data-ttu-id="71fd3-210">C#</span><span class="sxs-lookup"><span data-stu-id="71fd3-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71fd3-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71fd3-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71fd3-212">Java</span><span class="sxs-lookup"><span data-stu-id="71fd3-212">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71fd3-213">Resposta</span><span class="sxs-lookup"><span data-stu-id="71fd3-213">Response</span></span>

<span data-ttu-id="71fd3-214">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71fd3-214">Here is an example of the response.</span></span> <span data-ttu-id="71fd3-215">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="71fd3-215">Note: The response object shown here might be shortened for readability.</span></span>

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
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness",
  "isReminderOn": true,
  "hideAttendees": false,
  "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+91 22 6241 6885"
  }
}
```

## <a name="see-also"></a><span data-ttu-id="71fd3-216">Confira também</span><span class="sxs-lookup"><span data-stu-id="71fd3-216">See also</span></span>

- [<span data-ttu-id="71fd3-217">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="71fd3-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="71fd3-218">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="71fd3-218">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="71fd3-219">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="71fd3-219">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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

