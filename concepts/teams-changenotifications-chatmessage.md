---
title: Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph
description: As notificações de alterações te habilitam a ouvir as alterações nas mensagens no canal ou no chat
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 12d8bfd49ebc71b6cb82cccd9525a3706cd570fd
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690610"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="e33a3-103">Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e33a3-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="e33a3-104">As notificações de alteração habilitam você a assinar para receber alterações (criar, atualizar e excluir) de [ mensagens ](/graph/api/resources/chatMessage?preserve-view=true) em um [ canal ](/graph/api/resources/channel?preserve-view=true) ou [chat](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e33a3-104">Change notifications enable you to subscribe to changes (create, update, and delete) to [messages](/graph/api/resources/chatMessage?preserve-view=true) in a [channel](/graph/api/resources/channel?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true).</span></span> <span data-ttu-id="e33a3-105">As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e33a3-105">Change notifications provide a low latency model by allowing you to maintain a [subscription](/graph/api/resources/webhooks?preserve-view=true).</span></span> <span data-ttu-id="e33a3-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e33a3-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

><span data-ttu-id="e33a3-107">**Observação:** o tempo máximo que uma assinatura pode durar é 60 minutos; entretanto, as assinaturas podem ser renovadas até que o chamador tenha permissão para acessar o recurso.</span><span class="sxs-lookup"><span data-stu-id="e33a3-107">**Note:** The maximum time a subscription can last is 60 minutes; however, subscriptions can be renewed until the caller has permissions to access to resource.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="e33a3-108">Assinar para receber alterações no nível do locatário</span><span class="sxs-lookup"><span data-stu-id="e33a3-108">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="e33a3-109">Para acompanhar todas as alterações relacionadas a mensagens em um locatário, você pode usar assinaturas em um nível de locatário para mensagens de canal e chat.</span><span class="sxs-lookup"><span data-stu-id="e33a3-109">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="e33a3-110">Isso requer que você crie duas assinaturas: uma para acompanhar todas as mensagens nos [canais](/graph/api/resources/channel?preserve-view=true) e outra para acompanhar todas as mensagens nos [chats](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="e33a3-110">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="e33a3-111">Assine para receber mensagens em todos os canais</span><span class="sxs-lookup"><span data-stu-id="e33a3-111">Subscribe to messages across channels</span></span>

<span data-ttu-id="e33a3-112">Para obter notificações de alteração para todas as mensagens e respostas nos canais de um locatário, assine em `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-112">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="e33a3-113">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="e33a3-113">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="e33a3-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="e33a3-114">Permissions</span></span>

|<span data-ttu-id="e33a3-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33a3-115">Permission type</span></span>      | <span data-ttu-id="e33a3-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e33a3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33a3-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33a3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e33a3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-118">Not supported.</span></span> |
|<span data-ttu-id="e33a3-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33a3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33a3-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-120">Not supported.</span></span>    |
|<span data-ttu-id="e33a3-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33a3-121">Application</span></span> | <span data-ttu-id="e33a3-122">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33a3-122">ChannelMessage.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="e33a3-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e33a3-123">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="e33a3-124">Assinar para receber mensagens em chats</span><span class="sxs-lookup"><span data-stu-id="e33a3-124">Subscribe to messages across chats</span></span>

<span data-ttu-id="e33a3-125">Para obter notificações de alteração para todas as mensagens em chats em um locatário, assine em `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-125">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="e33a3-126">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="e33a3-126">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="e33a3-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="e33a3-127">Permissions</span></span>

|<span data-ttu-id="e33a3-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33a3-128">Permission type</span></span>      | <span data-ttu-id="e33a3-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e33a3-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33a3-130">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33a3-130">Delegated (work or school account)</span></span> | <span data-ttu-id="e33a3-131">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-131">Not supported.</span></span> |
|<span data-ttu-id="e33a3-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33a3-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33a3-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-133">Not supported.</span></span>    |
|<span data-ttu-id="e33a3-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33a3-134">Application</span></span> | <span data-ttu-id="e33a3-135">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33a3-135">Chat.Read.All</span></span> |

#### <a name="example"></a><span data-ttu-id="e33a3-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e33a3-136">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="e33a3-137">Assine em mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="e33a3-137">Subscribe to messages in a channel</span></span>

<span data-ttu-id="e33a3-138">Para acompanhar mensagens e respostas em um canal, você pode criar uma assinatura de notificação de alteraração no nível do canal.</span><span class="sxs-lookup"><span data-stu-id="e33a3-138">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="e33a3-139">Para fazer isso, assine em `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-139">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="e33a3-140">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="e33a3-140">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="e33a3-141">As assinaturas no nível do canal também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-141">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="e33a3-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="e33a3-142">Permissions</span></span>

|<span data-ttu-id="e33a3-143">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33a3-143">Permission type</span></span>      | <span data-ttu-id="e33a3-144">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e33a3-144">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33a3-145">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33a3-145">Delegated (work or school account)</span></span> | <span data-ttu-id="e33a3-146">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33a3-146">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="e33a3-147">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33a3-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33a3-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-148">Not supported.</span></span>    |
|<span data-ttu-id="e33a3-149">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33a3-149">Application</span></span> | <span data-ttu-id="e33a3-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="e33a3-150">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> |

><span data-ttu-id="e33a3-151">**Observação:** ChannelMessage.Read.Group é suportado como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="e33a3-151">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="e33a3-152">Exemplo 1: assinar em todas as mensagens (e respostas) em um canal</span><span class="sxs-lookup"><span data-stu-id="e33a3-152">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="e33a3-153">Exemplo 2: assinar para receber mensagens (e respostas) em um canal que contém determinado texto</span><span class="sxs-lookup"><span data-stu-id="e33a3-153">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="e33a3-154">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="e33a3-154">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="e33a3-155">Exemplo 3: assinar para receber mensagens (e respostas) em um canal sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="e33a3-155">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="e33a3-156">Exemplo 4: assinar para receber mensagens (e respostas) em um canal que menciona um usuário específico</span><span class="sxs-lookup"><span data-stu-id="e33a3-156">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="e33a3-157">Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.</span><span class="sxs-lookup"><span data-stu-id="e33a3-157">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="e33a3-158">Assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="e33a3-158">Subscribe to messages in a chat</span></span>

<span data-ttu-id="e33a3-159">Para acompanhar mensagens em um chat, você pode criar uma assinatura de notificação de alteração em um nível de chat.</span><span class="sxs-lookup"><span data-stu-id="e33a3-159">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="e33a3-160">Para fazer isso, assine em `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-160">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="e33a3-161">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="e33a3-161">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="e33a3-162">As assinaturas no nível do chat também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="e33a3-162">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="e33a3-163">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="e33a3-163">**Note.**</span></span> <span data-ttu-id="e33a3-164">assinar para receber mensagens em um chat que esteja atualmente em pré-visualização.</span><span class="sxs-lookup"><span data-stu-id="e33a3-164">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="e33a3-165">Permissões</span><span class="sxs-lookup"><span data-stu-id="e33a3-165">Permissions</span></span>

|<span data-ttu-id="e33a3-166">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e33a3-166">Permission type</span></span>      | <span data-ttu-id="e33a3-167">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e33a3-167">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e33a3-168">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e33a3-168">Delegated (work or school account)</span></span> | <span data-ttu-id="e33a3-169">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="e33a3-169">Chat.Read</span></span> |
|<span data-ttu-id="e33a3-170">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e33a3-170">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e33a3-171">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e33a3-171">Not supported.</span></span>    |
|<span data-ttu-id="e33a3-172">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e33a3-172">Application</span></span> | <span data-ttu-id="e33a3-173">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="e33a3-173">Chat.Read.All</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="e33a3-174">Exemplo 1: assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="e33a3-174">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="e33a3-175">Exemplo 2: assinar para receber mensagens em um chat que contenham determinado texto</span><span class="sxs-lookup"><span data-stu-id="e33a3-175">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="e33a3-176">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="e33a3-176">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="e33a3-177">Exemplo 3: assinar para receber mensagens (e respostas) em um chat sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="e33a3-177">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="e33a3-178">Exemplo 4: assinar para receber mensagem em um chat no qual um usuário específico for mencionado</span><span class="sxs-lookup"><span data-stu-id="e33a3-178">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="e33a3-179">Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.</span><span class="sxs-lookup"><span data-stu-id="e33a3-179">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="see-also"></a><span data-ttu-id="e33a3-180">Confira também</span><span class="sxs-lookup"><span data-stu-id="e33a3-180">See also</span></span>
- [<span data-ttu-id="e33a3-181">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e33a3-181">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="e33a3-182">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e33a3-182">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
