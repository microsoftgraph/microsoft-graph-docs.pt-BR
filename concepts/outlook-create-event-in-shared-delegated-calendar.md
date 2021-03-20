---
title: Crie eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: e09b3552ca0d4a3ecd85855c471ec1cc16950abf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941397"
---
# <a name="create-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="f17e9-104">Crie eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="f17e9-104">Create Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="f17e9-105">No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles vejam, criem ou modifiquem eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="f17e9-105">In Outlook, customers can share a calendar with other users and let them view, create, or modify events in that calendar.</span></span> <span data-ttu-id="f17e9-106">Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="f17e9-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="f17e9-107">Programaticamente, o Microsoft Graph oferece suporte à leitura e à criação de eventos em calendários que foram compartilhadas por outros usuários, além de leitura da calendários compartilhados e da atualização do nome do calendário para compartilhados.</span><span class="sxs-lookup"><span data-stu-id="f17e9-107">Programmatically, Microsoft Graph supports reading or writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="f17e9-108">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="f17e9-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="f17e9-109">O restante deste artigo discorre sobre a criação de um evento de reunião em um calendário compartilhado ou delegado.</span><span class="sxs-lookup"><span data-stu-id="f17e9-109">The rest of this article walks through creating a meeting event in a shared or delegated calendar.</span></span> <span data-ttu-id="f17e9-110">Para obter eventos, consulte[Obter eventos do Outlook em um calendário compartilhado ou delegado](outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="f17e9-110">For getting events, refer to [Get Outlook events in a shared or delegated calendar](outlook-get-shared-events-calendars.md).</span></span>

<span data-ttu-id="f17e9-111">A instrução a seguir usa o cenário de exemplo em que Alex delega seu calendário principal à Adele no Outlook e mantém a configuração de caixa de correio do Outlook padrão para direcionar solicitações de reunião e respostas apenas às pessoas delegadas.</span><span class="sxs-lookup"><span data-stu-id="f17e9-111">The walkthrough below uses the example scenario where Alex has delegated his primary calendar to Adele in Outlook, and kept the default Outlook mailbox setting to direct meeting requests and responses to only delegates.</span></span> <span data-ttu-id="f17e9-112">(Esta configuração corresponde à propriedade **delegateMeetingMessageDeliveryOptions** de [mailboxSettings](/graph/api/resources/mailboxsettings) do Alex, definida como o valor padrão `sendToDelegateOnly`).</span><span class="sxs-lookup"><span data-stu-id="f17e9-112">(This setting corresponds to the **delegateMeetingMessageDeliveryOptions** property of Alex' [mailboxSettings](/graph/api/resources/mailboxsettings) set as the default value `sendToDelegateOnly`.)</span></span> 

<span data-ttu-id="f17e9-113">A instrução passo a passo descreve algumas etapas subsequentes:</span><span class="sxs-lookup"><span data-stu-id="f17e9-113">The walkthrough describes a few subsequent steps:</span></span>
1. <span data-ttu-id="f17e9-114">[Adele obtém o calendário que Alex delegou a ela](#step-1-adele-gets-the-delegated-calendar).</span><span class="sxs-lookup"><span data-stu-id="f17e9-114">[Adele gets the calendar that Alex has delegated to her](#step-1-adele-gets-the-delegated-calendar).</span></span>
2. <span data-ttu-id="f17e9-115">[Adele envia um convite de reunião para Clara e Sara em nome de Alex](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf).</span><span class="sxs-lookup"><span data-stu-id="f17e9-115">[Adele sends a meeting invitation to Christie and Megan on Alex' behalf](#step-2-adele-creates-and-sends-an-invitation-on-alex-behalf).</span></span> 
3. <span data-ttu-id="f17e9-116">[Clara recebe a solicitação de reunião e examina o evento associado no seu calendário](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).</span><span class="sxs-lookup"><span data-stu-id="f17e9-116">[Christie receives the meeting request, and inspects the associated event in her calendar](#step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar).</span></span>
4. <span data-ttu-id="f17e9-117">[Clara responde com um “talvez” ao convite](#step-4-christie-responds-to-the-meeting-request).</span><span class="sxs-lookup"><span data-stu-id="f17e9-117">[Christie responds tentative to the invitation](#step-4-christie-responds-to-the-meeting-request).</span></span>
5. <span data-ttu-id="f17e9-118">[Adele recebe a mensagem de resposta da Clara](#step-5-adele-receives-the-response-message).</span><span class="sxs-lookup"><span data-stu-id="f17e9-118">[Adele receives Christie's response message](#step-5-adele-receives-the-response-message).</span></span>
6. <span data-ttu-id="f17e9-119">[Alex verifica as respostas dos participantes como parte do evento](#step-6-alex-accesses-responses-as-part-of-the-event).</span><span class="sxs-lookup"><span data-stu-id="f17e9-119">[Alex checks attendees' responses as part of the event](#step-6-alex-accesses-responses-as-part-of-the-event).</span></span>

<span data-ttu-id="f17e9-120">Caso Alex tenha compartilhado com Adele mas não tiver delegado seu calendário à ela:</span><span class="sxs-lookup"><span data-stu-id="f17e9-120">If Alex has shared and not delegated his calendar with Adele:</span></span>

- <span data-ttu-id="f17e9-121">Conectado como Adele, um aplicativo pode [obter o calendário que Alex compartilhou com Adele](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span><span class="sxs-lookup"><span data-stu-id="f17e9-121">Signed in as Adele, an app can [get the calendar that Alex has shared with Adele](outlook-get-shared-events-calendars.md#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span>
- <span data-ttu-id="f17e9-122">O aplicativo pode usar as solicitações e respostas nas etapas 2 a 4 para aplicar ao calendário compartilhado da mesma maneira que ao calendário delegado.</span><span class="sxs-lookup"><span data-stu-id="f17e9-122">The app can use the requests and responses in steps 2 to 4 to apply to the shared calendar the same way as the delegated calendar.</span></span>
- <span data-ttu-id="f17e9-123">Na etapa 5, o aplicativo pode entrar como Alex, em vez de Adele, para receber a mensagem de resposta do Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-123">In step 5, the app can sign in as Alex, instead of Adele, to receive Christie's response message.</span></span>

## <a name="step-1-adele-gets-the-delegated-calendar"></a><span data-ttu-id="f17e9-124">Etapa 1: Adele obtém o calendário delegado</span><span class="sxs-lookup"><span data-stu-id="f17e9-124">Step 1: Adele gets the delegated calendar</span></span>

<span data-ttu-id="f17e9-125">Entre como Adele, obtenha os calendários a que ela tem acesso e identifique aquele que Alex delegou a ela, para usá-lo na próxima etapa para criar um evento no calendário.</span><span class="sxs-lookup"><span data-stu-id="f17e9-125">Signed in as Adele, get the calendars she has access to and identify the one Alex has delegated to her, so to use it in the next step to create an event in that calendar.</span></span> 

<span data-ttu-id="f17e9-126">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-126">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-127">Use a permissão delegada com menos privilégios, `Calendars.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-127">Use the least privileged delegated permission, `Calendars.Read.Shared`.</span></span> <span data-ttu-id="f17e9-128">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-128">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="f17e9-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17e9-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_Adele_calendars"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendars
```
# <a name="c"></a>[<span data-ttu-id="f17e9-130">C#</span><span class="sxs-lookup"><span data-stu-id="f17e9-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adele-calendars-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f17e9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17e9-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adele-calendars-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f17e9-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f17e9-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adele-calendars-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f17e9-133">Java</span><span class="sxs-lookup"><span data-stu-id="f17e9-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adele-calendars-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f17e9-134">Observe que uma resposta bem-sucedida inclui o código de resposta HTTP 200, o principal calendário do Adele e uma cópia do calendário delegado por Alex na caixa de correio do Adele, com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="f17e9-134">Notice a successful response includes the response code HTTP 200, Adele's own primary calendar, and a copy of the calendar delegated by Alex in Adele's mailbox, with the following properties:</span></span>

- <span data-ttu-id="f17e9-135">**canShare** é falso porque Adele é somente uma representante e não a proprietária do calendário.</span><span class="sxs-lookup"><span data-stu-id="f17e9-135">**canShare** is false since Adele is only a delegate and not the calendar owner.</span></span>
- <span data-ttu-id="f17e9-136">**canEdit** é verdadeiro, uma vez como representante, Adele tem acesso de gravação para eventos não privados no calendário delegado.</span><span class="sxs-lookup"><span data-stu-id="f17e9-136">**canEdit** is true since as delegate, Adele has write access to non-private events in the delegated calendar.</span></span>
- <span data-ttu-id="f17e9-137">**owner** é `Alex Wilber` indicando que é o calendário de Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-137">**owner** is `Alex Wilber` indicating it is Alex' calendar.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_Adele_calendars",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars",
    "value": [
        {
            "id": "AQMkADGkAAAJMjAAAAA==",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAAAACXQ==",
            "canShare": true,
            "canViewPrivateItems": true,
            "canEdit": true,
            "owner": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "AAMkADRpAABf0JlzAAA=",
            "name": "Alex Wilber",
            "color": "auto",
            "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m4eQ==",
            "canShare": false,
            "canViewPrivateItems": false,
            "canEdit": true,
            "owner": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    ]
}
```

> <span data-ttu-id="f17e9-138">**OBSERVAÇÃO** Conectado como Adele, você pode, como alternativa, obter o calendário delegado diretamente da caixa de correio de Alex, especificando a identidade de Alex e o atalho de `calendar`, como em `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-138">**NOTE** Signed in as Adele, you can alternatively get the delegated calendar directly from Alex' mailbox, by specifying Alex' identity and the `calendar` shortcut, as in `GET https://graph.microsoft.com/v1.0/users/AlexW@contoso.OnMicrosoft.com/calendar`.</span></span> <span data-ttu-id="f17e9-139">A ID do calendário retornado corresponde apenas à caixa de correio de Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-139">The returned calendar ID corresponds to only Alex' mailbox.</span></span> 

## <a name="step-2-adele-creates-and-sends-an-invitation-on-alex-behalf"></a><span data-ttu-id="f17e9-140">Etapa 2: Adele cria e envia um convite em nome de Alex</span><span class="sxs-lookup"><span data-stu-id="f17e9-140">Step 2: Adele creates and sends an invitation on Alex' behalf</span></span>

<span data-ttu-id="f17e9-141">Conectado como Adele, use o ID do calendário obtido na etapa 1 para criar um [evento](/graph/api/resources/event) no calendário delegado e envie-o para Christie e Megan, em nome de Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-141">Signed in as Adele, use the calendar ID obtained from step 1 to create an [event](/graph/api/resources/event) in the delegated calendar and send it to Christie and Megan, on Alex' behalf.</span></span>

<span data-ttu-id="f17e9-142">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-142">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-143">Use a permissão delegada com menos privilégios, `Calendars.ReadWrite.Shared`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-143">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="f17e9-144">Para mais informações, veja [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-144">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADRpAABf0JlzAAA="],
  "name": "create_send_invitation"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars/AAMkADRpAABf0JlzAAA=/events

Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{
  "subject": "Christmas dinner",
  "body": {
    "contentType": "HTML",
    "content": "Happy holidays!"
  },
  "start": {
      "dateTime": "2019-12-25T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-12-25T22:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Alex' home"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"meganb@contoso.onmicrosoft.com",
        "name": "Megan Bowen"
      },
      "type": "required"
    },
    {
      "emailAddress": {
        "address":"ChristieC@contoso.onmicrosoft.com",
        "name": "Christie Cline"
      },
      "type": "required"
    }
  ]
}
```

<span data-ttu-id="f17e9-145">Observe que uma resposta bem-sucedida inclui HTTP 201 e as seguintes propriedades da instância [event](/graph/api/resources/event):</span><span class="sxs-lookup"><span data-stu-id="f17e9-145">Notice a successful response includes HTTP 201 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="f17e9-146">**isOrganizer** é definido como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="f17e9-146">**isOrganizer** is set to true.</span></span> <span data-ttu-id="f17e9-147">Em geral, essa propriedade é verdadeira se o proprietário do calendário (Alex) é o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="f17e9-147">In general, this property is true if the calendar owner (Alex) is the organizer of the meeting.</span></span> <span data-ttu-id="f17e9-148">Isso também se aplica se um representante (Adele) organizou o evento em nome do proprietário.</span><span class="sxs-lookup"><span data-stu-id="f17e9-148">This also applies if a delegate (Adele) organized the meeting on behalf of the owner.</span></span>
- <span data-ttu-id="f17e9-149">A coleção **attendees** especifica Sara e Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-149">The **attendees** collection specifies Megan and Christie.</span></span>
- <span data-ttu-id="f17e9-150">A propriedade **organizer** está definido como Alex, uma vez que o convite foi enviado pela representante de Alex (Adele) no calendário principal de Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-150">**organizer** is set to Alex, since the invitation was sent by Alex' delegate (Adele) in Alex' primary calendar.</span></span>
- <span data-ttu-id="f17e9-151">Nem a instância **participantes** nem a **organizer** especifica o representante (Adele).</span><span class="sxs-lookup"><span data-stu-id="f17e9-151">Neither the **attendees** nor **organizer** specifies the delegate (Adele).</span></span>

<!-- {
  "blockType": "response",
  "name": "create_send_invitation",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/calendars('AAMkADRpAABf0JlzAAA%3D')/events/$entity",
    "@odata.etag": "W/\"NDznl+Uh50WkanaCOKHkaQAAX8m47Q==\"",
    "id": "AAMkADI4oeRpAABf0LrcAAA=",
    "createdDateTime": "2019-12-21T04:59:01.9766929Z",
    "lastModifiedDateTime": "2019-12-21T04:59:02.0214967Z",
    "changeKey": "NDznl+Uh50WkanaCOKHkaQAAX8m47Q==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": false,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI4oeRpAABf0LrcAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-25T18:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-12-25T22:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="step-3-christie-receives-meeting-request-and-inspects-the-associated-event-in-her-calendar"></a><span data-ttu-id="f17e9-152">Etapa 3: Clara recebe a solicitação de reunião e examina o evento associado no seu calendário</span><span class="sxs-lookup"><span data-stu-id="f17e9-152">Step 3: Christie receives meeting request and inspects the associated event in her calendar</span></span>

<span data-ttu-id="f17e9-153">Ao entregar a solicitação de reunião, o Outlook cria automaticamente um[evento](/graph/api/resources/event)não confirmado no calendário de Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-153">Upon delivering the meeting request, Outlook automatically creates a tentative [event](/graph/api/resources/event) in Christie's calendar.</span></span>

<span data-ttu-id="f17e9-154">Conectado como Christie, obtenha o [eventMessage](/graph/api/resources/eventmessage) e **evento** que estão associados à solicitação de reunião da etapa 2.</span><span class="sxs-lookup"><span data-stu-id="f17e9-154">Signed in as Christie, get the [eventMessage](/graph/api/resources/eventmessage) and **event** that are associated with the meeting request from step 2.</span></span>

<span data-ttu-id="f17e9-155">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-155">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-156">Use a permissão delegada com menos privilégios, `Mail.Read` e`Calendar.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-156">Use the least privileged delegated permisson, `Mail.Read` and `Calendar.Read.Shared`.</span></span> <span data-ttu-id="f17e9-157">Para mais informações, veja [permissões de correio](permissions-reference.md#mail-permissions) e [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-157">For more information, see [mail permissions](permissions-reference.md#mail-permissions) and [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="f17e9-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17e9-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5hYdAAA="],
  "name": "get_eventmessage_and_event"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADADVj3fyAABZ5hYdAAA=?$expand=microsoft.graph.eventMessage/event
```
# <a name="c"></a>[<span data-ttu-id="f17e9-159">C#</span><span class="sxs-lookup"><span data-stu-id="f17e9-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-eventmessage-and-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f17e9-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17e9-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-eventmessage-and-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f17e9-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f17e9-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-eventmessage-and-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f17e9-162">Java</span><span class="sxs-lookup"><span data-stu-id="f17e9-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-eventmessage-and-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f17e9-163">Observe que uma resposta bem-sucedida inclui HTTP 200 e as seguintes propriedades do[eventMessage](/graph/api/resources/eventmessage):</span><span class="sxs-lookup"><span data-stu-id="f17e9-163">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="f17e9-164">**meetingMessageType** especifica se essa mensagem é `meetingRequest`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-164">**meetingMessageType** specifies this message is `meetingRequest`.</span></span>
- <span data-ttu-id="f17e9-165">**sender** é Adele.</span><span class="sxs-lookup"><span data-stu-id="f17e9-165">**sender** is Adele.</span></span>
- <span data-ttu-id="f17e9-166">**from** é Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-166">**from** is Alex.</span></span>
- <span data-ttu-id="f17e9-167">**toRecipients** incluem Sara e Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-167">**toRecipients** include Megan and Christie.</span></span>

<span data-ttu-id="f17e9-168">E as seguintes propriedades da instância [event](/graph/api/resources/event):</span><span class="sxs-lookup"><span data-stu-id="f17e9-168">And the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="f17e9-169">**attendees** incluem Alex, Sara e Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-169">**attendees** include Alex, Megan, and Christie.</span></span>
- <span data-ttu-id="f17e9-170">**organizer** é Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-170">**organizer** is Alex.</span></span>

<span data-ttu-id="f17e9-171">A identidade de Adele é exibida somente na propriedade **sender**, da **eventMessage** e não no **evento** associado.</span><span class="sxs-lookup"><span data-stu-id="f17e9-171">Adele's identity appears only in the **sender** property of the **eventMessage** and not in the associated **event**.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages(microsoft.graph.eventMessage/event())/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h\"",
    "id": "AAMkADADVj3fyAABZ5hYdAAA=",
    "createdDateTime": "2019-12-21T04:59:03Z",
    "lastModifiedDateTime": "2019-12-21T04:59:04Z",
    "changeKey": "CwAAABYAAADK82uJYVo4RrFV3ADVj3fyAABZ378h",
    "categories": [],
    "receivedDateTime": "2019-12-21T04:59:03Z",
    "sentDateTime": "2019-12-21T04:59:01Z",
    "hasAttachments": false,
    "internetMessageId": "<DM6PR17MB3593711A1C0A098167F5A977A12C0@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "parentFolderId": "AQMkADIAAAIBDAAAAA==",
    "conversationId": "AAQkADNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAw==",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": true,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADADVj3fyAABZ5hYdAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingRequest",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Adele Vance",
            "address": "AdeleV@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    },
    "event@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('662b947c-d9a1-4064-926c-eba1316d4462')/messages('AAMkADADVj3fyAABZ5hYdAAA%3D')/microsoft.graph.eventMessage/microsoft.graph.eventMessage/event/$entity",
    "event": {
        "@odata.etag": "W/\"yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==\"",
        "id": "AAMkADADVj3fyAABZ5ieyAAA=",
        "createdDateTime": "2019-12-21T04:59:03.4336242Z",
        "lastModifiedDateTime": "2019-12-27T01:38:32.3766961Z",
        "changeKey": "yvNriWFaOEaxVdwA1Y938gAAX+T7Jg==",
        "categories": [],
        "originalStartTimeZone": "Pacific Standard Time",
        "originalEndTimeZone": "Pacific Standard Time",
        "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
        "reminderMinutesBeforeStart": 15,
        "isReminderOn": true,
        "hasAttachments": false,
        "subject": "Christmas dinner",
        "bodyPreview": "Happy holidays!",
        "importance": "normal",
        "sensitivity": "normal",
        "isAllDay": false,
        "isCancelled": false,
        "isOrganizer": false,
        "responseRequested": true,
        "seriesMasterId": null,
        "showAs": "tentative",
        "type": "singleInstance",
        "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADADVj3fyAABZ5ieyAAA%3D&exvsurl=1&path=/calendar/item",
        "onlineMeetingUrl": null,
        "recurrence": null,
        "responseStatus": {
            "response": "none",
            "time": "2019-12-21T05:16:48.8931825Z"
        },
        "body": {
            "contentType": "html",
            "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
        },
        "start": {
            "dateTime": "2019-12-26T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "end": {
            "dateTime": "2019-12-26T06:00:00.0000000",
            "timeZone": "UTC"
        },
        "location": {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        },
        "locations": [
            {
                "displayName": "Alex' home",
                "locationType": "default",
                "uniqueId": "1396aaf3-e344-4567-a4e3-797557ec24c8",
                "uniqueIdType": "locationStore"
            }
        ],
        "attendees": [
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Megan Bowen",
                    "address": "MeganB@contoso.OnMicrosoft.com"
                }
            },
            {
                "type": "required",
                "status": {
                    "response": "none",
                    "time": "0001-01-01T00:00:00Z"
                },
                "emailAddress": {
                    "name": "Christie Cline",
                    "address": "ChristieC@contoso.OnMicrosoft.com"
                }
            }
        ],
        "organizer": {
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        }
    }
}
```


## <a name="step-4-christie-responds-to-the-meeting-request"></a><span data-ttu-id="f17e9-172">Etapa 4: a Clara responde à solicitação de reunião</span><span class="sxs-lookup"><span data-stu-id="f17e9-172">Step 4: Christie responds to the meeting request</span></span>

<span data-ttu-id="f17e9-173">Conectada como Clara, define o **evento** como provisório e inclui uma mensagem na resposta:</span><span class="sxs-lookup"><span data-stu-id="f17e9-173">Signed in as Christie, reply to the **event** as tentative, and include a reply message in the response:</span></span>

<span data-ttu-id="f17e9-174">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-174">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-175">Use a permissão delegada com menos privilégios, `Calendars.ReadWrite.Shared`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-175">Use the least privileged delegated permission, `Calendars.ReadWrite.Shared`.</span></span> <span data-ttu-id="f17e9-176">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-176">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>

# <a name="http"></a>[<span data-ttu-id="f17e9-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17e9-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADADVj3fyAABZ5ieyAAA="],
  "name": "event_reply_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/AAMkADADVj3fyAABZ5ieyAAA=/tentativelyAccept
Content-type: application/json

{
  "comment": "I will probably be able to make it.",
  "sendResponse": true
}
```
# <a name="c"></a>[<span data-ttu-id="f17e9-178">C#</span><span class="sxs-lookup"><span data-stu-id="f17e9-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-reply-tentativelyaccept-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f17e9-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17e9-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-reply-tentativelyaccept-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f17e9-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f17e9-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-reply-tentativelyaccept-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f17e9-181">Java</span><span class="sxs-lookup"><span data-stu-id="f17e9-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-reply-tentativelyaccept-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f17e9-182">Uma resposta bem-sucedida retorna HTTP 202 Aceito.</span><span class="sxs-lookup"><span data-stu-id="f17e9-182">A successful response returns HTTP 202 Accepted.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```


## <a name="step-5-adele-receives-the-response-message"></a><span data-ttu-id="f17e9-183">Etapa 5: Adele recebe a mensagem de resposta</span><span class="sxs-lookup"><span data-stu-id="f17e9-183">Step 5: Adele receives the response message</span></span>

<span data-ttu-id="f17e9-184">Como Adele é uma representante do calendário principal de Alex, Adele recebe todas as respostas de reunião desse calendário em nome de Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-184">Because Adele is a delegate of Alex' primary calendar, Adele receives all meeting responses for that calendar on Alex' behalf.</span></span>

<span data-ttu-id="f17e9-185">Conectado como Adele, obtenha o [eventMessage](/graph/api/resources/eventmessage) que representa a resposta de Christie na etapa 4.</span><span class="sxs-lookup"><span data-stu-id="f17e9-185">Signed in as Adele, get the [eventMessage](/graph/api/resources/eventmessage) that represents the response from Christie in step 4.</span></span>

<span data-ttu-id="f17e9-186">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-186">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-187">Use a permissão delegada com menos privilégios, `Mail.Read.Shared`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-187">Use the least privileged delegated permission, `Mail.Read.Shared`.</span></span> <span data-ttu-id="f17e9-188">Para mais informações, veja [permissões de correio](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-188">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="f17e9-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17e9-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI4oeRpAABf0HJUAAA="],
  "name": "message_get_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages/AAMkADI4oeRpAABf0HJUAAA=
```
# <a name="c"></a>[<span data-ttu-id="f17e9-190">C#</span><span class="sxs-lookup"><span data-stu-id="f17e9-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-get-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f17e9-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17e9-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-get-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f17e9-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f17e9-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-get-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f17e9-193">Java</span><span class="sxs-lookup"><span data-stu-id="f17e9-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-get-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f17e9-194">Observe que uma resposta bem-sucedida inclui HTTP 200 e as seguintes propriedades do[eventMessage](/graph/api/resources/eventmessage):</span><span class="sxs-lookup"><span data-stu-id="f17e9-194">Notice a successful response includes the response code HTTP 200 and the following [eventMessage](/graph/api/resources/eventmessage) properties:</span></span>

- <span data-ttu-id="f17e9-195">**meetingMessageType** é `meetingTenativelyAccepted`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-195">**meetingMessageType** is `meetingTenativelyAccepted`.</span></span>
- <span data-ttu-id="f17e9-196">**de** é Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-196">**from** is Christie.</span></span>
- <span data-ttu-id="f17e9-197">**toRecipients** inclui somente Adele, mas não o proprietário do calendário Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-197">**toRecipients** includes only Adele, but not the calendar owner Alex.</span></span> <span data-ttu-id="f17e9-198">Isso ocorre porque Alex manteve o padrão para fazer o Outlook direcionar todas as respostas de reunião somente para delegados.</span><span class="sxs-lookup"><span data-stu-id="f17e9-198">This is because Alex kept the default to have Outlook direct all meeting responses to only delegates.</span></span>

<!-- {
  "blockType": "response",
  "name": "message_get_reply",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('d3b9214b-dd8b-441d-b7dc-c446c9fa0e69')/messages/$entity",
    "@odata.type": "#microsoft.graph.eventMessage",
    "@odata.etag": "W/\"DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT\"",
    "id": "AAMkADI4oeRpAABf0HJUAAA=",
    "createdDateTime": "2019-12-21T05:16:55Z",
    "lastModifiedDateTime": "2019-12-21T05:16:57Z",
    "changeKey": "DAAAABYAAAA0POeX5SHnRaRqdoI4oeRpAABfybkT",
    "categories": [],
    "receivedDateTime": "2019-12-21T05:16:56Z",
    "sentDateTime": "2019-12-21T05:16:49Z",
    "hasAttachments": false,
    "internetMessageId": "<86880ccb8ec64184996e46eaddaed279@DM6PR17MB3593.namprd17.prod.outlook.com>",
    "subject": "Tentative: Christmas dinner",
    "bodyPreview": "I will probably be able to make it.",
    "importance": "normal",
    "parentFolderId": "AQMkAD5GkAAAIBDAAAAA==",
    "conversationId": "AAQkADK25bhNqQlzYAM8jQM=",
    "conversationIndex": "AdW3u1xx5S7TYrbluE2pCXNgAzyNAwAAoBoZ",
    "isDeliveryReceiptRequested": null,
    "isReadReceiptRequested": false,
    "isRead": false,
    "isDraft": false,
    "webLink": "https://outlook.office365.com/owa/?ItemID=AAMkADI4oeRpAABf0HJUAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "focused",
    "meetingMessageType": "meetingTenativelyAccepted",
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nI will probably be able to make it.\r\n</body>\r\n</html>\r\n"
    },
    "sender": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "from": {
        "emailAddress": {
            "name": "Christie Cline",
            "address": "ChristieC@contoso.OnMicrosoft.com"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Adele Vance",
                "address": "AdeleV@contoso.OnMicrosoft.com"
            }
        }
    ],
    "ccRecipients": [],
    "bccRecipients": [],
    "replyTo": [],
    "flag": {
        "flagStatus": "notFlagged"
    }
}
```

## <a name="step-6-alex-accesses-responses-as-part-of-the-event"></a><span data-ttu-id="f17e9-199">Etapa 6: Alex acessa respostas como parte do evento</span><span class="sxs-lookup"><span data-stu-id="f17e9-199">Step 6: Alex accesses responses as part of the event</span></span>

<span data-ttu-id="f17e9-200">Como Alex manteve o padrão de fazer com que o Outlook direcionasse todas as solicitações e respostas de reunião apenas para delegados, Alex não recebe a resposta de Clara da etapa 4.</span><span class="sxs-lookup"><span data-stu-id="f17e9-200">Because Alex kept the default to have Outlook direct all meeting requests and responses to only delegates, Alex does not receive Christie's response from step 4.</span></span> <span data-ttu-id="f17e9-201">No entanto, ele pode obter a resposta por meio de [evento](/graph/api/resources/event) no calendário principal.</span><span class="sxs-lookup"><span data-stu-id="f17e9-201">He can however get the response through the [event](/graph/api/resources/event) in his primary calendar.</span></span>

<span data-ttu-id="f17e9-202">Conectado como Alex, obtenha o [evento](/graph/api/resources/event) que Adele criou na etapa 2 e obtém respostas do **participantes** propriedade.</span><span class="sxs-lookup"><span data-stu-id="f17e9-202">Signed in as Alex, get the [event](/graph/api/resources/event) that Adele created in step 2 and get responses from the **attendees** property.</span></span>

<span data-ttu-id="f17e9-203">**Permissões do Microsoft Graph**</span><span class="sxs-lookup"><span data-stu-id="f17e9-203">**Microsoft Graph permissions**</span></span>

<span data-ttu-id="f17e9-204">Use a permissão delegada com menos privilégios, `Calendars.Read`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-204">Use the least privileged delegated permission, `Calendars.Read`.</span></span> <span data-ttu-id="f17e9-205">Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).</span><span class="sxs-lookup"><span data-stu-id="f17e9-205">For more information, see [calendar permissions](permissions-reference.md#calendars-permissions).</span></span>


# <a name="http"></a>[<span data-ttu-id="f17e9-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="f17e9-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADJXJGu0AABf02qwAAA="],
  "name": "event_get_responses"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/calendar/events/AAMkADJXJGu0AABf02qwAAA=
```
# <a name="c"></a>[<span data-ttu-id="f17e9-207">C#</span><span class="sxs-lookup"><span data-stu-id="f17e9-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-get-responses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f17e9-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f17e9-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-get-responses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f17e9-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f17e9-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/event-get-responses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f17e9-210">Java</span><span class="sxs-lookup"><span data-stu-id="f17e9-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-get-responses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f17e9-211">Observe que uma resposta bem-sucedida inclui HTTP 200 e as seguintes propriedades do[event](/graph/api/resources/event):</span><span class="sxs-lookup"><span data-stu-id="f17e9-211">Notice a successful response includes the response code HTTP 200 and the following [event](/graph/api/resources/event) properties:</span></span>

- <span data-ttu-id="f17e9-212">**isOrganizer** é verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="f17e9-212">**isOrganizer** is true.</span></span>
- <span data-ttu-id="f17e9-213">**attendees** incluem Sara e Clara.</span><span class="sxs-lookup"><span data-stu-id="f17e9-213">**attendees** include only Megan and Christie.</span></span>
- <span data-ttu-id="f17e9-214">A propriedade **status** de cada instância **participante** indica qualquer resposta do participante:</span><span class="sxs-lookup"><span data-stu-id="f17e9-214">The **status** property of each **attendee** instance indicates any response from the attendee:</span></span>
  - <span data-ttu-id="f17e9-215">A resposta de Sara é `none`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-215">Megan's response is `none`.</span></span>
  - <span data-ttu-id="f17e9-216">A resposta de Clara é `tentativelyAccepted`.</span><span class="sxs-lookup"><span data-stu-id="f17e9-216">Christie's response is `tentativelyAccepted`.</span></span>
- <span data-ttu-id="f17e9-217">**organizer** é Alex.</span><span class="sxs-lookup"><span data-stu-id="f17e9-217">**organizer** is Alex.</span></span>
- <span data-ttu-id="f17e9-218">Nenhuma propriedade no **evento** retornado indica a delegada, Adele.</span><span class="sxs-lookup"><span data-stu-id="f17e9-218">No property in the returned **event** indicates the delegate, Adele.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_get_responses",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AQMkADAw7QAAAJfygAAAA%3D%3D')/events/$entity",
    "@odata.etag": "W/\"NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==\"",
    "id": "AAMkADJXJGu0AABf02qwAAA=",
    "createdDateTime": "2019-12-21T04:59:01.4435895Z",
    "lastModifiedDateTime": "2019-12-21T05:16:54.689345Z",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAX8xuhA==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200FEFE0BA532444B5FD89BDE22BA103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Christmas dinner",
    "bodyPreview": "Happy holidays!",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADJXJGu0AABf02qwAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nHappy holidays!\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-12-26T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-12-26T06:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Alex' home",
        "locationType": "default",
        "uniqueId": "Alex' home",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Alex' home",
            "locationType": "default",
            "uniqueId": "Alex' home",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "tentativelyAccepted",
                "time": "2019-12-21T05:16:48.8931825Z"
            },
            "emailAddress": {
                "name": "Christie Cline",
                "address": "ChristieC@contoso.OnMicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Alex Wilber",
            "address": "AlexW@contoso.OnMicrosoft.com"
        }
    }
}
```


## <a name="next-steps"></a><span data-ttu-id="f17e9-219">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f17e9-219">Next steps</span></span>

<span data-ttu-id="f17e9-220">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="f17e9-220">Find out more about:</span></span>

- [<span data-ttu-id="f17e9-221">Obter eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="f17e9-221">Get Outlook events in a shared or delegated calendar</span></span>](outlook-get-shared-events-calendars.md)
- [<span data-ttu-id="f17e9-222">Compartilhar ou delegar um calendário no Outlook (visualização)</span><span class="sxs-lookup"><span data-stu-id="f17e9-222">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="f17e9-223">Por que se integrar com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="f17e9-223">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="f17e9-224">A [API de calendário](/graph/api/resources/calendar) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="f17e9-224">The [calendar API](/graph/api/resources/calendar) in Microsoft Graph v1.0.</span></span>
