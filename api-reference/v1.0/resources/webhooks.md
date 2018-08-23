# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="49954-101">Usar a API do Microsoft Graph para obter notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="49954-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="49954-102">A API REST do Microsoft Graph usa um mecanismo de webhook para enviar notificações aos clientes.</span><span class="sxs-lookup"><span data-stu-id="49954-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="49954-103">Um cliente é um serviço Web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="49954-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="49954-104">Aplicativos cliente usam notificações para atualizar seu estado após as alterações.</span><span class="sxs-lookup"><span data-stu-id="49954-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="49954-105">Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para alterações nos dados do usuário](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="49954-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="49954-106">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para ser notificado de alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="49954-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="49954-107">Mensagens</span><span class="sxs-lookup"><span data-stu-id="49954-107">Messages</span></span>
- <span data-ttu-id="49954-108">Eventos</span><span class="sxs-lookup"><span data-stu-id="49954-108">Events</span></span>
- <span data-ttu-id="49954-109">Contatos</span><span class="sxs-lookup"><span data-stu-id="49954-109">Contacts</span></span>
- <span data-ttu-id="49954-110">Usuários</span><span class="sxs-lookup"><span data-stu-id="49954-110">Users</span></span>
- <span data-ttu-id="49954-111">Grupos</span><span class="sxs-lookup"><span data-stu-id="49954-111">Groups</span></span>
- <span data-ttu-id="49954-112">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="49954-112">Group conversations</span></span>
- <span data-ttu-id="49954-113">Conteúdo compartilhado no OneDrive, incluindo unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="49954-113">Content shared on OneDrive including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="49954-114">Pastas pessoais de usuários no OneDrive</span><span class="sxs-lookup"><span data-stu-id="49954-114">User's personal OneDrive folders</span></span>

## <a name="permissions"></a><span data-ttu-id="49954-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="49954-115">Permissions</span></span>

<span data-ttu-id="49954-p102">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="49954-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="49954-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="49954-120">Permission type</span></span>                        | <span data-ttu-id="49954-121">Tipos de recurso com suporte na v1.0</span><span class="sxs-lookup"><span data-stu-id="49954-121">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="49954-122">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="49954-122">Delegated - work or school account</span></span>     | <span data-ttu-id="49954-123">[contato][], [conversa][], [unidade][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="49954-123">[contact][], [conversation][], [drive][], [event][], [message][]</span></span> |
| <span data-ttu-id="49954-124">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="49954-124">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="49954-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49954-125">None</span></span>                                                             |
| <span data-ttu-id="49954-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="49954-126">Application</span></span>                            | <span data-ttu-id="49954-127">[contato][], [conversa][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="49954-127">[contact][], [conversation][], [event][], [message][]</span></span>            |

## <a name="see-also"></a><span data-ttu-id="49954-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="49954-128">See also</span></span>

- [<span data-ttu-id="49954-129">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="49954-129">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="49954-130">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="49954-130">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="49954-131">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="49954-131">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="49954-132">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="49954-132">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="49954-133">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="49954-133">Delete subscription</span></span>](../api/subscription_delete.md)

[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[unidade]: ./drive.md
[drive]: ./drive.md
[evento]: ./event.md
[event]: ./event.md
[mensagem]: ./message.md
[message]: ./message.md
