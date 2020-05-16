---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 3a5f59c16e19fae5da17f8d43efc1f2ba63f00d4
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272686"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="bc8ed-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-104">chatMessage resource type</span></span>

<span data-ttu-id="bc8ed-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc8ed-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc8ed-106">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="bc8ed-106">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="bc8ed-107">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="bc8ed-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc8ed-108">Methods</span></span>

| <span data-ttu-id="bc8ed-109">Método</span><span class="sxs-lookup"><span data-stu-id="bc8ed-109">Method</span></span>       | <span data-ttu-id="bc8ed-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc8ed-110">Return Type</span></span>  |<span data-ttu-id="bc8ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc8ed-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc8ed-112">**Mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="bc8ed-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="bc8ed-113">Listar canal chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="bc8ed-114">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc8ed-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="bc8ed-115">Lista de todas as mensagens de chat raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="bc8ed-116">Obter chatMessages em um Delta de canal</span><span class="sxs-lookup"><span data-stu-id="bc8ed-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="bc8ed-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="bc8ed-118">Obter mensagens de chat incrementais em um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="bc8ed-119">Criar assinatura para novas mensagens de canal</span><span class="sxs-lookup"><span data-stu-id="bc8ed-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="bc8ed-120">assinatura</span><span class="sxs-lookup"><span data-stu-id="bc8ed-120">subscription</span></span>](subscription.md) | <span data-ttu-id="bc8ed-121">Ouvir mensagens de canal novas e editadas e reações para elas.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="bc8ed-122">Obter canal chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="bc8ed-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="bc8ed-124">Obtenha uma única mensagem de chat raiz de um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="bc8ed-125">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="bc8ed-125">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="bc8ed-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="bc8ed-127">Criar uma nova mensagem de chat de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-127">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="bc8ed-128">**Respostas de mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="bc8ed-128">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="bc8ed-129">Listar respostas a um chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-129">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="bc8ed-130">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc8ed-130">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="bc8ed-131">Lista de todas as respostas para uma mensagem de chat no canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-131">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="bc8ed-132">Obter uma resposta para um chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-132">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="bc8ed-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="bc8ed-134">Obter uma única resposta para uma mensagem de chat em um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-134">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="bc8ed-135">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="bc8ed-135">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="bc8ed-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="bc8ed-137">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-137">Reply to an existing chat message in a channel.</span></span>|
|<span data-ttu-id="bc8ed-138">**1:1 e mensagens de chat de grupo**</span><span class="sxs-lookup"><span data-stu-id="bc8ed-138">**1:1 and group chat messages**</span></span>| | |
|[<span data-ttu-id="bc8ed-139">Criar chat em um chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-139">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="bc8ed-140">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-140">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="bc8ed-141">Envie uma mensagem de chat em uma conversa existente de chat de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-141">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="bc8ed-142">Listar chatMessages em um chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-142">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="bc8ed-143">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-143">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="bc8ed-144">Listar mensagens de chat em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-144">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="bc8ed-145">Criar assinatura para novas mensagens de chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-145">Create subscription for new chat messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="bc8ed-146">assinatura</span><span class="sxs-lookup"><span data-stu-id="bc8ed-146">subscription</span></span>](subscription.md) | <span data-ttu-id="bc8ed-147">Ouvir mensagens de chat novas e editadas e reações para elas.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-147">Listen for new and edited chat messages, and reactions to them.</span></span> |
|[<span data-ttu-id="bc8ed-148">Obter chat no chat</span><span class="sxs-lookup"><span data-stu-id="bc8ed-148">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="bc8ed-149">chatMessage</span><span class="sxs-lookup"><span data-stu-id="bc8ed-149">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="bc8ed-150">Obter uma única mensagem de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-150">Get a single chat message in a chat.</span></span> |
|<span data-ttu-id="bc8ed-151">**Conteúdo hospedado**</span><span class="sxs-lookup"><span data-stu-id="bc8ed-151">**Hosted content**</span></span>| | |
|[<span data-ttu-id="bc8ed-152">Listar todo o conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="bc8ed-152">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="bc8ed-153">coleção [chatMessageHostedContent](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="bc8ed-153">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="bc8ed-154">Obter todo o conteúdo hospedado em uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-154">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="bc8ed-155">Obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="bc8ed-155">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="bc8ed-156">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="bc8ed-156">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="bc8ed-157">Obter conteúdo hospedado de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-157">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc8ed-158">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc8ed-158">Properties</span></span>

| <span data-ttu-id="bc8ed-159">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc8ed-159">Property</span></span>   | <span data-ttu-id="bc8ed-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc8ed-160">Type</span></span> |<span data-ttu-id="bc8ed-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc8ed-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc8ed-162">id</span><span class="sxs-lookup"><span data-stu-id="bc8ed-162">id</span></span>|<span data-ttu-id="bc8ed-163">String</span><span class="sxs-lookup"><span data-stu-id="bc8ed-163">String</span></span>| <span data-ttu-id="bc8ed-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-164">Read-only.</span></span> <span data-ttu-id="bc8ed-165">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-165">Unique Id of the message.</span></span>|
|<span data-ttu-id="bc8ed-166">replyToId</span><span class="sxs-lookup"><span data-stu-id="bc8ed-166">replyToId</span></span>| <span data-ttu-id="bc8ed-167">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc8ed-167">string</span></span> | <span data-ttu-id="bc8ed-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-168">Read-only.</span></span> <span data-ttu-id="bc8ed-169">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-169">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="bc8ed-170">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="bc8ed-170">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="bc8ed-171">from</span><span class="sxs-lookup"><span data-stu-id="bc8ed-171">from</span></span>|[<span data-ttu-id="bc8ed-172">identitySet</span><span class="sxs-lookup"><span data-stu-id="bc8ed-172">identitySet</span></span>](identityset.md)| <span data-ttu-id="bc8ed-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-173">Read only.</span></span> <span data-ttu-id="bc8ed-174">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-174">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="bc8ed-175">etag</span><span class="sxs-lookup"><span data-stu-id="bc8ed-175">etag</span></span>| <span data-ttu-id="bc8ed-176">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc8ed-176">string</span></span> | <span data-ttu-id="bc8ed-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-177">Read-only.</span></span> <span data-ttu-id="bc8ed-178">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-178">Version number of the chat message.</span></span> |
|<span data-ttu-id="bc8ed-179">messageType</span><span class="sxs-lookup"><span data-stu-id="bc8ed-179">messageType</span></span>|<span data-ttu-id="bc8ed-180">string</span><span class="sxs-lookup"><span data-stu-id="bc8ed-180">string</span></span>|<span data-ttu-id="bc8ed-181">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-181">The type of chat message.</span></span> <span data-ttu-id="bc8ed-182">Os valores possíveis são: `message` .</span><span class="sxs-lookup"><span data-stu-id="bc8ed-182">The possible values are: `message`.</span></span>|
|<span data-ttu-id="bc8ed-183">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bc8ed-183">createdDateTime</span></span>|<span data-ttu-id="bc8ed-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc8ed-184">dateTimeOffset</span></span>|<span data-ttu-id="bc8ed-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-185">Read only.</span></span> <span data-ttu-id="bc8ed-186">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-186">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="bc8ed-187">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc8ed-187">lastModifiedDateTime</span></span>|<span data-ttu-id="bc8ed-188">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc8ed-188">dateTimeOffset</span></span>|<span data-ttu-id="bc8ed-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-189">Read only.</span></span> <span data-ttu-id="bc8ed-190">Carimbo de data/hora de quando a mensagem de chat é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem de chat raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-190">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="bc8ed-191">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc8ed-191">deletedDateTime</span></span>|<span data-ttu-id="bc8ed-192">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc8ed-192">dateTimeOffset</span></span>|<span data-ttu-id="bc8ed-193">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-193">Read only.</span></span> <span data-ttu-id="bc8ed-194">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-194">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="bc8ed-195">subject</span><span class="sxs-lookup"><span data-stu-id="bc8ed-195">subject</span></span>|<span data-ttu-id="bc8ed-196">string</span><span class="sxs-lookup"><span data-stu-id="bc8ed-196">string</span></span>| <span data-ttu-id="bc8ed-197">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-197">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="bc8ed-198">body</span><span class="sxs-lookup"><span data-stu-id="bc8ed-198">body</span></span>|[<span data-ttu-id="bc8ed-199">itemBody</span><span class="sxs-lookup"><span data-stu-id="bc8ed-199">itemBody</span></span>](itembody.md)|<span data-ttu-id="bc8ed-200">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-200">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="bc8ed-201">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-201">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="bc8ed-202">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="bc8ed-202">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="bc8ed-203">summary</span><span class="sxs-lookup"><span data-stu-id="bc8ed-203">summary</span></span>|<span data-ttu-id="bc8ed-204">string</span><span class="sxs-lookup"><span data-stu-id="bc8ed-204">string</span></span>| <span data-ttu-id="bc8ed-205">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-205">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="bc8ed-206">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-206">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="bc8ed-207">attachments</span><span class="sxs-lookup"><span data-stu-id="bc8ed-207">attachments</span></span>|<span data-ttu-id="bc8ed-208">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc8ed-208">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="bc8ed-209">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-209">Attached files.</span></span> <span data-ttu-id="bc8ed-210">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-210">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="bc8ed-211">mentions</span><span class="sxs-lookup"><span data-stu-id="bc8ed-211">mentions</span></span>|<span data-ttu-id="bc8ed-212">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc8ed-212">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="bc8ed-213">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-213">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="bc8ed-214">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-214">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="bc8ed-215">importância</span><span class="sxs-lookup"><span data-stu-id="bc8ed-215">importance</span></span>|<span data-ttu-id="bc8ed-216">string</span><span class="sxs-lookup"><span data-stu-id="bc8ed-216">string</span></span> | <span data-ttu-id="bc8ed-217">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-217">The importance of the chat message.</span></span> <span data-ttu-id="bc8ed-218">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-218">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="bc8ed-219">reactions</span><span class="sxs-lookup"><span data-stu-id="bc8ed-219">reactions</span></span>| <span data-ttu-id="bc8ed-220">[chatMessageReaction](./chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="bc8ed-220">[chatMessageReaction](./chatmessagereaction.md) collection</span></span> | <span data-ttu-id="bc8ed-221">Reações para esta mensagem de chat (por exemplo, como).</span><span class="sxs-lookup"><span data-stu-id="bc8ed-221">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="bc8ed-222">localidade</span><span class="sxs-lookup"><span data-stu-id="bc8ed-222">locale</span></span>|<span data-ttu-id="bc8ed-223">string</span><span class="sxs-lookup"><span data-stu-id="bc8ed-223">string</span></span>|<span data-ttu-id="bc8ed-224">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-224">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc8ed-225">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc8ed-225">JSON representation</span></span>

<span data-ttu-id="bc8ed-226">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc8ed-226">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions":  "string",
  "locale": "string",
  "deleted": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
