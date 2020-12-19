---
title: Criar evento
description: Crie um evento no calendário especificado ou no calendário padrão do usuário.
localization_priority: Priority
doc_type: apiPageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 94bdccb632b2bf02fe05a0a854d298d805ad77f3
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720032"
---
# <a name="create-event"></a><span data-ttu-id="d5b3c-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="d5b3c-103">Create Event</span></span>

<span data-ttu-id="d5b3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5b3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5b3c-105">Criar um [evento](../resources/event.md) no calendário padrão do usuário ou em um calendário específico.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-105">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="d5b3c-106">Por padrão, a propriedade **allowNewTimeProposals** está definida como verdadeira quando um evento é criado, o que significa que os convidados podem propor uma data/hora diferente para o evento.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-106">By default, the **allowNewTimeProposals** property is set to true when an event is created, which means invitees can propose a different date/time for the event.</span></span> <span data-ttu-id="d5b3c-107">Confira [Propor novos horários de reunião](/graph/outlook-calendar-meeting-proposals) para obter mais informações sobre como propor um horário e como receber e aceitar uma nova proposta de horário.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-107">See [Propose new meeting times](/graph/outlook-calendar-meeting-proposals) for more information on how to propose a time, and how to receive and accept a new time proposal.</span></span>

<span data-ttu-id="d5b3c-108">Você pode especificar o fuso horário de cada um dos horários de início e de término do evento como parte de seus valores, porque as propriedades **inicial** e **final** são do tipo [ dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-108">You can specify the time zone for each of the start and end times of the event as part of their values, because the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="d5b3c-109">Primeiro [localize os fusos horários com suporte](outlookuser-supportedtimezones.md) para garantir que você tenha definido somente fusos horários que tenham sido configurados para o servidor de caixas de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-109">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="d5b3c-110">Quando um evento é enviado, o servidor envia convites para os participantes.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-110">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="d5b3c-111">**Definir o local em um evento**</span><span class="sxs-lookup"><span data-stu-id="d5b3c-111">**Setting the location in an event**</span></span>

<span data-ttu-id="d5b3c-112">Um administrador do Exchange pode configurar um endereço de email e uma caixa de correio para um recurso como uma sala de reunião ou equipamento como um projetor.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-112">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="d5b3c-113">Os usuários podem convidar o recurso como um participante para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-113">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="d5b3c-114">Em nome do recurso, o servidor aceita ou recusa a solicitação de reunião com base na disponibilidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-114">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="d5b3c-115">Se o servidor aceitar uma reunião do recurso, ele criará um evento para a reunião no calendário do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-115">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="d5b3c-116">Se a reunião for reagendada, o servidor atualizará o evento no calendário do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-116">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="d5b3c-117">Outra vantagem de configurar uma caixa de correio para um recurso é controlar o agendamento do recurso. Por exemplo, somente executivos ou seus representantes podem agendar uma sala de reunião particular.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-117">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="d5b3c-118">Se você está organizando um evento que envolve um local de reunião:</span><span class="sxs-lookup"><span data-stu-id="d5b3c-118">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="d5b3c-119">Defina a propriedade **location** de **event** adequadamente.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-119">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="d5b3c-120">Defina a propriedade opcional **locationEmailAddress** se o local da reunião tiver um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-120">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="d5b3c-121">Além disso, se o local da reunião tiver sido configurado como um recurso ou se o evento envolver algum equipamento que tenha sido definido como um recurso:</span><span class="sxs-lookup"><span data-stu-id="d5b3c-121">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="d5b3c-122">Convide o recurso como um [participante](../resources/attendee.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-122">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="d5b3c-123">Defina a propriedade **type** do participante como `resource`.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-123">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="d5b3c-124">Defina o **emailAddress** do participante como o endereço de email do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-124">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="d5b3c-125">Permissões</span><span class="sxs-lookup"><span data-stu-id="d5b3c-125">Permissions</span></span>
<span data-ttu-id="d5b3c-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5b3c-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5b3c-128">Permission type</span></span>      | <span data-ttu-id="d5b3c-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d5b3c-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5b3c-130">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5b3c-130">Delegated (work or school account)</span></span> | <span data-ttu-id="d5b3c-131">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5b3c-131">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d5b3c-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5b3c-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5b3c-133">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5b3c-133">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d5b3c-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5b3c-134">Application</span></span> | <span data-ttu-id="d5b3c-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d5b3c-135">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5b3c-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b3c-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="d5b3c-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-137">Request headers</span></span>
| <span data-ttu-id="d5b3c-138">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5b3c-138">Header</span></span>       | <span data-ttu-id="d5b3c-139">Valor</span><span class="sxs-lookup"><span data-stu-id="d5b3c-139">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="d5b3c-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5b3c-140">Authorization</span></span>  | <span data-ttu-id="d5b3c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d5b3c-143">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d5b3c-143">Content-Type</span></span>  | <span data-ttu-id="d5b3c-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d5b3c-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-146">Request body</span></span>
<span data-ttu-id="d5b3c-147">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-147">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d5b3c-148">Como o recurso **event** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o evento ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-148">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="d5b3c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b3c-149">Response</span></span>

<span data-ttu-id="d5b3c-150">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-150">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5b3c-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d5b3c-151">Examples</span></span>

### <a name="example-1-create-an-event-in-the-specified-time-zone-and-assign-the-event-an-optional-transactionid-value"></a><span data-ttu-id="d5b3c-152">Exemplo 1: Crie um evento no fuso horário especificado e atribua um valor opcional transactionId ao evento.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-152">Example 1: Create an event in the specified time zone, and assign the event an optional transactionId value.</span></span>

#### <a name="request"></a><span data-ttu-id="d5b3c-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-153">Request</span></span>
<span data-ttu-id="d5b3c-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-154">Here is an example of the request.</span></span> <span data-ttu-id="d5b3c-155">Ela usa o cabeçalho da solicitação `Prefer: outlook.timezone` para especificar o fuso horário para as horas de início e fim na resposta.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-155">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the start and end times in the response.</span></span> <span data-ttu-id="d5b3c-156">Ele também define a propriedade **transactionId** para reduzir tentativas desnecessárias no servidor.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-156">It also sets the **transactionId** property to reduce unnecessary retries on the server.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5b3c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b3c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7"
}
```
# <a name="c"></a>[<span data-ttu-id="d5b3c-158">C#</span><span class="sxs-lookup"><span data-stu-id="d5b3c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b3c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b3c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b3c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b3c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b3c-161">Java</span><span class="sxs-lookup"><span data-stu-id="d5b3c-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d5b3c-162">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-162">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="d5b3c-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b3c-163">Response</span></span>
<span data-ttu-id="d5b3c-164">Veja um exemplo de resposta que exibe as propriedades **start** e **end** usando o fuso horário especificado no cabeçalho `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-164">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="d5b3c-165">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-165">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5b3c-166">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-166">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "transactionId":"7E163156-7762-4BEB-A1C6-729EA81755A7",
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting":false,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```


### <a name="example-2-create-an-event-that-occurs-in-multiple-locations"></a><span data-ttu-id="d5b3c-167">Exemplo 2: criar um evento que ocorrerá em vários locais</span><span class="sxs-lookup"><span data-stu-id="d5b3c-167">Example 2: Create an event that occurs in multiple locations</span></span>

#### <a name="request"></a><span data-ttu-id="d5b3c-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-168">Request</span></span>
<span data-ttu-id="d5b3c-169">A solicitação de exemplo a seguir especifica três locais de onde o organizador e os participantes podem participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-169">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="d5b3c-170">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-170">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5b3c-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b3c-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_multiple_locations"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 1390

{
  "subject": "Plan summer company picnic",
  "body": {
    "contentType": "HTML",
    "content": "Let's kick-start this event planning!"
  },
  "start": {
      "dateTime": "2017-08-30T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-08-30T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "DanaS@contoso.onmicrosoft.com",
        "name": "Dana Swope"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "AlexW@contoso.onmicrosoft.com",
        "name": "Alex Wilber"
      },
      "type": "Required"
    }
  ],
  "location": {
    "displayName": "Conf Room 3; Fourth Coffee; Home Office",
    "locationType": "Default"
  },
  "locations": [
    {
      "displayName": "Conf Room 3"
    },
    {
      "displayName": "Fourth Coffee",
      "address": {
        "street": "4567 Main St",
        "city": "Redmond",
        "state": "WA",
        "countryOrRegion": "US",
        "postalCode": "32008"
      },
      "coordinates": {
        "latitude": 47.672,
        "longitude": -102.103
      }
    },
    {
      "displayName": "Home Office"
    }
  ],
  "allowNewTimeProposals": true
}
```
# <a name="c"></a>[<span data-ttu-id="d5b3c-172">C#</span><span class="sxs-lookup"><span data-stu-id="d5b3c-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b3c-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b3c-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b3c-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b3c-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b3c-175">Java</span><span class="sxs-lookup"><span data-stu-id="d5b3c-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d5b3c-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b3c-176">Response</span></span>
<span data-ttu-id="d5b3c-177">O exemplo de resposta a seguir mostra o evento criado que especifica as informações dos três locais de reunião.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-177">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="d5b3c-178">Devido ao cabeçalho da solicitação `Prefer: outlook.timezone="Pacific Standard Time"`, as propriedades **start** e **end** são expressas em PST.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-178">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="d5b3c-179">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5b3c-180">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-180">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_multiple_locations",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2985

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('d1a2fae9-db66-4cc9-8133-2184c77af1b8')/events/$entity",
  "@odata.etag":"W/\"y53lbKh6jkaxHzFwGhgyxgAAw5zhug==\"",
  "id":"AAMkADAGAADDdm4NAAA=",
  "createdDateTime":"2017-08-30T07:06:33.8673345Z",
  "lastModifiedDateTime":"2017-08-30T07:06:34.5079772Z",
  "changeKey":"y53lbKh6jkaxHzFwGhgyxgAAz3IKMA==",
  "categories":[

  ],
  "originalStartTimeZone":"Pacific Standard Time",
  "originalEndTimeZone":"Pacific Standard Time",
  "iCalUId":"04000000820089190544",
  "reminderMinutesBeforeStart":15,
  "isReminderOn":true,
  "hasAttachments":false,
  "hideAttendees": false,
  "subject":"Plan summer company picnic",
  "bodyPreview":"Let's kick-start this event planning!",
  "importance":"normal",
  "sensitivity":"normal",
  "isAllDay":false,
  "isCancelled":false,
  "isOrganizer":true,
  "responseRequested":true,
  "seriesMasterId":null,
  "showAs":"busy",
  "type":"singleInstance",
  "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADAGAADDdm4NAAA%3D&exvsurl=1&path=/calendar/item",
  "onlineMeetingUrl":null,
  "isOnlineMeeting":true,
  "onlineMeetingProvider":"unknown",
  "onlineMeeting":null,
  "allowNewTimeProposals": true,
  "responseStatus":{
    "response":"organizer",
    "time":"0001-01-01T00:00:00Z"
  },
  "body":{
    "contentType":"html",
    "content":"<html>\r\n<head>\r\n</head>\r\n<body>\r\nLet's kick-start this event planning!\r\n</body>\r\n</html>\r\n"
  },
  "start":{
    "dateTime":"2017-08-30T11:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "end":{
    "dateTime":"2017-08-30T12:00:00.0000000",
    "timeZone":"Pacific Standard Time"
  },
  "location":{
    "displayName":"Conf Room 3; Fourth Coffee; Home Office",
    "locationType":"default",
    "uniqueId":"Conf Room 3; Fourth Coffee; Home Office",
    "uniqueIdType":"private"
  },
  "locations":[
    {
      "displayName":"Conf Room 3",
      "locationType":"default",
      "uniqueIdType":"unknown"
    },
    {
      "displayName":"Fourth Coffee",
      "locationType":"default",
      "uniqueId":"Fourth Coffee",
      "uniqueIdType":"private",
      "address":{
        "street":"4567 Main St",
        "city":"Redmond",
        "state":"WA",
        "countryOrRegion":"US",
        "postalCode":"32008"
      },
      "coordinates":{
        "latitude":47.672,
        "longitude":-102.103
      }
    },
    {
      "displayName":"Home Office",
      "locationType":"default",
      "uniqueIdType":"unknown"
    }
  ],
  "recurrence":null,
  "attendees":[
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Dana Swope",
        "address":"DanaS@contoso.onmicrosoft.com"
      }
    },
    {
      "type":"required",
      "status":{
        "response":"none",
        "time":"0001-01-01T00:00:00Z"
      },
      "emailAddress":{
        "name":"Alex Wilber",
        "address":"AlexW@contoso.onmicrosoft.com"
      }
    }
  ],
  "organizer":{
    "emailAddress":{
      "name":"Adele Vance",
      "address":"AdeleV@contoso.onmicrosoft.com"
    }
  }
}
```


### <a name="example-3-create-a-recurring-event"></a><span data-ttu-id="d5b3c-181">Exemplo 3: criar um evento recorrente</span><span class="sxs-lookup"><span data-stu-id="d5b3c-181">Example 3: Create a recurring event</span></span>

#### <a name="request"></a><span data-ttu-id="d5b3c-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-182">Request</span></span>
<span data-ttu-id="d5b3c-183">O terceiro exemplo mostra como criar um evento recorrente uma vez na semana. </span><span class="sxs-lookup"><span data-stu-id="d5b3c-183">The third example shows how to create a recurring event that occurs once a week.</span></span> <span data-ttu-id="d5b3c-184">O evento ocorre das 12:00 às 2:00 da tarde, todas as segundas-feiras a partir de 4 de setembro de 2017 até o final do ano.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-184">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5b3c-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b3c-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon time work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true
}
```
# <a name="c"></a>[<span data-ttu-id="d5b3c-186">C#</span><span class="sxs-lookup"><span data-stu-id="d5b3c-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b3c-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b3c-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b3c-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b3c-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b3c-189">Java</span><span class="sxs-lookup"><span data-stu-id="d5b3c-189">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-recurring-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d5b3c-190">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-190">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="d5b3c-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b3c-191">Response</span></span>
<span data-ttu-id="d5b3c-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==\"",
    "id":"AAMkADQwMD",
    "createdDateTime":"2017-10-07T04:59:12.9698856Z",
    "lastModifiedDateTime":"2017-10-07T04:59:13.8136423Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA5a9Acw==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E0080000000028CEBE04293FD3010000000000000000100000009F85AB8AF8ED4D4FAC777FA89954BDB7",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go for lunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMD&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting":true,
    "onlineMeetingProvider":"unknown",
    "onlineMeeting":null,
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T14:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar",
        "locationType":"default",
        "uniqueId":"Harry's Bar",
        "uniqueIdType":"private"
    },
    "locations":[
        {
            "displayName":"Harry's Bar",
            "locationType":"default",
            "uniqueIdType":"unknown"
        }
    ],
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    },
}
```
### <a name="example-4-create-and-enable-an-event-as-an-online-meeting"></a><span data-ttu-id="d5b3c-195">Exemplo 4: criar e habilitar um evento como uma reunião online</span><span class="sxs-lookup"><span data-stu-id="d5b3c-195">Example 4: Create and enable an event as an online meeting</span></span>

#### <a name="request"></a><span data-ttu-id="d5b3c-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5b3c-196">Request</span></span>
<span data-ttu-id="d5b3c-197">Veja um exemplo de uma solicitação que cria um evento e o habilita como uma reunião online.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-197">Here is an example of a request which creates an event and enables it as an online meeting.</span></span> <span data-ttu-id="d5b3c-198">Ela usa o cabeçalho da solicitação `Prefer: outlook.timezone` para especificar o fuso horário para as horas de **início** e **fim** na resposta.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-198">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="d5b3c-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5b3c-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user_with_online_meeting"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does noon work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ],
  "allowNewTimeProposals": true,
  "isOnlineMeeting": true,
  "onlineMeetingProvider": "teamsForBusiness"
}
```
# <a name="c"></a>[<span data-ttu-id="d5b3c-200">C#</span><span class="sxs-lookup"><span data-stu-id="d5b3c-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-with-online-meeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5b3c-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5b3c-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-with-online-meeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5b3c-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5b3c-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-with-online-meeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5b3c-203">Java</span><span class="sxs-lookup"><span data-stu-id="d5b3c-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-with-online-meeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="d5b3c-204">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="d5b3c-204">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
#### <a name="response"></a><span data-ttu-id="d5b3c-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5b3c-205">Response</span></span>
<span data-ttu-id="d5b3c-206">Veja um exemplo de resposta que exibe as propriedades **start** e **end** usando o fuso horário especificado no cabeçalho `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-206">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span>
<span data-ttu-id="d5b3c-207">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-207">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5b3c-208">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d5b3c-208">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_from_user_with_online_meeting",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt8AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[
    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "hideAttendees": false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does noon work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "teamsForBusiness",
    "allowNewTimeProposals": true,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueIdType": "unknown"
        }
    ],
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    },
    "onlineMeeting": {
        "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_NzIyNzhlMGEtM2YyZC00ZmY0LTlhNzUtZmZjNWFmZGNlNzE2%40thread.v2/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22bc55b173-cff6-457d-b7a1-64bda7d7581a%22%7d",
        "conferenceId": "177513992",
        "tollNumber": "+1 425 555 0123"
    }
}
```

## <a name="see-also"></a><span data-ttu-id="d5b3c-209">Confira também</span><span class="sxs-lookup"><span data-stu-id="d5b3c-209">See also</span></span>

- [<span data-ttu-id="d5b3c-210">Agendar compromissos repetidos como eventos recorrentes no Outlook</span><span class="sxs-lookup"><span data-stu-id="d5b3c-210">Schedule repeating appointments as recurring events in Outlook</span></span>](/graph/outlook-schedule-recurring-events)
- [<span data-ttu-id="d5b3c-211">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="d5b3c-211">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d5b3c-212">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="d5b3c-212">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="d5b3c-213">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="d5b3c-213">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

