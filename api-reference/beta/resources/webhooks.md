---
title: Usar a API do Microsoft Graph para acessar as notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Aplicativos cliente usam notificações para atualizar seu estado após alterações. Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira Configurar notificações para alterações nos dados de usuário.
localization_priority: Normal
author: baywet
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: 2a93e0e25a426fec3d7ab1e10a51953c286da0ab
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216238"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="398d6-106">Usar a API do Microsoft Graph para acessar as notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="398d6-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="398d6-107">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes.</span><span class="sxs-lookup"><span data-stu-id="398d6-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="398d6-108">Um cliente é um serviço Web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="398d6-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="398d6-109">Aplicativos cliente usam notificações para atualizar seu estado após alterações.</span><span class="sxs-lookup"><span data-stu-id="398d6-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="398d6-110">Para saber mais, incluindo como se inscrever e lidar com as notificações recebidas, confira [Configurar notificações para alterações nos dados de usuário](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="398d6-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="398d6-111">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="398d6-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="398d6-112">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="398d6-112">Outlook [message][]</span></span>
- <span data-ttu-id="398d6-113">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="398d6-113">Outlook [event][]</span></span>
- <span data-ttu-id="398d6-114">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="398d6-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="398d6-115">[user][]</span><span class="sxs-lookup"><span data-stu-id="398d6-115">[user][]</span></span>
- <span data-ttu-id="398d6-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="398d6-116">[group][]</span></span>
- <span data-ttu-id="398d6-117">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="398d6-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="398d6-118">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="398d6-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="398d6-119">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="398d6-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="398d6-120">[chatMessage][]</span><span class="sxs-lookup"><span data-stu-id="398d6-120">[chatMessage][]</span></span>
- <span data-ttu-id="398d6-121">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="398d6-121">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="398d6-122">Permissões</span><span class="sxs-lookup"><span data-stu-id="398d6-122">Permissions</span></span>

<span data-ttu-id="398d6-p103">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="398d6-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="398d6-127">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="398d6-127">Permission type</span></span>                        | <span data-ttu-id="398d6-128">Tipos de recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="398d6-128">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="398d6-129">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="398d6-129">Delegated - work or school account</span></span>     | <span data-ttu-id="398d6-130">[alerta][], [contato][], [conversa][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]</span><span class="sxs-lookup"><span data-stu-id="398d6-130">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="398d6-131">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="398d6-131">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="398d6-132">[contato][], [driveItem][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="398d6-132">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="398d6-133">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="398d6-133">Application</span></span>                            | <span data-ttu-id="398d6-134">[alerta][], [contato][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][], [chat][]</span><span class="sxs-lookup"><span data-stu-id="398d6-134">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][], [chatMessage][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="398d6-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="398d6-135">See also</span></span>

- [<span data-ttu-id="398d6-136">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="398d6-136">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="398d6-137">Listar de assinaturas</span><span class="sxs-lookup"><span data-stu-id="398d6-137">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="398d6-138">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="398d6-138">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="398d6-139">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="398d6-139">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="398d6-140">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="398d6-140">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="398d6-141">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="398d6-141">Delete subscription</span></span>](../api/subscription-delete.md)

[chatMessage]: ./chatmessage.md
[contato]: ./contact.md
[contact]: ./contact.md
[conversa]: ./conversation.md
[conversation]: ./conversation.md
[driveItem]: ./driveitem.md
[event]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[alert]: ./alert.md
