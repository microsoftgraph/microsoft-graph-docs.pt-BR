---
title: Criar evento
description: Crie um evento no calendário especificado ou no calendário padrão do usuário.
localization_priority: Priority
doc_type: apiPageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5812e0f11d23a54109e99bdc39fab9ac15d86594
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346370"
---
# <a name="create-event"></a><span data-ttu-id="a01bf-103">Criar evento</span><span class="sxs-lookup"><span data-stu-id="a01bf-103">Create Event</span></span>

<span data-ttu-id="a01bf-104">Criar um [evento](../resources/event.md) no calendário padrão do usuário ou em um calendário específico.</span><span class="sxs-lookup"><span data-stu-id="a01bf-104">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="a01bf-105">Você pode especificar o fuso horário de cada um dos horários de início e de término do evento como parte de seus valores, porque as propriedades**inicial** e **final** são do tipo [ dateTimeTimeZone](../resources/datetimetimezone.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-105">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> <span data-ttu-id="a01bf-106">Primeiro [localize os fusos horários com suporte](outlookuser-supportedtimezones.md) para garantir que você tenha definido somente fusos horários que tenham sido configurados para o servidor de caixas de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a01bf-106">First [find the supported time zones](outlookuser-supportedtimezones.md) to make sure you set only time zones that have been configured for the user's mailbox server.</span></span> 

<span data-ttu-id="a01bf-107">Quando um evento é enviado, o servidor envia convites para os participantes.</span><span class="sxs-lookup"><span data-stu-id="a01bf-107">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="a01bf-108">**Definir o local em um evento**</span><span class="sxs-lookup"><span data-stu-id="a01bf-108">**Setting the location in an event**</span></span>

<span data-ttu-id="a01bf-109">Um administrador do Exchange pode configurar um endereço de email e uma caixa de correio para um recurso como uma sala de reunião ou equipamento como um projetor.</span><span class="sxs-lookup"><span data-stu-id="a01bf-109">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="a01bf-110">Os usuários podem convidar o recurso como um participante para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="a01bf-110">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="a01bf-111">Em nome do recurso, o servidor aceita ou recusa a solicitação de reunião com base na disponibilidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="a01bf-111">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="a01bf-112">Se o servidor aceitar uma reunião do recurso, ele criará um evento para a reunião no calendário do recurso.</span><span class="sxs-lookup"><span data-stu-id="a01bf-112">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="a01bf-113">Se a reunião for reagendada, o servidor atualizará o evento no calendário do recurso.</span><span class="sxs-lookup"><span data-stu-id="a01bf-113">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="a01bf-114">Outra vantagem de configurar uma caixa de correio para um recurso é controlar o agendamento do recurso. Por exemplo, somente executivos ou seus representantes podem agendar uma sala de reunião particular.</span><span class="sxs-lookup"><span data-stu-id="a01bf-114">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="a01bf-115">Se você está organizando um evento que envolve um local de reunião:</span><span class="sxs-lookup"><span data-stu-id="a01bf-115">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="a01bf-116">Defina a propriedade **location** de **event** adequadamente.</span><span class="sxs-lookup"><span data-stu-id="a01bf-116">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="a01bf-117">Defina a propriedade opcional **locationEmailAddress** se o local da reunião tiver um endereço de email.</span><span class="sxs-lookup"><span data-stu-id="a01bf-117">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="a01bf-118">Além disso, se o local da reunião tiver sido configurado como um recurso ou se o evento envolver algum equipamento que tenha sido definido como um recurso:</span><span class="sxs-lookup"><span data-stu-id="a01bf-118">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="a01bf-119">Convide o recurso como um [participante](../resources/attendee.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-119">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="a01bf-120">Defina a propriedade **type** do participante como `resource`.</span><span class="sxs-lookup"><span data-stu-id="a01bf-120">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="a01bf-121">Defina o **emailAddress** do participante como o endereço de email do recurso.</span><span class="sxs-lookup"><span data-stu-id="a01bf-121">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="a01bf-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="a01bf-122">Permissions</span></span>
<span data-ttu-id="a01bf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a01bf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a01bf-125">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a01bf-125">Permission type</span></span>      | <span data-ttu-id="a01bf-126">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a01bf-126">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a01bf-127">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a01bf-127">Delegated (work or school account)</span></span> | <span data-ttu-id="a01bf-128">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01bf-128">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a01bf-129">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a01bf-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a01bf-130">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01bf-130">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a01bf-131">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a01bf-131">Application</span></span> | <span data-ttu-id="a01bf-132">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a01bf-132">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a01bf-133">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a01bf-133">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="a01bf-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a01bf-134">Request headers</span></span>
| <span data-ttu-id="a01bf-135">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a01bf-135">Header</span></span>       | <span data-ttu-id="a01bf-136">Valor</span><span class="sxs-lookup"><span data-stu-id="a01bf-136">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="a01bf-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="a01bf-137">Authorization</span></span>  | <span data-ttu-id="a01bf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a01bf-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a01bf-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a01bf-140">Content-Type</span></span>  | <span data-ttu-id="a01bf-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a01bf-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a01bf-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a01bf-143">Request body</span></span>
<span data-ttu-id="a01bf-144">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-144">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="a01bf-145">Como o recurso **event** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o evento ao criá-lo.</span><span class="sxs-lookup"><span data-stu-id="a01bf-145">Since the **event** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="a01bf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a01bf-146">Response</span></span>

<span data-ttu-id="a01bf-147">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [event](../resources/event.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a01bf-147">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a01bf-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a01bf-148">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a01bf-149">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a01bf-149">Request 1</span></span>
<span data-ttu-id="a01bf-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a01bf-150">Here is an example of the request.</span></span> <span data-ttu-id="a01bf-151">Ela usa o cabeçalho da solicitação `Prefer: outlook.timezone` para especificar o fuso horário para as horas de **início** e **fim** na resposta.</span><span class="sxs-lookup"><span data-stu-id="a01bf-151">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a01bf-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a01bf-152">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
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
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a01bf-153">C#</span><span class="sxs-lookup"><span data-stu-id="a01bf-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a01bf-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a01bf-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a01bf-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a01bf-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a01bf-156">Java</span><span class="sxs-lookup"><span data-stu-id="a01bf-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a01bf-157">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-157">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="a01bf-158">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a01bf-158">Response 1</span></span>
<span data-ttu-id="a01bf-159">Veja um exemplo de resposta que exibe as propriedades **start** e **end** usando o fuso horário especificado no cabeçalho `Prefer: outlook.timezone`.</span><span class="sxs-lookup"><span data-stu-id="a01bf-159">Here is an example of the response, which shows the **start** and **end** properties use the time zone specified in the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="a01bf-160">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a01bf-160">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a01bf-161">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a01bf-161">All of the properties will be returned from an actual call.</span></span>
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
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
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


##### <a name="request-2"></a><span data-ttu-id="a01bf-162">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a01bf-162">Request 2</span></span>
<span data-ttu-id="a01bf-163">A solicitação de exemplo a seguir especifica três locais de onde o organizador e os participantes podem participar da reunião.</span><span class="sxs-lookup"><span data-stu-id="a01bf-163">The next example request specifies 3 locations where the organizer and attendees can attend the meeting from.</span></span>

<span data-ttu-id="a01bf-164">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-164">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a01bf-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="a01bf-165">--Http</span></span>](#tab/http)
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
  ]

}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a01bf-166">C#</span><span class="sxs-lookup"><span data-stu-id="a01bf-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-user-multiple-locations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a01bf-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a01bf-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-user-multiple-locations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a01bf-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a01bf-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-user-multiple-locations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a01bf-169">Java</span><span class="sxs-lookup"><span data-stu-id="a01bf-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-user-multiple-locations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="a01bf-170">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a01bf-170">Response 2</span></span>
<span data-ttu-id="a01bf-171">O exemplo de resposta a seguir mostra o evento criado que especifica as informações dos três locais de reunião.</span><span class="sxs-lookup"><span data-stu-id="a01bf-171">The following example response shows the created event that specifies information for the 3 locations for the meeting.</span></span> <span data-ttu-id="a01bf-172">Devido ao cabeçalho da solicitação `Prefer: outlook.timezone="Pacific Standard Time"`, as propriedades **start** e **end** são expressas em PST.</span><span class="sxs-lookup"><span data-stu-id="a01bf-172">Because of the `Prefer: outlook.timezone="Pacific Standard Time"` request header, the **start** and **end** properties are expressed in PST.</span></span>
<span data-ttu-id="a01bf-173">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a01bf-173">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a01bf-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a01bf-174">All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="a01bf-175">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="a01bf-175">Request 3</span></span>
<span data-ttu-id="a01bf-176">O terceiro exemplo mostra como criar um evento recorrente.</span><span class="sxs-lookup"><span data-stu-id="a01bf-176">The third example shows how to create a recurring event.</span></span> <span data-ttu-id="a01bf-177">O evento ocorre das 12:00 às 2:00 da tarde, todas as segundas-feiras a partir de 4 de setembro de 2017 até o final do ano.</span><span class="sxs-lookup"><span data-stu-id="a01bf-177">The event occurs from 12:00pm to 2:00pm, every Monday starting September 4, 2017, through the end of the year.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a01bf-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="a01bf-178">--Http</span></span>](#tab/http)
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
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a01bf-179">C#</span><span class="sxs-lookup"><span data-stu-id="a01bf-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-recurring-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a01bf-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a01bf-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-recurring-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a01bf-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a01bf-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-recurring-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a01bf-182">Java</span><span class="sxs-lookup"><span data-stu-id="a01bf-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-recurring-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a01bf-183">No corpo da solicitação, forneça uma representação JSON do objeto [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a01bf-183">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-3"></a><span data-ttu-id="a01bf-184">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="a01bf-184">Response 3</span></span>
<span data-ttu-id="a01bf-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a01bf-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "OnlineMeeting":null
}
```


## <a name="see-also"></a><span data-ttu-id="a01bf-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="a01bf-188">See also</span></span>

- [<span data-ttu-id="a01bf-189">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a01bf-189">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a01bf-190">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="a01bf-190">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a01bf-191">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="a01bf-191">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)



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
