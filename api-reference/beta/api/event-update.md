---
title: Atualizar evento
description: Atualize as propriedades do objeto event.
author: angelgolfer-ms
ms.openlocfilehash: 05612f50b038f491598b98c5661fac17238419df
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330671"
---
# <a name="update-event"></a><span data-ttu-id="f7194-103">Atualizar evento</span><span class="sxs-lookup"><span data-stu-id="f7194-103">Update event</span></span>

> <span data-ttu-id="f7194-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7194-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7194-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7194-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7194-106">Atualize as propriedades do objeto [event](../resources/event.md) .</span><span class="sxs-lookup"><span data-stu-id="f7194-106">Update the properties of the [event](../resources/event.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f7194-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7194-107">Permissions</span></span>
<span data-ttu-id="f7194-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7194-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7194-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7194-110">Permission type</span></span>      | <span data-ttu-id="f7194-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7194-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7194-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7194-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7194-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7194-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f7194-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7194-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7194-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7194-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f7194-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7194-116">Application</span></span> | <span data-ttu-id="f7194-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7194-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7194-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7194-118">HTTP request</span></span>
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
## <a name="request-headers"></a><span data-ttu-id="f7194-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7194-119">Request headers</span></span>
| <span data-ttu-id="f7194-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f7194-120">Name</span></span>       | <span data-ttu-id="f7194-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7194-121">Type</span></span> | <span data-ttu-id="f7194-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7194-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f7194-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7194-123">Authorization</span></span>  | <span data-ttu-id="f7194-124">string</span><span class="sxs-lookup"><span data-stu-id="f7194-124">string</span></span>  | <span data-ttu-id="f7194-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7194-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7194-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7194-127">Request body</span></span>
<span data-ttu-id="f7194-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f7194-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7194-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7194-131">Property</span></span>       | <span data-ttu-id="f7194-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7194-132">Type</span></span>    | <span data-ttu-id="f7194-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7194-133">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="f7194-134">attendees</span><span class="sxs-lookup"><span data-stu-id="f7194-134">attendees</span></span>|<span data-ttu-id="f7194-135">Attendee</span><span class="sxs-lookup"><span data-stu-id="f7194-135">Attendee</span></span>|<span data-ttu-id="f7194-136">A coleção de participantes do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-136">The collection of attendees for the event.</span></span>|
| <span data-ttu-id="f7194-137">corpo</span><span class="sxs-lookup"><span data-stu-id="f7194-137">body</span></span>|<span data-ttu-id="f7194-138">ItemBody</span><span class="sxs-lookup"><span data-stu-id="f7194-138">ItemBody</span></span>|<span data-ttu-id="f7194-139">O corpo da mensagem associada ao evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-139">The body of the message associated with the event.</span></span>|
| <span data-ttu-id="f7194-140">categories</span><span class="sxs-lookup"><span data-stu-id="f7194-140">categories</span></span>|<span data-ttu-id="f7194-141">String</span><span class="sxs-lookup"><span data-stu-id="f7194-141">String</span></span>|<span data-ttu-id="f7194-142">As categorias associadas ao evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-142">The categories associated with the event.</span></span>|
| <span data-ttu-id="f7194-143">end</span><span class="sxs-lookup"><span data-stu-id="f7194-143">end</span></span>|<span data-ttu-id="f7194-144">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f7194-144">DateTimeTimeZone</span></span>|<span data-ttu-id="f7194-145">A data e a hora em que o evento termina.</span><span class="sxs-lookup"><span data-stu-id="f7194-145">The date and time that the event ends.</span></span><br/><br/><span data-ttu-id="f7194-p105">Por padrão, a hora de término é em UTC. Você pode especificar um fuso horário opcional em EndTimeZone, expressar a hora de término nesse fuso horário e incluir uma diferença de tempo em relação a UTC. Se usar EndTimeZone, você deverá especificar um valor para StartTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="f7194-p105">By default, the end time is in UTC. You can specify an optional time zone in EndTimeZone, express the end time in that time zone, and include a time offset from UTC. Note that if you use EndTimeZone, you must specify a value for StartTimeZone as well.</span></span><br/><br/><span data-ttu-id="f7194-149">Este exemplo especifica 25 de fevereiro de 2015, 21: 34 na Hora Padrão do Pacífico: "2015-02-25T21:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="f7194-149">This example specifies February 25, 2015, 9:34pm in Pacific Standard Time: "2015-02-25T21:34:00-08:00".</span></span> |
| <span data-ttu-id="f7194-150">importance</span><span class="sxs-lookup"><span data-stu-id="f7194-150">importance</span></span>|<span data-ttu-id="f7194-151">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7194-151">String</span></span>|<span data-ttu-id="f7194-152">A importância do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-152">The importance of the event.</span></span> <span data-ttu-id="f7194-153">Os valores possíveis são: `low`, `normal`, `high`.</span><span class="sxs-lookup"><span data-stu-id="f7194-153">Possible values are: `low`, `normal`, `high`.</span></span>|
| <span data-ttu-id="f7194-154">isAllDay</span><span class="sxs-lookup"><span data-stu-id="f7194-154">isAllDay</span></span>|<span data-ttu-id="f7194-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7194-155">Boolean</span></span>|<span data-ttu-id="f7194-156">Defina como true se o evento durar o dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="f7194-156">Set to true if the event lasts all day.</span></span>|
| <span data-ttu-id="f7194-157">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="f7194-157">isReminderOn</span></span>|<span data-ttu-id="f7194-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7194-158">Boolean</span></span>|<span data-ttu-id="f7194-159">Defina como true se um alerta estiver definido para lembrar o usuário sobre o evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-159">Set to true if an alert is set to remind the user of the event.</span></span>|
| <span data-ttu-id="f7194-160">location</span><span class="sxs-lookup"><span data-stu-id="f7194-160">location</span></span>|<span data-ttu-id="f7194-161">Location</span><span class="sxs-lookup"><span data-stu-id="f7194-161">Location</span></span>|<span data-ttu-id="f7194-162">O local do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-162">The location of the event.</span></span>|
|<span data-ttu-id="f7194-163">locations</span><span class="sxs-lookup"><span data-stu-id="f7194-163">locations</span></span>|<span data-ttu-id="f7194-164">Coleção de [local](../resources/location.md)</span><span class="sxs-lookup"><span data-stu-id="f7194-164">[Location](../resources/location.md) collection</span></span>|<span data-ttu-id="f7194-165">Locais onde o evento é realizado ou onde participar.</span><span class="sxs-lookup"><span data-stu-id="f7194-165">The locations where the event is held or attended from.</span></span> <span data-ttu-id="f7194-166">As propriedades **location** e **locations** sempre correspondem entre si.</span><span class="sxs-lookup"><span data-stu-id="f7194-166">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="f7194-167">Se você atualizar a propriedade **location**, os locais anteriores na coleção **locations** deverão ser removidos e substituídos pelo novo valor **location**.</span><span class="sxs-lookup"><span data-stu-id="f7194-167">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
| <span data-ttu-id="f7194-168">recurrence</span><span class="sxs-lookup"><span data-stu-id="f7194-168">recurrence</span></span>|<span data-ttu-id="f7194-169">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f7194-169">PatternedRecurrence</span></span>|<span data-ttu-id="f7194-170">O padrão de recorrência do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-170">The recurrence pattern for the event.</span></span>|
| <span data-ttu-id="f7194-171">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f7194-171">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="f7194-172">Int32</span><span class="sxs-lookup"><span data-stu-id="f7194-172">Int32</span></span>|<span data-ttu-id="f7194-173">O número de minutos antes da hora de início do evento em que o alerta de lembrete ocorre.</span><span class="sxs-lookup"><span data-stu-id="f7194-173">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
| <span data-ttu-id="f7194-174">responseRequested</span><span class="sxs-lookup"><span data-stu-id="f7194-174">responseRequested</span></span>|<span data-ttu-id="f7194-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7194-175">Boolean</span></span>|<span data-ttu-id="f7194-176">Defina como true se o remetente quiser receber uma resposta quando o evento for aceito ou recusado.</span><span class="sxs-lookup"><span data-stu-id="f7194-176">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
| <span data-ttu-id="f7194-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="f7194-177">sensitivity</span></span>|<span data-ttu-id="f7194-178">String</span><span class="sxs-lookup"><span data-stu-id="f7194-178">String</span></span>| <span data-ttu-id="f7194-179">Os valores possíveis são: `normal`, `personal`, `private`, `confidential`.</span><span class="sxs-lookup"><span data-stu-id="f7194-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
| <span data-ttu-id="f7194-180">showAs</span><span class="sxs-lookup"><span data-stu-id="f7194-180">showAs</span></span>|<span data-ttu-id="f7194-181">String</span><span class="sxs-lookup"><span data-stu-id="f7194-181">String</span></span>|<span data-ttu-id="f7194-182">O status a ser exibido.</span><span class="sxs-lookup"><span data-stu-id="f7194-182">The status to show.</span></span> <span data-ttu-id="f7194-183">Os valores possíveis são: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f7194-183">Possible values are: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
| <span data-ttu-id="f7194-184">start</span><span class="sxs-lookup"><span data-stu-id="f7194-184">start</span></span>|<span data-ttu-id="f7194-185">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f7194-185">DateTimeTimeZone</span></span>|<span data-ttu-id="f7194-186">A hora de início do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-186">The start time of the event.</span></span> <br/><br/><span data-ttu-id="f7194-p109">Por padrão, a hora de início é em UTC. Você pode especificar um fuso horário opcional em StartTimeZone, expressar a hora de início no fuso horário correspondente e incluir uma diferença de tempo em relação a UTC. Se usar StartTimeZone, você deverá especificar um valor para EndTimeZone também.</span><span class="sxs-lookup"><span data-stu-id="f7194-p109">By default, the start time is in UTC. You can specify an optional time zone in StartTimeZone, express the start time in that time zone, and include a time offset from UTC. Note that if you use StartTimeZone, you must specify a value for EndTimeZone as well.</span></span><br/><br/><span data-ttu-id="f7194-190">Este exemplo especifica 25 de fevereiro de 2015, 19:34 na Hora Padrão do Pacífico: "2015-02-25T19:34:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="f7194-190">This example specifies February 25, 2015, 7:34pm in Pacific Standard Time: "2015-02-25T19:34:00-08:00".</span></span>  |
| <span data-ttu-id="f7194-191">subject</span><span class="sxs-lookup"><span data-stu-id="f7194-191">subject</span></span>|<span data-ttu-id="f7194-192">String</span><span class="sxs-lookup"><span data-stu-id="f7194-192">String</span></span>|<span data-ttu-id="f7194-193">O texto da linha de assunto do evento.</span><span class="sxs-lookup"><span data-stu-id="f7194-193">The text of the event's subject line.</span></span>|

<span data-ttu-id="f7194-194">Como o recurso de **evento** oferece suporte às [extensões](/graph/extensibility-overview), você pode usar o `PATCH` operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância existente do **evento** .</span><span class="sxs-lookup"><span data-stu-id="f7194-194">Because the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **event** instance.</span></span>

<span data-ttu-id="f7194-195">Se o **evento** que você está atualizando é o evento mestre de uma série recorrente, contém vários participantes e tem instâncias que foram atualizadas separadamente, notificação de vários emails serão enviadas: uma para a série de mestre e um por instância que tenha foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="f7194-195">If the **event** you're updating is the master event of a recurring series, contains multiple attendees, and has instances that have been updated separately, multiple notification emails will be sent out: one for the master series and one per instance that has been updated.</span></span>

## <a name="response"></a><span data-ttu-id="f7194-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7194-196">Response</span></span>

<span data-ttu-id="f7194-197">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [event](../resources/event.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7194-197">If successful, this method returns a `200 OK` response code and updated [event](../resources/event.md) object in the response body.</span></span>

><span data-ttu-id="f7194-198">**Observação:** Este método pode retornar uma resposta de HTTP 400 Solicitação incorreta com um código de erro de `ErrorOccurrenceCrossingBoundary` e a seguinte mensagem de erro: a ocorrência modificada é Cruzando ou sobrepostas ocorrência adjacente.</span><span class="sxs-lookup"><span data-stu-id="f7194-198">**Note:** This method can return an HTTP 400 Bad Request response with an error code of `ErrorOccurrenceCrossingBoundary` and the following error message: Modified occurrence is crossing or overlapping adjacent occurrence.</span></span> <span data-ttu-id="f7194-199">Isso indica que a atualização viola a seguinte restrição do Outlook em exceções de recorrência: uma ocorrência não pode ser transferida para ou antes do dia da ocorrência anterior e não podem ser movida para ou após o dia da ocorrência seguinte.</span><span class="sxs-lookup"><span data-stu-id="f7194-199">This indicates that the update violates the following Outlook restriction on recurrence exceptions: an occurrence cannot be moved to or before the day of the previous occurrence, and cannot be moved to or after the day of the following occurrence.</span></span>

## <a name="example"></a><span data-ttu-id="f7194-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7194-200">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7194-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7194-201">Request</span></span>

<span data-ttu-id="f7194-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7194-202">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f7194-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7194-203">Response</span></span>
<span data-ttu-id="f7194-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7194-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="f7194-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7194-207">See also</span></span>

- [<span data-ttu-id="f7194-208">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="f7194-208">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f7194-209">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="f7194-209">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f7194-210">Adicionar dados personalizados a grupos usando extensões do esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="f7194-210">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
