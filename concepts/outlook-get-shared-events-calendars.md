---
title: Obter eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.
author: angelgolfer-ms
ms.openlocfilehash: 8ceb6a49b971c5ad01f27b53c0f3cd3cf047865d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346561"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="265c0-104">Obter eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="265c0-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="265c0-105">No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="265c0-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="265c0-106">Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="265c0-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="265c0-107">O Microsoft Graph oferece suporte de forma programática para colocar eventos em calendários que foram compartilhadas por outros usuários, além de receber os calendários compartilhadas propriamente ditos.</span><span class="sxs-lookup"><span data-stu-id="265c0-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="265c0-108">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="265c0-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="265c0-109">Por exemplo, Henrique compartilhou com Diogo seu calendário padrão e deu a ele acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="265c0-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="265c0-110">Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o aplicativo poderá acessar o calendário padrão de Henrique e os eventos nesse calendário, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="265c0-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="265c0-111">Obter um evento no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="265c0-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="265c0-112">Você pode obter um evento específico no calendário padrão compartilhado de Henrique:</span><span class="sxs-lookup"><span data-stu-id="265c0-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="265c0-113">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificada por `{id}` do calendário padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="265c0-113">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="265c0-114">Obter todos os eventos no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="265c0-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="265c0-115">Obtenha todos os eventos no calendário padrão que Henrique compartilhou com Diogo:</span><span class="sxs-lookup"><span data-stu-id="265c0-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="265c0-116">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) no calendário padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="265c0-116">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="265c0-117">Obter o calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="265c0-117">Get the shared calendar</span></span>

<span data-ttu-id="265c0-118">Obtenha o calendário padrão que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="265c0-118">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="265c0-119">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa a pasta padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="265c0-119">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="265c0-120">Os mesmos recursos de GET se aplicarão se Henrique delegar a Diogo mais acesso ao seu calendário padrão ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="265c0-120">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="265c0-121">Se Henrique não tiver compartilhado seu calendário padrão com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="265c0-121">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="265c0-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="265c0-122">Next steps</span></span>

<span data-ttu-id="265c0-123">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="265c0-123">Find out more about:</span></span>

- [<span data-ttu-id="265c0-124">Por que se integrar com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="265c0-124">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="265c0-125">A [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="265c0-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>