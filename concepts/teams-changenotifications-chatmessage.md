---
title: Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph
description: As notificações de alterações te habilitam a ouvir as alterações nas mensagens no canal ou no chat
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 78718b1b486231ae2549323433312aa878806210
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941421"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a><span data-ttu-id="629c2-103">Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="629c2-103">Get change notifications for messages in Teams channels and chats using Microsoft Graph</span></span>

<span data-ttu-id="629c2-104">As notificações de alteração habilitam você a inscrever-se para receber alterações (criar, atualizar e excluir) de mensagens em um canal ou chat.</span><span class="sxs-lookup"><span data-stu-id="629c2-104">Change notifications enable you to subscribe to changes (create, update, and delete) to messages in a channel or chat.</span></span> <span data-ttu-id="629c2-105">As notificações da alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="629c2-105">Change notifications provide a low latency model by allowing you to maintain a subscription.</span></span> <span data-ttu-id="629c2-106">Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter a carga útil.</span><span class="sxs-lookup"><span data-stu-id="629c2-106">You can also get the resource data in the notifications and therefore avoid calling the API to get the payload.</span></span>

## <a name="subscribe-to-changes-at-the-tenant-level"></a><span data-ttu-id="629c2-107">Assinar para receber alterações no nível do locatário</span><span class="sxs-lookup"><span data-stu-id="629c2-107">Subscribe to changes at the tenant level</span></span>

<span data-ttu-id="629c2-108">Para acompanhar todas as alterações relacionadas a mensagens em um locatário, você pode usar assinaturas em um nível de locatário para mensagens de canal e chat.</span><span class="sxs-lookup"><span data-stu-id="629c2-108">To track all changes related to messages in a tenant, you can use subscriptions at a tenant level for channel and chat messages.</span></span> <span data-ttu-id="629c2-109">Isso requer que você crie duas assinaturas: uma para acompanhar todas as mensagens nos [canais](/graph/api/resources/channel?preserve-view=true) e outra para acompanhar todas as mensagens nos [chats](/graph/api/resources/chat?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="629c2-109">This requires you to create two subscriptions: one to track all messages across [channels](/graph/api/resources/channel?preserve-view=true), and one to track all messages across [chats](/graph/api/resources/chat?preserve-view=true).</span></span>

### <a name="subscribe-to-messages-across-channels"></a><span data-ttu-id="629c2-110">Assine para receber mensagens em todos os canais</span><span class="sxs-lookup"><span data-stu-id="629c2-110">Subscribe to messages across channels</span></span>

<span data-ttu-id="629c2-111">Para obter notificações de alteração para todas as mensagens e respostas nos canais de um locatário, assine em `/teams/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="629c2-111">To get to change notifications for all messages and replies across channels in a tenant, subscribe to `/teams/getAllMessages`.</span></span> <span data-ttu-id="629c2-112">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="629c2-112">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="629c2-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="629c2-113">Permissions</span></span>

|<span data-ttu-id="629c2-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629c2-114">Permission type</span></span>      | <span data-ttu-id="629c2-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629c2-115">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="629c2-116">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="629c2-116">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="629c2-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629c2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="629c2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-118">Not supported.</span></span> | <span data-ttu-id="629c2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-119">Not supported.</span></span> |
|<span data-ttu-id="629c2-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629c2-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629c2-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-121">Not supported.</span></span>    | <span data-ttu-id="629c2-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-122">Not supported.</span></span> |
|<span data-ttu-id="629c2-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629c2-123">Application</span></span> | <span data-ttu-id="629c2-124">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="629c2-124">ChannelMessage.Read.All</span></span> | <span data-ttu-id="629c2-125">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-125">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="629c2-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="629c2-126">Example</span></span>

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

### <a name="subscribe-to-messages-across-chats"></a><span data-ttu-id="629c2-127">Assinar para receber mensagens em chats</span><span class="sxs-lookup"><span data-stu-id="629c2-127">Subscribe to messages across chats</span></span>

<span data-ttu-id="629c2-128">Para obter notificações de alteração para todas as mensagens em chats em um locatário, assine em `/chats/getAllMessages`.</span><span class="sxs-lookup"><span data-stu-id="629c2-128">To get change notifications for all messages across chats in a tenant, subscribe to `/chats/getAllMessages`.</span></span> <span data-ttu-id="629c2-129">Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.</span><span class="sxs-lookup"><span data-stu-id="629c2-129">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification.</span></span>

#### <a name="permissions"></a><span data-ttu-id="629c2-130">Permissões</span><span class="sxs-lookup"><span data-stu-id="629c2-130">Permissions</span></span>

|<span data-ttu-id="629c2-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629c2-131">Permission type</span></span>      | <span data-ttu-id="629c2-132">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629c2-132">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="629c2-133">Versões com suporte</span><span class="sxs-lookup"><span data-stu-id="629c2-133">Supported versions</span></span> |
|:--------------------|:---------------------------------------------------------|:-------------------|
|<span data-ttu-id="629c2-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629c2-134">Delegated (work or school account)</span></span> | <span data-ttu-id="629c2-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-135">Not supported.</span></span> | <span data-ttu-id="629c2-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-136">Not supported.</span></span> |
|<span data-ttu-id="629c2-137">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629c2-137">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629c2-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-138">Not supported.</span></span>    | <span data-ttu-id="629c2-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-139">Not supported.</span></span> |
|<span data-ttu-id="629c2-140">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629c2-140">Application</span></span> | <span data-ttu-id="629c2-141">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="629c2-141">Chat.Read.All</span></span> | <span data-ttu-id="629c2-142">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-142">beta, v1.0</span></span> |

#### <a name="example"></a><span data-ttu-id="629c2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="629c2-143">Example</span></span>

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

## <a name="subscribe-to-messages-in-a-channel"></a><span data-ttu-id="629c2-144">Assine em mensagens em um canal</span><span class="sxs-lookup"><span data-stu-id="629c2-144">Subscribe to messages in a channel</span></span>

<span data-ttu-id="629c2-145">Para acompanhar mensagens e respostas em um canal, você pode criar uma assinatura de notificação de alteraração no nível do canal.</span><span class="sxs-lookup"><span data-stu-id="629c2-145">To track messages and replies in a channel, you can create a change notification subscription at a channel level.</span></span> <span data-ttu-id="629c2-146">Para fazer isso, assine em `/teams{id}/channels/{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="629c2-146">To do this, subscribe to `/teams{id}/channels/{id}/messages`.</span></span> <span data-ttu-id="629c2-147">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="629c2-147">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="629c2-148">As assinaturas no nível do canal também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="629c2-148">Channel-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

### <a name="permissions"></a><span data-ttu-id="629c2-149">Permissões</span><span class="sxs-lookup"><span data-stu-id="629c2-149">Permissions</span></span>

|<span data-ttu-id="629c2-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629c2-150">Permission type</span></span>      | <span data-ttu-id="629c2-151">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629c2-151">Permissions (from least to most privileged)</span></span>              |<span data-ttu-id="629c2-152">Com suporte na versão</span><span class="sxs-lookup"><span data-stu-id="629c2-152">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:--------------------|
|<span data-ttu-id="629c2-153">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629c2-153">Delegated (work or school account)</span></span> | <span data-ttu-id="629c2-154">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="629c2-154">ChannelMessage.Read.All</span></span> | <span data-ttu-id="629c2-155">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-155">beta, v1.0</span></span> |
|<span data-ttu-id="629c2-156">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629c2-156">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629c2-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-157">Not supported.</span></span>    | <span data-ttu-id="629c2-158">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-158">Not supported.</span></span> |
|<span data-ttu-id="629c2-159">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629c2-159">Application</span></span> | <span data-ttu-id="629c2-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span><span class="sxs-lookup"><span data-stu-id="629c2-160">ChannelMessage.Read.All, ChannelMessage.Read.Group\*</span></span> | <span data-ttu-id="629c2-161">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-161">beta, v1.0</span></span> |

><span data-ttu-id="629c2-162">**Observação:** ChannelMessage.Read.Group é suportado como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span><span class="sxs-lookup"><span data-stu-id="629c2-162">**Note:** ChannelMessage.Read.Group is supported as part of [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a><span data-ttu-id="629c2-163">Exemplo 1: assinar em todas as mensagens (e respostas) em um canal</span><span class="sxs-lookup"><span data-stu-id="629c2-163">Example 1: Subscribe to all messages (and replies) in a channel</span></span>

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

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a><span data-ttu-id="629c2-164">Exemplo 2: assinar para receber mensagens (e respostas) em um canal que contém determinado texto</span><span class="sxs-lookup"><span data-stu-id="629c2-164">Example 2: Subscribe to messages (and replies) in a channel that contain certain text</span></span>

<span data-ttu-id="629c2-165">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="629c2-165">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a><span data-ttu-id="629c2-166">Exemplo 3: assinar para receber mensagens (e respostas) em um canal sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="629c2-166">Example 3: Subscribe to messages (and replies) in a channel without resource data</span></span>

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

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a><span data-ttu-id="629c2-167">Exemplo 4: assinar para receber mensagens (e respostas) em um canal que menciona um usuário específico</span><span class="sxs-lookup"><span data-stu-id="629c2-167">Example 4: Subscribe to messages (and replies) in a channel that mention a specific user</span></span>

<span data-ttu-id="629c2-168">Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.</span><span class="sxs-lookup"><span data-stu-id="629c2-168">To get notifications only for messages where a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="subscribe-to-messages-in-a-chat"></a><span data-ttu-id="629c2-169">Assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="629c2-169">Subscribe to messages in a chat</span></span>

<span data-ttu-id="629c2-170">Para acompanhar mensagens em um chat, você pode criar uma assinatura de notificação de alteração em um nível de chat.</span><span class="sxs-lookup"><span data-stu-id="629c2-170">To track messages in a chat, you can create a change notification subscription at a chat level.</span></span> <span data-ttu-id="629c2-171">Para fazer isso, assine em `/chats{id}/messages`.</span><span class="sxs-lookup"><span data-stu-id="629c2-171">To do this, subscribe to `/chats{id}/messages`.</span></span> <span data-ttu-id="629c2-172">Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.</span><span class="sxs-lookup"><span data-stu-id="629c2-172">This resource supports [including resource data](webhooks-with-resource-data.md) in the notification in *application-only mode*.</span></span>

<span data-ttu-id="629c2-173">As assinaturas no nível do chat também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.</span><span class="sxs-lookup"><span data-stu-id="629c2-173">Chat-level subscriptions also support keyword-based search via the `$search` query parameter.</span></span>

> <span data-ttu-id="629c2-174">**Observação:**</span><span class="sxs-lookup"><span data-stu-id="629c2-174">**Note.**</span></span> <span data-ttu-id="629c2-175">assinar para receber mensagens em um chat que esteja atualmente em pré-visualização.</span><span class="sxs-lookup"><span data-stu-id="629c2-175">Subcribing to messages in a chat is currently in preview.</span></span>

### <a name="permissions"></a><span data-ttu-id="629c2-176">Permissões</span><span class="sxs-lookup"><span data-stu-id="629c2-176">Permissions</span></span>

|<span data-ttu-id="629c2-177">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="629c2-177">Permission type</span></span>      | <span data-ttu-id="629c2-178">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="629c2-178">Permissions (from least to most privileged)</span></span>              | <span data-ttu-id="629c2-179">Com suporte na versão</span><span class="sxs-lookup"><span data-stu-id="629c2-179">Supported in version</span></span> |
|:--------------------|:---------------------------------------------------------|:---------------------|
|<span data-ttu-id="629c2-180">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="629c2-180">Delegated (work or school account)</span></span> | <span data-ttu-id="629c2-181">Chat.Read</span><span class="sxs-lookup"><span data-stu-id="629c2-181">Chat.Read</span></span> | <span data-ttu-id="629c2-182">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-182">beta, v1.0</span></span> |
|<span data-ttu-id="629c2-183">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="629c2-183">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="629c2-184">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-184">Not supported.</span></span>    | <span data-ttu-id="629c2-185">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="629c2-185">Not supported.</span></span> |
|<span data-ttu-id="629c2-186">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="629c2-186">Application</span></span> | <span data-ttu-id="629c2-187">Chat.Read.All</span><span class="sxs-lookup"><span data-stu-id="629c2-187">Chat.Read.All</span></span> | <span data-ttu-id="629c2-188">beta, v1.0</span><span class="sxs-lookup"><span data-stu-id="629c2-188">beta, v1.0</span></span> |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a><span data-ttu-id="629c2-189">Exemplo 1: assinar para receber mensagens em um chat</span><span class="sxs-lookup"><span data-stu-id="629c2-189">Example 1: Subscribe to messages in a chat</span></span>

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

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a><span data-ttu-id="629c2-190">Exemplo 2: assinar para receber mensagens em um chat que contenham determinado texto</span><span class="sxs-lookup"><span data-stu-id="629c2-190">Example 2: Subscribe to messages in a chat that contain certain text</span></span>

<span data-ttu-id="629c2-191">A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.</span><span class="sxs-lookup"><span data-stu-id="629c2-191">The following request will send messages that contain `Hello` to the subscriber.</span></span>

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

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a><span data-ttu-id="629c2-192">Exemplo 3: assinar para receber mensagens (e respostas) em um chat sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="629c2-192">Example 3: Subscribe to messages (and replies) in a chat without resource data</span></span>

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

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a><span data-ttu-id="629c2-193">Exemplo 4: assinar para receber mensagem em um chat no qual um usuário específico for mencionado</span><span class="sxs-lookup"><span data-stu-id="629c2-193">Example 4: Subscribe to message in a chat in which a specific user is mentioned</span></span>

<span data-ttu-id="629c2-194">Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.</span><span class="sxs-lookup"><span data-stu-id="629c2-194">To get notifications only for messages in which a specific user has been mentioned, you can specify the user's ID (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` in this example) in the query.</span></span>

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

## <a name="notification-payloads"></a><span data-ttu-id="629c2-195">Notificação de conteúdo</span><span class="sxs-lookup"><span data-stu-id="629c2-195">Notification payloads</span></span>

<span data-ttu-id="629c2-196">Dependendo da sua assinatura, você pode receber a notificação com dados de recursos ou sem ele.</span><span class="sxs-lookup"><span data-stu-id="629c2-196">Depending on your subscription, you can either get the notification with resource data, or without it.</span></span> <span data-ttu-id="629c2-197">Assinar com dados de recursos permite que você receba a carga da mensagem junto com a notificação, removendo a necessidade de ligar de volta e obter o conteúdo.</span><span class="sxs-lookup"><span data-stu-id="629c2-197">Subscribing with resource data allows you to get the message payload along with the notification, removing the need to call back and get the content.</span></span>

### <a name="notifications-with-resource-data"></a><span data-ttu-id="629c2-198">Notificações com dados de recursos</span><span class="sxs-lookup"><span data-stu-id="629c2-198">Notifications with resource data</span></span>

<span data-ttu-id="629c2-199">Para notificações com dados de recursos, a carga se parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="629c2-199">For notifications with resource data, the payload looks like the following.</span></span> <span data-ttu-id="629c2-200">Este conteúdo é para uma mensagem enviada em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="629c2-200">This payload is for a message sent in a chat.</span></span>

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

<span data-ttu-id="629c2-201">Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).</span><span class="sxs-lookup"><span data-stu-id="629c2-201">For details about how to validate tokens and decrypt the payload, see [Set up change notifications that include resource data](webhooks-with-resource-data.md).</span></span>

<span data-ttu-id="629c2-202">A carga de notificação descriptografada parece com a seguinte.</span><span class="sxs-lookup"><span data-stu-id="629c2-202">The decrypted notification payload looks like the following.</span></span> <span data-ttu-id="629c2-203">A carga está de acordo com o esquema [chatMessage](/graph/api/resources/chatMessage?preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="629c2-203">The payload conforms to the [chatMessage](/graph/api/resources/chatMessage?preserve-view=true) schema.</span></span> <span data-ttu-id="629c2-204">A carga é semelhante à devolvida pelas operações GET.</span><span class="sxs-lookup"><span data-stu-id="629c2-204">The payload is similar to that returned by GET operations.</span></span>

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a><span data-ttu-id="629c2-205">Notificações sem dados de recursos</span><span class="sxs-lookup"><span data-stu-id="629c2-205">Notifications without resource data</span></span>

<span data-ttu-id="629c2-206">Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="629c2-206">Notifications without resource data give you enough information to make GET calls to get the message content.</span></span> <span data-ttu-id="629c2-207">As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).</span><span class="sxs-lookup"><span data-stu-id="629c2-207">Subscriptions for notifications without resource data do not require an encryption certificate (because actual resource data is not sent over).</span></span>

<span data-ttu-id="629c2-208">A carga parece ser a seguinte.</span><span class="sxs-lookup"><span data-stu-id="629c2-208">The payload looks like the following.</span></span> <span data-ttu-id="629c2-209">Este conteúdo é para uma mensagem enviada em um canal.</span><span class="sxs-lookup"><span data-stu-id="629c2-209">This payload is for a message sent in a channel.</span></span>

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

<span data-ttu-id="629c2-210">As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="629c2-210">The **resource** and **@odata.id** properties can be used to make calls to Microsoft Graph to get the payload for the message.</span></span> <span data-ttu-id="629c2-211">As chamadas GET sempre retornarão o estado atual da mensagem.</span><span class="sxs-lookup"><span data-stu-id="629c2-211">GET calls will always return the current state of the message.</span></span> <span data-ttu-id="629c2-212">Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.</span><span class="sxs-lookup"><span data-stu-id="629c2-212">If the message is changed between when the notification is sent and when the message is retrieved, the operation will return the updated message.</span></span>

## <a name="see-also"></a><span data-ttu-id="629c2-213">Confira também</span><span class="sxs-lookup"><span data-stu-id="629c2-213">See also</span></span>
- [<span data-ttu-id="629c2-214">Notificações de alteração do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="629c2-214">Microsoft Graph change notifications</span></span>](webhooks.md)
- [<span data-ttu-id="629c2-215">Visão geral da API do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="629c2-215">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
