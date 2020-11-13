---
title: Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph
description: As notificações de alterações te habilitam a ouvir as alterações nas mensagens no canal ou no chat
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1d9767a913b5fe5878cb1cc8e72ec9900fcec4ac
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000711"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="b526b-103">Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b526b-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="b526b-104">As notificações de alteração habilitam você a assinar para receber alterações (criar, atualizar e excluir) de [ mensagens ](/graph/api/resources/chatMessage?preserve-view=true) em um [ canal ](/graph/api/resources/channel?preserve-view=true) ou [chat](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b526b-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="b526b-105">As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b526b-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="b526b-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b526b-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="b526b-107">**Observação:** o tempo máximo que uma assinatura pode durar é 60 minutos; entretanto, as assinaturas podem ser renovadas até que o chamador tenha permissão para acessar o recurso.</span><span class="sxs-lookup"><span data-stu-id="b526b-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="b526b-108">Assinar para receber alterações no nível do locatário</span><span class="sxs-lookup"><span data-stu-id="b526b-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="b526b-109">Para acompanhar todas as alterações relacionadas a mensagens em um locatário, você pode usar assinaturas em um nível de locatário para mensagens de canal e chat.</span><span class="sxs-lookup"><span data-stu-id="b526b-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="b526b-110">Isso requer que você crie duas assinaturas: uma para acompanhar todas as mensagens nos [canais](/graph/api/resources/channel?preserve-view=true) e outra para acompanhar todas as mensagens nos [chats](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b526b-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="b526b-111">Assine para receber mensagens em todos os canais</span><span class="sxs-lookup"><span data-stu-id="b526b-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="b526b-112">Para obter notificações de alteração para todas as mensagens e respostas nos canais de um locatário, assine em `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="b526b-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="b526b-113">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="b526b-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="b526b-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="b526b-114">Permissions</span></span>

|<span data-ttu-id="b526b-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b526b-115">Permission type</span></span>      | <span data-ttu-id="b526b-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b526b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b526b-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b526b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b526b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-118">Not supported.</span></span> |
|<span data-ttu-id="b526b-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b526b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b526b-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-120">Not supported.</span></span>    |
|<span data-ttu-id="b526b-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b526b-121">Application</span></span> | <span data-ttu-id="b526b-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b526b-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="b526b-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b526b-123">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="b526b-124">Assinar para receber mensagens em chats</span><span class="sxs-lookup"><span data-stu-id="b526b-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="b526b-125">Para obter notificações de alteração para todas as mensagens em chats em um locatário, assine em `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="b526b-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="b526b-126">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="b526b-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="b526b-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="b526b-127">Permissions</span></span>

|<span data-ttu-id="b526b-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b526b-128">Permission type</span></span>      | <span data-ttu-id="b526b-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b526b-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b526b-130">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b526b-130">Delegated (work or school account)</span></span> | <span data-ttu-id="b526b-131">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-131">Not supported.</span></span> |
|<span data-ttu-id="b526b-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b526b-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b526b-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-133">Not supported.</span></span>    |
|<span data-ttu-id="b526b-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b526b-134">Application</span></span> | <span data-ttu-id="b526b-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b526b-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="b526b-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b526b-136">Example</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="b526b-137">Assine em mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="b526b-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="b526b-138">Para acompanhar mensagens e respostas em um canal, você pode criar uma assinatura de notificação de alteraração no nível do canal.</span><span class="sxs-lookup"><span data-stu-id="b526b-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="b526b-139">Para fazer isso, assine em `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="b526b-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="b526b-140">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="b526b-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="b526b-141">As assinaturas no nível do canal também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="b526b-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="b526b-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="b526b-142">Permissions</span></span>

|<span data-ttu-id="b526b-143">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b526b-143">Permission type</span></span>      | <span data-ttu-id="b526b-144">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b526b-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b526b-145">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b526b-145">Delegated (work or school account)</span></span> | <span data-ttu-id="b526b-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b526b-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="b526b-147">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b526b-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b526b-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-148">Not supported.</span></span>    |
|<span data-ttu-id="b526b-149">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b526b-149">Application</span></span> | <span data-ttu-id="b526b-150">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="b526b-150">ChannelMessage.Read.All</span></span> |

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="b526b-151">Exemplo 1: assinar em todas as mensagens (e respostas) em um canal</span><span class="sxs-lookup"><span data-stu-id="b526b-151">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="b526b-152">Exemplo 2: assinar para receber mensagens (e respostas) em um canal que contém determinado texto</span><span class="sxs-lookup"><span data-stu-id="b526b-152">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="b526b-153">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="b526b-153">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="b526b-154">Exemplo 3: assinar para receber mensagens (e respostas) em um canal sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="b526b-154">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="b526b-155">Assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="b526b-155">Subscribe to messages in a chat</span></span>

<span data-ttu-id="b526b-156">Para acompanhar mensagens em um chat, você pode criar uma assinatura de notificação de alteração em um nível de chat.</span><span class="sxs-lookup"><span data-stu-id="b526b-156">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="b526b-157">Para fazer isso, assine em `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="b526b-157">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="b526b-158">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="b526b-158">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="b526b-159">As assinaturas no nível do chat também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="b526b-159">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="b526b-160">Permissões</span><span class="sxs-lookup"><span data-stu-id="b526b-160">Permissions</span></span>

|<span data-ttu-id="b526b-161">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b526b-161">Permission type</span></span>      | <span data-ttu-id="b526b-162">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b526b-162">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b526b-163">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b526b-163">Delegated (work or school account)</span></span> | <span data-ttu-id="b526b-164">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="b526b-164">Chat.Read</span></span> |
|<span data-ttu-id="b526b-165">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b526b-165">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b526b-166">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b526b-166">Not supported.</span></span>    |
|<span data-ttu-id="b526b-167">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b526b-167">Application</span></span> | <span data-ttu-id="b526b-168">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="b526b-168">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="b526b-169">Exemplo 1: assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="b526b-169">Example 1: Subscribe to messages in a chat</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="b526b-170">Exemplo 2: assinar para receber mensagens em um chat que contenham determinado texto</span><span class="sxs-lookup"><span data-stu-id="b526b-170">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="b526b-171">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="b526b-171">The following request will send messages that contain `Hello` to the subscriber.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="b526b-172">Exemplo 3: assinar para receber mensagens (e respostas) em um chat sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="b526b-172">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="see-also"></a><span data-ttu-id="b526b-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="b526b-173">See also</span></span>
- [<span data-ttu-id="b526b-174">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b526b-174">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="b526b-175">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b526b-175">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
