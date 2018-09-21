# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="32e67-101">Obter eventos do Outlook em um calendário compartilhado ou delegado</span><span class="sxs-lookup"><span data-stu-id="32e67-101">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="32e67-102">No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que visualizem ou modifiquem os eventos nele.</span><span class="sxs-lookup"><span data-stu-id="32e67-102">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="32e67-103">Os clientes também podem nomear um representante para agir em nome deles, para receber ou responder a solicitações de reunião, ou criar e alterar itens do calendário.</span><span class="sxs-lookup"><span data-stu-id="32e67-103">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="32e67-104">Via programação, o Microsoft Graph oferece suporte para obter eventos em calendários compartilhados por outros usuários, bem como para obter o próprio calendário compartilhado.</span><span class="sxs-lookup"><span data-stu-id="32e67-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="32e67-105">O suporte também se aplica a calendários que foram delegados.</span><span class="sxs-lookup"><span data-stu-id="32e67-105">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="32e67-106">Por exemplo, Garth compartilhou com John seu calendário padrão com acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="32e67-106">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="32e67-107">Se o John entrar no seu aplicativo e apresentar permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o seu aplicativo será capaz de acessar o calendário padrão do Garth e os eventos contidos nele, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="32e67-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="32e67-108">Obter um evento no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="32e67-108">Get an event in the shared calendar</span></span>

<span data-ttu-id="32e67-109">Você pode obter um evento específico no calendário padrão compartilhado por Garth:</span><span class="sxs-lookup"><span data-stu-id="32e67-109">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="32e67-110">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e a instância [event](../api-reference/v1.0/resources/event.md) identificada por `{id}` do calendário padrão do Garth.</span><span class="sxs-lookup"><span data-stu-id="32e67-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/event.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="32e67-111">Obter todos os eventos no calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="32e67-111">Get all the events in the shared calendar</span></span>

<span data-ttu-id="32e67-112">Obtenha todos os eventos no calendário padrão que Garth compartilhou com John:</span><span class="sxs-lookup"><span data-stu-id="32e67-112">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="32e67-113">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e um conjunto de instâncias [event](../api-reference/v1.0/resources/event.md) no calendário padrão do Garth.</span><span class="sxs-lookup"><span data-stu-id="32e67-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/event.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="32e67-114">Obter o calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="32e67-114">Get the shared folder</span></span>

<span data-ttu-id="32e67-115">Obtenha o calendário padrão que Garth compartilhou com John.</span><span class="sxs-lookup"><span data-stu-id="32e67-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="32e67-116">Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma instância [calendar](../api-reference/v1.0/resources/calendar.md) que representa a pasta padrão do Garth.</span><span class="sxs-lookup"><span data-stu-id="32e67-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/calendar.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="32e67-117">Os mesmos recursos de GET se aplicam se Garth delegar a John mais acesso ao seu calendário padrão ou se delegar toda a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="32e67-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="32e67-118">Se Garth não tiver compartilhado seu calendário padrão com John, nem delegado sua caixa de correio, especificando a identificação de usuário do John ou o nome UPN, essas operações GET retornarão um erro.</span><span class="sxs-lookup"><span data-stu-id="32e67-118">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="32e67-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="32e67-119">Next steps</span></span>

<span data-ttu-id="32e67-120">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="32e67-120">Find out more about:</span></span>

- [<span data-ttu-id="32e67-121">Por que integrar-se com o calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="32e67-121">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="32e67-122">A [API de calendário](../api-reference/v1.0/resources/calendar.md) no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="32e67-122">The [calendar API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1.0.</span></span>