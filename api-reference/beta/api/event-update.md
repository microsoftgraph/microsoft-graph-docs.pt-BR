---
title: Atualizar evento
description: Atualizar as propriedades do objeto evento.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0c9b182d4a586b43aead0023651844dc98581da0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33586368"
---
# <a name="update-event"></a><span data-ttu-id="1fae7-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="1fae7-103">Update event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fae7-104">Atualizar as propriedades do objeto [evento](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="1fae7-104">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fae7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1fae7-105">Permissions</span></span>
<span data-ttu-id="1fae7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fae7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fae7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1fae7-108">Permission type</span></span>      | <span data-ttu-id="1fae7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1fae7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fae7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1fae7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1fae7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fae7-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1fae7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1fae7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fae7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fae7-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="1fae7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1fae7-114">Application</span></span> | <span data-ttu-id="1fae7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fae7-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fae7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1fae7-116">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="1fae7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1fae7-117">Request headers</span></span>
| <span data-ttu-id="1fae7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1fae7-118">Name</span></span>       | <span data-ttu-id="1fae7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fae7-119">Type</span></span> | <span data-ttu-id="1fae7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fae7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1fae7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1fae7-121">Authorization</span></span>  | <span data-ttu-id="1fae7-122">string</span><span class="sxs-lookup"><span data-stu-id="1fae7-122">string</span></span>  | <span data-ttu-id="1fae7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1fae7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fae7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1fae7-125">Request body</span></span>
<span data-ttu-id="1fae7-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="1fae7-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1fae7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fae7-129">Property</span></span>       | <span data-ttu-id="1fae7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fae7-130">Type</span></span>    | <span data-ttu-id="1fae7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fae7-131">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="1fae7-132">attendees</span><span class="sxs-lookup"><span data-stu-id="1fae7-132">attendees</span></span>|<span data-ttu-id="1fae7-133">Attendee</span><span class="sxs-lookup"><span data-stu-id="1fae7-133">Attendee</span></span>|<span data-ttu-id="1fae7-134">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-134">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="1fae7-135">corpo</span><span class="sxs-lookup"><span data-stu-id="1fae7-135">body</span></span>|<span data-ttu-id="1fae7-136">ItemBody</span><span class="sxs-lookup"><span data-stu-id="1fae7-136">ItemBody</span></span>|<span data-ttu-id="1fae7-137">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-137">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="1fae7-138">categories</span><span class="sxs-lookup"><span data-stu-id="1fae7-138">categories</span></span>|<span data-ttu-id="1fae7-139">String</span><span class="sxs-lookup"><span data-stu-id="1fae7-139">String</span></span>|<span data-ttu-id="1fae7-140">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-140">The categories associated with the event.</span></span>|
| <span data-ttu-id="1fae7-141">end</span><span class="sxs-lookup"><span data-stu-id="1fae7-141">end</span></span>|<span data-ttu-id="1fae7-142">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1fae7-142">DateTimeTimeZone</span></span>|<span data-ttu-id="1fae7-143">A data e a hora em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="1fae7-143">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="1fae7-p104">Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="1fae7-p104">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="1fae7-147">Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1fae7-147">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="1fae7-148">importance</span><span class="sxs-lookup"><span data-stu-id="1fae7-148">importance</span></span>|<span data-ttu-id="1fae7-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fae7-149">String</span></span>|<span data-ttu-id="1fae7-150">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-150">The importance of the event.</span></span> <span data-ttu-id="1fae7-151">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="1fae7-151">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="1fae7-152">isAllDay</span><span class="sxs-lookup"><span data-stu-id="1fae7-152">isAllDay</span></span>|<span data-ttu-id="1fae7-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fae7-153">Boolean</span></span>|<span data-ttu-id="1fae7-154">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="1fae7-154">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="1fae7-155">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="1fae7-155">isReminderOn</span></span>|<span data-ttu-id="1fae7-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fae7-156">Boolean</span></span>|<span data-ttu-id="1fae7-157">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-157">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="1fae7-158">location</span><span class="sxs-lookup"><span data-stu-id="1fae7-158">location</span></span>|<span data-ttu-id="1fae7-159">Locais</span><span class="sxs-lookup"><span data-stu-id="1fae7-159">Location</span></span>|<span data-ttu-id="1fae7-160">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-160">The location of the event.</span></span>|
|<span data-ttu-id="1fae7-161">locations</span><span class="sxs-lookup"><span data-stu-id="1fae7-161">locations</span></span>|<span data-ttu-id="1fae7-162">[location](../resources/location.md) collection</span><span class="sxs-lookup"><span data-stu-id="1fae7-162">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="1fae7-163">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="1fae7-163">The locations where the event is held or attended from.</span></span> <span data-ttu-id="1fae7-164">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="1fae7-164">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="1fae7-165">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="1fae7-165">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="1fae7-166">recurrence</span><span class="sxs-lookup"><span data-stu-id="1fae7-166">recurrence</span></span>|<span data-ttu-id="1fae7-167">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="1fae7-167">PatternedRecurrence</span></span>|<span data-ttu-id="1fae7-168">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-168">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="1fae7-169">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="1fae7-169">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="1fae7-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1fae7-170">Int32</span></span>|<span data-ttu-id="1fae7-171">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="1fae7-171">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="1fae7-172">responseRequested</span><span class="sxs-lookup"><span data-stu-id="1fae7-172">responseRequested</span></span>|<span data-ttu-id="1fae7-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="1fae7-173">Boolean</span></span>|<span data-ttu-id="1fae7-174">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="1fae7-174">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="1fae7-175">sensitivity</span><span class="sxs-lookup"><span data-stu-id="1fae7-175">sensitivity</span></span>|<span data-ttu-id="1fae7-176">String</span><span class="sxs-lookup"><span data-stu-id="1fae7-176">String</span></span>| <span data-ttu-id="1fae7-177">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="1fae7-177">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="1fae7-178">showAs</span><span class="sxs-lookup"><span data-stu-id="1fae7-178">showAs</span></span>|<span data-ttu-id="1fae7-179">String</span><span class="sxs-lookup"><span data-stu-id="1fae7-179">String</span></span>|<span data-ttu-id="1fae7-180">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="1fae7-180">The status to show.</span></span> <span data-ttu-id="1fae7-181">Os valores possíveis são `free` : `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`,.</span><span class="sxs-lookup"><span data-stu-id="1fae7-181">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="1fae7-182">iniciar</span><span class="sxs-lookup"><span data-stu-id="1fae7-182">start</span></span>|<span data-ttu-id="1fae7-183">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="1fae7-183">DateTimeTimeZone</span></span>|<span data-ttu-id="1fae7-184">A hora de início do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-184">The start time of the event.</span></span> <br/><br/><span data-ttu-id="1fae7-p108">Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="1fae7-p108">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="1fae7-188">Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="1fae7-188">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="1fae7-189">subject</span><span class="sxs-lookup"><span data-stu-id="1fae7-189">subject</span></span>|<span data-ttu-id="1fae7-190">String</span><span class="sxs-lookup"><span data-stu-id="1fae7-190">String</span></span>|<span data-ttu-id="1fae7-191">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="1fae7-191">The text of the event's subject line.</span></span>|

<span data-ttu-id="1fae7-192">Como o recurso **evento** dá suporte as [extensões](/graph/extensibility-overview), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância do **evento** existente.</span><span class="sxs-lookup"><span data-stu-id="1fae7-192">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="1fae7-193">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, com vários participantes e com instâncias atualizadas separadamente, vários emails de notificação serão enviados: uma para a série mestre e um por instância que foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="1fae7-193">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="1fae7-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fae7-194">Response</span></span>

<span data-ttu-id="1fae7-195">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1fae7-195">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="1fae7-196">**Observação:** Esse método poderá retornar uma Resposta de Solicitação Incorreta HTTP 400 com um código de erro `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: A ocorrência modificada está cruzando ou se sobrepondo à ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="1fae7-196">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="1fae7-197">Isso indica que a atualização viola a seguinte restrição do Outlook nas exceções de recorrência: uma ocorrência não pode ser movida para ou antes do dia da ocorrência anterior e não pode ser movida para ou após o dia da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="1fae7-197">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="1fae7-198">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1fae7-198">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1fae7-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1fae7-199">Request</span></span>

<span data-ttu-id="1fae7-200">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1fae7-200">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="1fae7-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="1fae7-201">Response</span></span>
<span data-ttu-id="1fae7-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1fae7-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1fae7-205">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1fae7-205">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1fae7-206">Basic</span><span class="sxs-lookup"><span data-stu-id="1fae7-206">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_event-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fae7-207">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fae7-207">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_event-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


## <a name="see-also"></a><span data-ttu-id="1fae7-208">Confira também</span><span class="sxs-lookup"><span data-stu-id="1fae7-208">See also</span></span>

- [<span data-ttu-id="1fae7-209">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1fae7-209">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1fae7-210">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="1fae7-210">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1fae7-211">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="1fae7-211">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/event-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
