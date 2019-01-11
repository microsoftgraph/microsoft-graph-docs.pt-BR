---
title: Usar a API do Microsoft Graph para obter notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após as alterações. Para obter mais detalhes, incluindo como se inscrever e manipular notificações de entrada, consulte Set up notificações de alterações nos dados do usuário.
localization_priority: Normal
ms.openlocfilehash: 9b1907d37115e21b41a9e957de9b7ae0a32fd311
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816468"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="ff1cb-106">Usar a API do Microsoft Graph para obter notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="ff1cb-106">Use the Microsoft Graph API to get change notifications</span></span>

> <span data-ttu-id="ff1cb-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff1cb-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff1cb-109">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-109">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="ff1cb-110">Um cliente é um serviço web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-110">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="ff1cb-111">Aplicativos cliente usam notificações para atualizar seu estado após as alterações.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-111">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="ff1cb-112">Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="ff1cb-112">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="ff1cb-113">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="ff1cb-113">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="ff1cb-114">Mensagens</span><span class="sxs-lookup"><span data-stu-id="ff1cb-114">Messages</span></span>
- <span data-ttu-id="ff1cb-115">Eventos</span><span class="sxs-lookup"><span data-stu-id="ff1cb-115">Events</span></span>
- <span data-ttu-id="ff1cb-116">Contatos</span><span class="sxs-lookup"><span data-stu-id="ff1cb-116">Contacts</span></span>
- <span data-ttu-id="ff1cb-117">Usuários</span><span class="sxs-lookup"><span data-stu-id="ff1cb-117">Users</span></span>
- <span data-ttu-id="ff1cb-118">Grupos</span><span class="sxs-lookup"><span data-stu-id="ff1cb-118">Groups</span></span>
- <span data-ttu-id="ff1cb-119">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="ff1cb-119">Group conversations</span></span>
- <span data-ttu-id="ff1cb-120">Conteúdo compartilhado na OneDrive, incluindo as unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="ff1cb-120">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="ff1cb-121">Pastas de OneDrive pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="ff1cb-121">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="ff1cb-122">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="ff1cb-122">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="ff1cb-123">Permissions</span><span class="sxs-lookup"><span data-stu-id="ff1cb-123">Permissions</span></span>

<span data-ttu-id="ff1cb-p104">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="ff1cb-p104">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="ff1cb-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff1cb-128">Permission type</span></span>                        | <span data-ttu-id="ff1cb-129">Tipos de recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="ff1cb-129">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="ff1cb-130">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="ff1cb-130">Delegated - work or school account</span></span>     | <span data-ttu-id="ff1cb-131">[entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="ff1cb-131">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="ff1cb-132">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="ff1cb-132">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="ff1cb-133">[entre em contato][], [unidade][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="ff1cb-133">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="ff1cb-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff1cb-134">Application</span></span>                            | <span data-ttu-id="ff1cb-135">[entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="ff1cb-135">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="ff1cb-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="ff1cb-136">See also</span></span>

- [<span data-ttu-id="ff1cb-137">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="ff1cb-137">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="ff1cb-138">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="ff1cb-138">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="ff1cb-139">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="ff1cb-139">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="ff1cb-140">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="ff1cb-140">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="ff1cb-141">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="ff1cb-141">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="ff1cb-142">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="ff1cb-142">Delete subscription</span></span>](../api/subscription-delete.md)

[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[unidade]: ./drive.md
[drive]: ./drive.md
[evento]: ./event.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alerta]: ./alert.md
[alert]: ./alert.md
