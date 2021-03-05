---
title: Obter calendário do Outlook compartilhado ou delegado e seus eventos
description: No Outlook, um proprietário de calendário pode compartilhar um calendário com outros usuários e deixá-los exibir ou modificar eventos nesse calendário. o calendário pode ser um calendário personalizado ou o calendário principal. O proprietário também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário da conta de email.
author: juforan
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 06e11f11b9c25e3392075e027278558d1330d51e
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470071"
---
# <a name="get-shared-or-delegated-outlook-calendar-and-its-events"></a><span data-ttu-id="2b925-104">Obter calendário do Outlook compartilhado ou delegado e seus eventos</span><span class="sxs-lookup"><span data-stu-id="2b925-104">Get shared or delegated Outlook calendar and its events</span></span>

<span data-ttu-id="2b925-105">No Outlook, um proprietário de calendário pode compartilhar um calendário com outros usuários e deixá-los exibir ou modificar eventos nesse calendário. o calendário compartilhado pode ser um calendário personalizado ou o calendário principal do proprietário, criado por ele..</span><span class="sxs-lookup"><span data-stu-id="2b925-105">In Outlook, a calendar owner can share a calendar with other users and let them view or modify events in that calendar; the shared calendar can be the owner's primary calendar or a custom calendar created by the owner.</span></span> <span data-ttu-id="2b925-106">Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="2b925-106">The owner can also grant a delegate to their primary calendar and act on their behalf, to receive or respond to meeting requests, or create or change items in the primary calendar.</span></span>

<span data-ttu-id="2b925-107">Programaticamente, o Microsoft Graph oferece suporte à leitura e à criação de eventos em calendários que foram compartilhadas por outros usuários, além de leitura de calendários compartilhados e atualização do nome do calendário para compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="2b925-107">Programmatically, Microsoft Graph supports reading and writing events in calendars that have been shared by other users, as well as reading the shared calendars, and updating the calendar name for sharees.</span></span> <span data-ttu-id="2b925-108">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="2b925-108">The support also applies to calendars that have been delegated.</span></span> <span data-ttu-id="2b925-109">O restante deste artigo descreve a leitura de eventos em um calendário compartilhado ou delegado.</span><span class="sxs-lookup"><span data-stu-id="2b925-109">The rest of this article describes reading events in a shared or delegated calendar.</span></span> <span data-ttu-id="2b925-110">Para obter eventos, consulte[Obter eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md).</span><span class="sxs-lookup"><span data-stu-id="2b925-110">For creating events, refer to [Create Outlook events in a shared or delegated calendar](outlook-create-event-in-shared-delegated-calendar.md).</span></span>

## <a name="sharee-get-a-shared-calendar-or-its-events-directly-from-calendar-owners-mailbox"></a><span data-ttu-id="2b925-111">Compartilhamento: Obtenha um calendário compartilhado ou seus eventos diretamente da caixa de correio do proprietário do calendário</span><span class="sxs-lookup"><span data-stu-id="2b925-111">Sharee: Get a shared calendar or its events directly from calendar owner's mailbox</span></span>

<span data-ttu-id="2b925-112">Os três exemplos a seguir usam esse cenário: no Outlook, Alex compartilhou seu calendário principal com Sara e recebeu de Sara permissões de leitura.</span><span class="sxs-lookup"><span data-stu-id="2b925-112">The three examples below use this scenario: in Outlook, Alex has shared his primary calendar with Megan and given Megan read permissions.</span></span> <span data-ttu-id="2b925-113">Se Sara entrar no aplicativo e oferecer _permissões delegadas_ (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), em nome de Sara, seu aplicativo poderá acessar o calendário principal e seus eventos diretamente da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2b925-113">If Megan signs into your app and provides _delegated permissions_ (Calendars.Read.Shared or Calendars.ReadWrite.Shared), on behalf of Megan, your app can access Alex' primary calendar and its events directly from Alex' mailbox.</span></span>

<span data-ttu-id="2b925-114">Os três exemplos especificam a identidade do proprietário (Alex ' ID de usuário ou nome de usuário do usuário) e o atalho `calendar`.</span><span class="sxs-lookup"><span data-stu-id="2b925-114">The three examples specify the owner's identity (Alex' user ID or user principal name) and the `calendar` shortcut.</span></span> <span data-ttu-id="2b925-115">Eles acessam o calendário e as IDs de eventos que correspondem somente à caixa de correio do proprietário.</span><span class="sxs-lookup"><span data-stu-id="2b925-115">They access calendar and event IDs that correspond to only the owner's mailbox.</span></span> <span data-ttu-id="2b925-116">Especificar esses IDs de eventos e calendários na caixa de correio do compartilhamento (ID de usuário de Sara ou nome de usuário principal) retornaria um erro.</span><span class="sxs-lookup"><span data-stu-id="2b925-116">Specifying these calendar and event IDs in the sharee's mailbox (Megan's user ID or user principal name) would return an error.</span></span> <span data-ttu-id="2b925-117">Para usar o calendário e as IDs de eventos que correspondem à caixa de correio do compartilhamento, confira [compartilhar: Obtenha calendário personalizado, compartilhado ou seus eventos na caixa de correio do compartilhamento](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span><span class="sxs-lookup"><span data-stu-id="2b925-117">To use calendar and event IDs that correspond to the sharee's mailbox, see [Sharee: Get shared, custom calendar or its events from sharee's mailbox](#sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox).</span></span> 

> <span data-ttu-id="2b925-118">**Observação** permissões de compartilhamento (Calendars.Read.Shared ou Calendars.ReadWrite.Shared) permitem a você ler ou escrever eventos em um calendário compartilhado ou representante.</span><span class="sxs-lookup"><span data-stu-id="2b925-118">**Note**: The sharing permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared) allow you to read or write events in a shared or delegated calendar.</span></span> <span data-ttu-id="2b925-119">Eles não têm suporte [subscrever para alterar notificações](webhooks.md) em itens como pastas.</span><span class="sxs-lookup"><span data-stu-id="2b925-119">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="2b925-120">Para configurar as assinaturas de notificação de alteração em eventos em um usuário compartilhado, representante ou qualquer outro usuário ou calendário de recursos no locatário, use a permissão de aplicativo Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="2b925-120">To set up change notification subscriptions on events in a shared, delegated, or any other user or resource calendar in the tenant, use the application permission, Calendars.Read.</span></span>

### <a name="megan-get-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="2b925-121">Sara: Obtenha o calendário principal compartilhado diretamente da caixa de correio de Alex</span><span class="sxs-lookup"><span data-stu-id="2b925-121">Megan: Get the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="2b925-122">Conectado como Sara, obtenha o calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:</span><span class="sxs-lookup"><span data-stu-id="2b925-122">Signed in as Megan, get the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar
```

<span data-ttu-id="2b925-123">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa calendário compartilhado, principal, na caixa de correio de Alex.</span><span class="sxs-lookup"><span data-stu-id="2b925-123">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Alex' shared, primary calendar, in Alex' mailbox.</span></span>

### <a name="megan-get-an-event-in-the-shared-primary-calendar-directly-from-alex-mailbox"></a><span data-ttu-id="2b925-124">Sara: Obtenha o calendário principal compartilhado diretamente a partir da caixa de correio de Alex</span><span class="sxs-lookup"><span data-stu-id="2b925-124">Megan: Get an event in the shared, primary calendar directly from Alex' mailbox</span></span>

<span data-ttu-id="2b925-125">Conectado como Sara, seu aplicativo pode obter um evento específico no calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:</span><span class="sxs-lookup"><span data-stu-id="2b925-125">Signed in as Megan, your app can get a specific event in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="2b925-126">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificada por `{id}` do calendário principal de Alex, diretamente da caixa de correio de Alex.</span><span class="sxs-lookup"><span data-stu-id="2b925-126">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` in Alex' primary calendar, directly from Alex' mailbox.</span></span>

### <a name="megan-get-all-the-events-in-the-shared-primary-calendar-from-alex-mailbox"></a><span data-ttu-id="2b925-127">Sara: Obtenha todos os eventos no calendário principal compartilhado da caixa de correio de Alex</span><span class="sxs-lookup"><span data-stu-id="2b925-127">Megan: Get all the events in the shared, primary calendar from Alex' mailbox</span></span>

<span data-ttu-id="2b925-128">Conectado como Sara, obtenha todos os eventos no calendário principal que Alex compartilhou com Sara, diretamente da caixa de correio de Alex:</span><span class="sxs-lookup"><span data-stu-id="2b925-128">Signed in as Megan, get all the events in the primary calendar that Alex has shared with Megan, directly from Alex' mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{Alex-userId | Alex-userPrincipalName}/calendar/events
```

<span data-ttu-id="2b925-129">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção das instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) do calendário principal de Alex, diretamente da caixa de correio de Alex.</span><span class="sxs-lookup"><span data-stu-id="2b925-129">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Alex' primary calendar, directly from Alex' mailbox.</span></span>

<span data-ttu-id="2b925-130">Os mesmos recursos GET se aplicam se a Alex tiver delegado o acesso a Sara ao calendário principal de Alex, ou se Alex tiver delegado a Sara a sua caixa de correio inteira.</span><span class="sxs-lookup"><span data-stu-id="2b925-130">The same GET capabilities apply if Alex has delegated Megan access to Alex' primary calendar, or if Alex has delegated Megan his entire mailbox.</span></span>

<span data-ttu-id="2b925-131">Se Alex não tiver compartilhado nem delegado o seu calendário principal com Sara, especificar a ID de usuário ou o nome de usuário da Alex nas operações de obter retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="2b925-131">If Alex has not shared nor delegated his primary calendar with Megan, specifying Alex’s user ID or user principal name in the preceding GET operations will return an error.</span></span> 


## <a name="sharee-get-shared-custom-calendar-or-its-events-from-sharees-mailbox"></a><span data-ttu-id="2b925-132">Compartilhamento: Obtenha calendário personalizado, compartilhado ou seus eventos da caixa de correio do compartilhamento</span><span class="sxs-lookup"><span data-stu-id="2b925-132">Sharee: Get shared, custom calendar or its events from sharee's mailbox</span></span>

<span data-ttu-id="2b925-133">Se Alex compartilhou um _calendário_ personalizado (por exemplo, um calendário chamado "festas de crianças") com Adele e Adele tiver fornecido permissões delegadas (Calendars.Read ou Calendars.ReadWrite), seu aplicativo poderá obter os eventos ou o calendário do calendário da cópia local do Alex ", na caixa de email de Adele, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="2b925-133">If Alex has shared a _custom_ calendar (as an example, a calendar named "Kids parties") with Adele, and Adele has provided delegated permissions (Calendars.Read or Calendars.ReadWrite), your app can get the events or calendar from the local copy of Alex' calendar in Adele's mailbox, as described below.</span></span>

1. <span data-ttu-id="2b925-134">Conectado como Adele, use uma das seguintes solicitações para obter todos os calendários aos quais Adele tem acesso, incluindo o calendário personalizado compartilhado.</span><span class="sxs-lookup"><span data-stu-id="2b925-134">Signed in as Adele, use either of the following requests to get all the calendars that Adele has access to, including the shared custom calendar.</span></span>

    <!-- {
      "blockType": "request",
      "name": "get_all_Adele_calendars"
    }-->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars
    ```

    <span data-ttu-id="2b925-135">Uma resposta bem-sucedida inclui o código de resposta HTTP 200 e o conjunto de calendários que Adele tem acesso, incluindo o calendário ("festas das crianças") com o nome do proprietário como "Alex Rodrigues" como o segundo calendário na resposta.</span><span class="sxs-lookup"><span data-stu-id="2b925-135">A successful response includes the response code HTTP 200, and the collection of calendars that Adele has access to, including the calendar ("Kids parties") that has the owner name as "Alex Wilber" as the second calendar in the response.</span></span> <span data-ttu-id="2b925-136">Para um compartilhamento, Adele, a propriedade **canShare** do calendário compartilhado é sempre falsa.</span><span class="sxs-lookup"><span data-stu-id="2b925-136">For a sharee, Adele, the **canShare** property of the shared calendar is always false.</span></span>

    <!-- {
      "blockType": "response",
      "name": "get_all_Adele_calendars",
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
                "id": "AQMkADU5NAAAJMjAAAAA==",
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
                "id": "AAMkADAABf0JlyAAA=",
                "name": "Kids parties",
                "color": "lightYellow",
                "changeKey": "NDznl+Uh50WkanaCOKHkaQAAYumJRQ==",
                "canShare": false,
                "canViewPrivateItems": false,
                "canEdit": false,
                "owner": {
                    "name": "Alex Wilber",
                    "address": "AlexW@contoso.OnMicrosoft.com"
                }
            }
        ]
    }
    ```

2. <span data-ttu-id="2b925-137">Conectado como Adele, obtenha o calendário compartilhado ou obtenha um ou mais eventos no calendário compartilhado usando a segunda ID de calendário na resposta da etapa 1.</span><span class="sxs-lookup"><span data-stu-id="2b925-137">Signed in as Adele, get the shared calendar, or get one or more events in the shared calendar, using the second calendar ID in the response from step 1.</span></span> <span data-ttu-id="2b925-138">As IDs do calendário compartilhado e seu evento correspondem à cópia local do calendário de Alex na caixa de correio de Adele.</span><span class="sxs-lookup"><span data-stu-id="2b925-138">The IDs of the shared calendar and its event correspond to the local copy of Alex' calendar in Adele's mailbox.</span></span>

    <!-- { "blockType": "ignored" } -->
    ```http
    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events/{id}
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events/{id}

    GET https://graph.microsoft.com/v1.0/me/calendars/AAMkADAABf0JlyAAA=/events
    GET https://graph.microsoft.com/v1.0/users/{Adele-userId | Adele-userPrincipalName}/calendars/AAMkADAABf0JlyAAA=/events
    ```

<span data-ttu-id="2b925-139">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e o evento, os eventos ou o calendário solicitado que Alex compartilhou com Adele.</span><span class="sxs-lookup"><span data-stu-id="2b925-139">On successful completion, you'll get HTTP 200 OK and the requested event, events, or calendar that Alex has shared with Adele.</span></span>


## <a name="next-steps"></a><span data-ttu-id="2b925-140">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2b925-140">Next steps</span></span>

<span data-ttu-id="2b925-141">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="2b925-141">Find out more about:</span></span>

- [<span data-ttu-id="2b925-142">Criar eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="2b925-142">Create Outlook events in a shared or delegated calendar</span></span>](outlook-create-event-in-shared-delegated-calendar.md)
- [<span data-ttu-id="2b925-143">Compartilhar ou delegar um calendário no Outlook (visualização)</span><span class="sxs-lookup"><span data-stu-id="2b925-143">Share or delegate a calendar in Outlook (preview)</span></span>](outlook-share-or-delegate-calendar.md)
- [<span data-ttu-id="2b925-144">Por que se integrar com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="2b925-144">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="2b925-145">A [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="2b925-145">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
