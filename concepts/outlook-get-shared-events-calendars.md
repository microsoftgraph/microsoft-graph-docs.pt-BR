---
title: Obtenha os eventos do Outlook em um calendário compartilhado ou delegado
description: No Outlook, os clientes podem compartilhar um calendário com outros usuários e permita que eles exibir ou modificar os eventos nesse calendário. Os clientes também podem conceder a um representante para agir em nome deles, para receber ou responder às solicitações de reunião, ou criar ou alterar itens do calendário.
ms.openlocfilehash: e05352e164b127adca1305dded5cbb00840eed52
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091617"
---
# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="184ea-104">Obtenha os eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="184ea-104">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="184ea-105">No Outlook, os clientes podem compartilhar um calendário com outros usuários e permita que eles exibir ou modificar os eventos nesse calendário.</span><span class="sxs-lookup"><span data-stu-id="184ea-105">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="184ea-106">Os clientes também podem conceder a um representante para agir em nome deles, para receber ou responder às solicitações de reunião, ou criar ou alterar itens do calendário.</span><span class="sxs-lookup"><span data-stu-id="184ea-106">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="184ea-107">Programaticamente, oferece suporte ao Microsoft Graph obtendo eventos no calendários que foram compartilhados por outros usuários, bem como obtendo o compartilhado calendários sozinhos.</span><span class="sxs-lookup"><span data-stu-id="184ea-107">Programmatically, Microsoft Graph supports getting events in calendars that have been shared by other users, as well as getting the shared calendars themselves.</span></span> <span data-ttu-id="184ea-108">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="184ea-108">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="184ea-109">Por exemplo, Garth tem compartilhadas com John seu calendário padrão e oferecido acesso de leitura de John.</span><span class="sxs-lookup"><span data-stu-id="184ea-109">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="184ea-110">Se John tiver entrado no seu aplicativo e oferecido permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o seu aplicativo será capaz de acessar o calendário padrão e os eventos do Garth nesse calendário conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="184ea-110">If John has signed into your app and provided delegated permissions (Calendars.Read.Shared or Calendars.ReadWrite.Shared), your app will be able to access Garth's default calendar and events in that calendar as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="184ea-111">Obtenha um evento no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="184ea-111">Get an event in the shared calendar</span></span>

<span data-ttu-id="184ea-112">Você pode obter um evento específico no calendário do Garth padrão compartilhada:</span><span class="sxs-lookup"><span data-stu-id="184ea-112">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="184ea-113">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e a instância de [evento](/graph/api/resources/event?view=graph-rest-1.0) identificado pela `{id}` de calendário do Garth padrão.</span><span class="sxs-lookup"><span data-stu-id="184ea-113">On successful completion, you'll get HTTP 200 OK and the [event](/graph/api/resources/event?view=graph-rest-1.0) instance identified by `{id}` from Garth's default calendar.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="184ea-114">Obtenha todos os eventos no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="184ea-114">Get all the events in the shared calendar</span></span>

<span data-ttu-id="184ea-115">Obtenha todos os eventos no calendário padrão que Garth compartilhada com John:</span><span class="sxs-lookup"><span data-stu-id="184ea-115">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="184ea-116">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e um conjunto de instâncias de [evento](/graph/api/resources/event?view=graph-rest-1.0) no calendário de padrão do Garth.</span><span class="sxs-lookup"><span data-stu-id="184ea-116">On successful completion, you'll get HTTP 200 OK and a collection of [event](/graph/api/resources/event?view=graph-rest-1.0) instances in Garth's default calendar.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="184ea-117">Obtenha o calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="184ea-117">Get the shared calendar</span></span>

<span data-ttu-id="184ea-118">Obtenha o calendário padrão que Garth compartilhada com John.</span><span class="sxs-lookup"><span data-stu-id="184ea-118">Get the default calendar that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="184ea-119">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e uma instância de [calendário](/graph/api/resources/calendar?view=graph-rest-1.0) que representa a pasta de padrão do Garth.</span><span class="sxs-lookup"><span data-stu-id="184ea-119">On successful completion, you'll get HTTP 200 OK and a [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) instance that represents Garth's default folder.</span></span>

<span data-ttu-id="184ea-120">Os mesmos recursos GET aplicam se Garth tinha John mais acesso delegado a calendário de padrão do Garth ou se Garth tinha delegada John sua caixa de correio inteira.</span><span class="sxs-lookup"><span data-stu-id="184ea-120">The same GET capabilities apply if Garth had delegated John further access to Garth's default calendar, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="184ea-121">Se Garth não compartilhou seu calendário padrão com John, nem ele tem delegado sua caixa de correio de John, a especificação user ID do Garth ou o nome principal do usuário nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="184ea-121">If Garth has not shared his default calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="184ea-122">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="184ea-122">Next steps</span></span>

<span data-ttu-id="184ea-123">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="184ea-123">Find out more about:</span></span>

- [<span data-ttu-id="184ea-124">Por que a integração com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="184ea-124">Why integrate with Outlook calendar</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="184ea-125">A [API do calendário](/graph/api/resources/calendar?view=graph-rest-1.0) na versão 1.0 do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="184ea-125">The [calendar API](/graph/api/resources/calendar?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>