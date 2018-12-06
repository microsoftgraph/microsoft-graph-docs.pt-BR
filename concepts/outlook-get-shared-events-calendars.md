---
title: Obter eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário. Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091617"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="46464-104">Obter eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="46464-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="46464-105">No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que eles exibam ou modifiquem eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="46464-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="46464-106">Os clientes também podem permitir que um representante aja em nome deles, para receber ou responder a solicitações de reunião ou então para criar ou alterar itens no calendário.</span><span class="sxs-lookup"><span data-stu-id="46464-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="46464-107">O Microsoft Graph oferece suporte de forma programática para colocar eventos em calendários que foram compartilhadas por outros usuários, além de receber os calendários compartilhadas propriamente ditos.</span><span class="sxs-lookup"><span data-stu-id="46464-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="46464-108">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="46464-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="46464-109">Por exemplo, Henrique compartilhou com Diogo seu calendário padrão e deu a ele acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="46464-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="46464-110">Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o aplicativo poderá acessar o calendário padrão de Henrique e os eventos nesse calendário, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="46464-110">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="46464-111">Obter um evento no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="46464-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="46464-112">Você pode obter um evento específico no calendário padrão compartilhado de Henrique:</span><span class="sxs-lookup"><span data-stu-id="46464-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="46464-113">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificada por `{id}` do calendário padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="46464-113">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="46464-114">Obter todos os eventos no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="46464-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="46464-115">Obtenha todos os eventos no calendário padrão que Henrique compartilhou com Diogo:</span><span class="sxs-lookup"><span data-stu-id="46464-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="46464-116">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) no calendário padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="46464-116">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="46464-117">Obter o calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="46464-117">Get the shared folder</span></span>

<span data-ttu-id="46464-118">Obtenha o calendário padrão que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="46464-118">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="46464-119">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa a pasta padrão de Henrique.</span><span class="sxs-lookup"><span data-stu-id="46464-119">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="46464-120">Os mesmos recursos de GET se aplicarão se Henrique delegar a Diogo mais acesso ao seu calendário padrão ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="46464-120">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="46464-121">Se Henrique não tiver compartilhado seu calendário padrão com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="46464-121">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="46464-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="46464-122">Next steps</span></span>

<span data-ttu-id="46464-123">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="46464-123">Find out more about:</span></span>

- [<span data-ttu-id="46464-124">Por que se integrar com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="46464-124">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="46464-125">A [API de calendário](/graph/api/resources/calendar?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="46464-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>