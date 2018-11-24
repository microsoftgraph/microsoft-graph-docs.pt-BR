# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="bdc8e-101">Usar a API do Microsoft Graph para obter notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="bdc8e-101">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="bdc8e-102">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes.</span><span class="sxs-lookup"><span data-stu-id="bdc8e-102">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="bdc8e-103">Um cliente é um serviço web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="bdc8e-103">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="bdc8e-104">Aplicativos cliente usam notificações para atualizar seu estado após as alterações.</span><span class="sxs-lookup"><span data-stu-id="bdc8e-104">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="bdc8e-105">Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para que as alterações nos dados do usuário](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="bdc8e-105">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](../../../concepts/webhooks.md).</span></span>

<span data-ttu-id="bdc8e-106">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="bdc8e-106">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="bdc8e-107">Mensagens</span><span class="sxs-lookup"><span data-stu-id="bdc8e-107">Messages</span></span>
- <span data-ttu-id="bdc8e-108">Eventos</span><span class="sxs-lookup"><span data-stu-id="bdc8e-108">Events</span></span>
- <span data-ttu-id="bdc8e-109">Contatos</span><span class="sxs-lookup"><span data-stu-id="bdc8e-109">Contacts</span></span>
- <span data-ttu-id="bdc8e-110">Usuários</span><span class="sxs-lookup"><span data-stu-id="bdc8e-110">Users</span></span>
- <span data-ttu-id="bdc8e-111">Grupos</span><span class="sxs-lookup"><span data-stu-id="bdc8e-111">Groups</span></span>
- <span data-ttu-id="bdc8e-112">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="bdc8e-112">Group conversations</span></span>
- <span data-ttu-id="bdc8e-113">Conteúdo compartilhado na OneDrive, incluindo as unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="bdc8e-113">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="bdc8e-114">Pastas de OneDrive pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="bdc8e-114">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="bdc8e-115">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="bdc8e-115">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="bdc8e-116">Permissions</span><span class="sxs-lookup"><span data-stu-id="bdc8e-116">Permissions</span></span>

<span data-ttu-id="bdc8e-p102">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription_post_subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="bdc8e-p102">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription_post_subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="bdc8e-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdc8e-121">Permission type</span></span>                        | <span data-ttu-id="bdc8e-122">Tipos de recurso com suporte na v1.0</span><span class="sxs-lookup"><span data-stu-id="bdc8e-122">Supported resource types in v1.0</span></span>                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="bdc8e-123">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="bdc8e-123">Delegated - work or school account</span></span>     | <span data-ttu-id="bdc8e-124">[entre em contato][], [conversa][], [unidade][], [evento][], [mensagem][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="bdc8e-124">[contact][], [conversation][], [drive][], [event][], [message][], [alert][]</span></span> |
| <span data-ttu-id="bdc8e-125">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bdc8e-125">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="bdc8e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bdc8e-126">None</span></span>                                                             |
| <span data-ttu-id="bdc8e-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdc8e-127">Application</span></span>                            | <span data-ttu-id="bdc8e-128">[entre em contato][], [conversa][], [evento][], [mensagem][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="bdc8e-128">[contact][], [conversation][], [event][], [message][], [alert][]</span></span>           |

## <a name="see-also"></a><span data-ttu-id="bdc8e-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="bdc8e-129">See also</span></span>

- [<span data-ttu-id="bdc8e-130">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc8e-130">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="bdc8e-131">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc8e-131">Get subscription</span></span>](../api/subscription_get.md)
- [<span data-ttu-id="bdc8e-132">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc8e-132">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
- [<span data-ttu-id="bdc8e-133">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc8e-133">Update subscription</span></span>](../api/subscription_update.md)
- [<span data-ttu-id="bdc8e-134">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="bdc8e-134">Delete subscription</span></span>](../api/subscription_delete.md)

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
[alerta]: ./alert.md
[alert]: ./alert.md