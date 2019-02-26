---
title: Usar a API do Microsoft Graph para obter notificações de alteração
description: A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes. Um cliente é um serviço Web que configura sua própria URL para receber notificações. Os aplicativos cliente usam notificações para atualizar seu estado nas alterações. Para obter mais detalhes, incluindo como inscrever-se e lidar com notificações de entrada, confira set up Notifications for Changes in User Data.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 1d7a3d868ffc640f7659623942ac102575fb94fc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151489"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a><span data-ttu-id="0fafe-106">Usar a API do Microsoft Graph para obter notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="0fafe-106">Use the Microsoft Graph API to get change notifications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fafe-107">A API REST do Microsoft Graph usa um mecanismo de webhook para fornecer notificações de alteração aos clientes.</span><span class="sxs-lookup"><span data-stu-id="0fafe-107">The Microsoft Graph REST API uses a webhook mechanism to deliver change notifications to clients.</span></span> <span data-ttu-id="0fafe-108">Um cliente é um serviço Web que configura sua própria URL para receber notificações.</span><span class="sxs-lookup"><span data-stu-id="0fafe-108">A client is a web service that configures its own URL to receive notifications.</span></span> <span data-ttu-id="0fafe-109">Os aplicativos cliente usam notificações para atualizar seu estado nas alterações.</span><span class="sxs-lookup"><span data-stu-id="0fafe-109">Client apps use notifications to update their state upon changes.</span></span> <span data-ttu-id="0fafe-110">Para obter mais detalhes, incluindo como inscrever-se e lidar com notificações de entrada, confira [set up Notifications for Changes in User Data](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="0fafe-110">For more details, including how to subscribe to and handle incoming notifications, see [Set up notifications for changes in user data](/graph/webhooks).</span></span>

<span data-ttu-id="0fafe-111">Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:</span><span class="sxs-lookup"><span data-stu-id="0fafe-111">Using the Microsoft Graph API, an app can subscribe to changes on the following resources:</span></span>

- <span data-ttu-id="0fafe-112">[Mensagem][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="0fafe-112">Outlook [message][]</span></span>
- <span data-ttu-id="0fafe-113">[Evento][] do Outlook</span><span class="sxs-lookup"><span data-stu-id="0fafe-113">Outlook [event][]</span></span>
- <span data-ttu-id="0fafe-114">[Contato][] pessoal do Outlook</span><span class="sxs-lookup"><span data-stu-id="0fafe-114">Outlook personal [contact][]</span></span>
- <span data-ttu-id="0fafe-115">[usuário][]</span><span class="sxs-lookup"><span data-stu-id="0fafe-115">[user][]</span></span>
- <span data-ttu-id="0fafe-116">[group][]</span><span class="sxs-lookup"><span data-stu-id="0fafe-116">[group][]</span></span>
- <span data-ttu-id="0fafe-117">[Conversa][] em grupo do Office 365</span><span class="sxs-lookup"><span data-stu-id="0fafe-117">Office 365 group [conversation][]</span></span>
- <span data-ttu-id="0fafe-118">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário</span><span class="sxs-lookup"><span data-stu-id="0fafe-118">Content within the hierarchy of _any folder_ [driveItem][] on a user's personal OneDrive</span></span>
- <span data-ttu-id="0fafe-119">Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="0fafe-119">Content within the hierarchy of the _root folder_ [driveItem][] on OneDrive for Business</span></span>
- <span data-ttu-id="0fafe-120">[Alerta][] de segurança</span><span class="sxs-lookup"><span data-stu-id="0fafe-120">Security [alert][]</span></span>

## <a name="permissions"></a><span data-ttu-id="0fafe-121">Permissões</span><span class="sxs-lookup"><span data-stu-id="0fafe-121">Permissions</span></span>

<span data-ttu-id="0fafe-p103">Em geral, as operações de assinatura exigem permissão de leitura ao recurso. Por exemplo, para obter notificações de mensagens, seu aplicativo precisa da permissão `Mail.Read`. O artigo [criar assinatura](../api/subscription-post-subscriptions.md) lista as permissões necessárias para cada tipo de recurso. A tabela a seguir lista os tipos de permissões que o aplicativo pode solicitar para usar webhooks para tipos específicos de recursos.</span><span class="sxs-lookup"><span data-stu-id="0fafe-p103">In general, subscription operations require read permission to the resource. For example, to get notifications for messages, your app needs the `Mail.Read` permission. The [create subscription](../api/subscription-post-subscriptions.md) article lists permissions needed for each resource type. The following table lists the types of permissions your app can request to use webhooks for specific resource types.</span></span>

| <span data-ttu-id="0fafe-126">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0fafe-126">Permission type</span></span>                        | <span data-ttu-id="0fafe-127">Tipos de recurso suportados</span><span class="sxs-lookup"><span data-stu-id="0fafe-127">Supported resource types</span></span>                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="0fafe-128">Delegado - conta corporativa ou de estudante</span><span class="sxs-lookup"><span data-stu-id="0fafe-128">Delegated - work or school account</span></span>     | <span data-ttu-id="0fafe-129">[alerta][], [contato][], [conversa][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]</span><span class="sxs-lookup"><span data-stu-id="0fafe-129">[alert][], [contact][], [conversation][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|
| <span data-ttu-id="0fafe-130">Delegado - conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0fafe-130">Delegated - personal Microsoft account</span></span> | <span data-ttu-id="0fafe-131">[contato][], [driveItem][], [evento][], [mensagem][]</span><span class="sxs-lookup"><span data-stu-id="0fafe-131">[contact][], [driveItem][], [event][], [message][]</span></span>                                        |
| <span data-ttu-id="0fafe-132">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0fafe-132">Application</span></span>                            | <span data-ttu-id="0fafe-133">[alerta][], [contato][], [driveItem][], [evento][], [grupo][], [mensagem][], [usuário][]</span><span class="sxs-lookup"><span data-stu-id="0fafe-133">[alert][], [contact][], [driveItem][], [event][], [group][], [message][], [user][]</span></span>|

## <a name="see-also"></a><span data-ttu-id="0fafe-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="0fafe-134">See also</span></span>

- [<span data-ttu-id="0fafe-135">Tipo de recurso de assinatura</span><span class="sxs-lookup"><span data-stu-id="0fafe-135">Subscription resource type</span></span>](subscription.md)
- [<span data-ttu-id="0fafe-136">Listar assinaturas</span><span class="sxs-lookup"><span data-stu-id="0fafe-136">List subscriptions</span></span>](../api/subscription-list.md)
- [<span data-ttu-id="0fafe-137">Obter assinatura</span><span class="sxs-lookup"><span data-stu-id="0fafe-137">Get subscription</span></span>](../api/subscription-get.md)
- [<span data-ttu-id="0fafe-138">Criar assinatura</span><span class="sxs-lookup"><span data-stu-id="0fafe-138">Create subscription</span></span>](../api/subscription-post-subscriptions.md)
- [<span data-ttu-id="0fafe-139">Atualizar assinatura</span><span class="sxs-lookup"><span data-stu-id="0fafe-139">Update subscription</span></span>](../api/subscription-update.md)
- [<span data-ttu-id="0fafe-140">Excluir assinatura</span><span class="sxs-lookup"><span data-stu-id="0fafe-140">Delete subscription</span></span>](../api/subscription-delete.md)

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/webhooks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
