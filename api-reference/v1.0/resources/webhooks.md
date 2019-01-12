---
title: Usar a API do Microsoft Graph para obter notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes. Um cliente é um serviço web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após as alterações. Para obter mais detalhes, incluindo como se inscrever e manipular notificações de entrada, consulte Set up notificações de alterações nos dados do usuário.
localization_priority: Priority
author: piotrci
ms.openlocfilehash: cb522c50b2cd9fec007dd32d4257dd68fc56ea6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981410"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="1d43d-106">Usar a API do Microsoft Graph para obter notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="1d43d-106">Use the Microsoft Graph API to get change notifications</span></span>

<span data-ttu-id="1d43d-107">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações aos clientes.</span><span class="sxs-lookup"><span data-stu-id="1d43d-107">The Microsoft Graph REST API uses a webhook mechanism to deliver notifications to clients.</span></span> <span data-ttu-id="1d43d-108">Um cliente é um serviço web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="1d43d-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="1d43d-109">Aplicativos cliente usam notificações para atualizar seu estado após as alterações.</span><span class="sxs-lookup"><span data-stu-id="1d43d-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="1d43d-110">Para obter mais detalhes, incluindo como assinar e manipular notificações de entrada, consulte [Configurar notificações para que as alterações nos dados do usuário](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="1d43d-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="1d43d-111">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="1d43d-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="1d43d-112">Mensagens</span><span class="sxs-lookup"><span data-stu-id="1d43d-112">Messages</span></span>
- <span data-ttu-id="1d43d-113">Eventos</span><span class="sxs-lookup"><span data-stu-id="1d43d-113">Events</span></span>
- <span data-ttu-id="1d43d-114">Contatos</span><span class="sxs-lookup"><span data-stu-id="1d43d-114">Contacts</span></span>
- <span data-ttu-id="1d43d-115">Usuários</span><span class="sxs-lookup"><span data-stu-id="1d43d-115">Users</span></span>
- <span data-ttu-id="1d43d-116">Grupos</span><span class="sxs-lookup"><span data-stu-id="1d43d-116">Groups</span></span>
- <span data-ttu-id="1d43d-117">Conversas em grupo</span><span class="sxs-lookup"><span data-stu-id="1d43d-117">Group conversations</span></span>
- <span data-ttu-id="1d43d-118">Conteúdo compartilhado na OneDrive, incluindo as unidades associadas a sites do SharePoint</span><span class="sxs-lookup"><span data-stu-id="1d43d-118">Content shared on OneDrive, including drives associated with SharePoint sites</span></span>
- <span data-ttu-id="1d43d-119">Pastas de OneDrive pessoais dos usuários</span><span class="sxs-lookup"><span data-stu-id="1d43d-119">Users' personal OneDrive folders</span></span>
- <span data-ttu-id="1d43d-120">Alertas de segurança</span><span class="sxs-lookup"><span data-stu-id="1d43d-120">Security alerts</span></span>

## <a name="permissions"></a><span data-ttu-id="1d43d-121">Permissions</span><span class="sxs-lookup"><span data-stu-id="1d43d-121">Permissions</span></span>

<span data-ttu-id="1d43d-p103">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="1d43d-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="1d43d-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d43d-126">Permission type</span></span>                        | <span data-ttu-id="1d43d-127">Tipos de recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="1d43d-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="1d43d-128">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="1d43d-128">Delegated - work or school account</span></span>     | <span data-ttu-id="1d43d-129">[entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="1d43d-129">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |
| <span data-ttu-id="1d43d-130">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1d43d-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="1d43d-131">[entre em contato][], [unidade][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="1d43d-131">[contact][], [drive][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="1d43d-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d43d-132">Application</span></span>                            | <span data-ttu-id="1d43d-133">[entre em contato][], [conversa][], [unidade][], [evento][], [grupo][], [mensagem][], [usuário][], [alerta][]</span><span class="sxs-lookup"><span data-stu-id="1d43d-133">[contact][], [conversation][], [drive][], [event][], [group][], [message][], [user][], [alert][]</span></span> |

## <a name="see-also"></a><span data-ttu-id="1d43d-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="1d43d-134">See also</span></span>

- [<span data-ttu-id="1d43d-135">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="1d43d-135">Subscription resource type</span></span>](./subscription.md)
- [<span data-ttu-id="1d43d-136">Inscrições de lista</span><span class="sxs-lookup"><span data-stu-id="1d43d-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="1d43d-137">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="1d43d-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="1d43d-138">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="1d43d-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="1d43d-139">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="1d43d-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="1d43d-140">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="1d43d-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
