---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 0d11230402d95009e414c16962a2eb9b5dce1f58
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333362"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="cce57-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cce57-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="cce57-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="cce57-106">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="cce57-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cce57-107">Methods</span></span>

| <span data-ttu-id="cce57-108">Método</span><span class="sxs-lookup"><span data-stu-id="cce57-108">Method</span></span>       | <span data-ttu-id="cce57-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cce57-109">Return Type</span></span>  |<span data-ttu-id="cce57-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cce57-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cce57-111">Listar canal chat</span><span class="sxs-lookup"><span data-stu-id="cce57-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="cce57-112">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="cce57-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="cce57-113">Lista de todas as mensagens de chat raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="cce57-114">Obter chatMessages em um Delta de canal</span><span class="sxs-lookup"><span data-stu-id="cce57-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="cce57-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cce57-116">Obter mensagens de chat incrementais em um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="cce57-117">Obter canal chat</span><span class="sxs-lookup"><span data-stu-id="cce57-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="cce57-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="cce57-119">Obtenha uma única mensagem de chat raiz de um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="cce57-120">Listar respostas a um chat</span><span class="sxs-lookup"><span data-stu-id="cce57-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="cce57-121">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="cce57-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="cce57-122">Lista de todas as respostas para uma mensagem de chat no canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="cce57-123">Obter uma resposta para um chat</span><span class="sxs-lookup"><span data-stu-id="cce57-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="cce57-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cce57-125">Obter uma única resposta para uma mensagem de chat em um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="cce57-126">Criar chat em um canal</span><span class="sxs-lookup"><span data-stu-id="cce57-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="cce57-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cce57-128">Criar uma nova mensagem de chat de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="cce57-129">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="cce57-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="cce57-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cce57-131">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="cce57-132">Criar chat em um chat</span><span class="sxs-lookup"><span data-stu-id="cce57-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="cce57-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="cce57-134">Envie uma mensagem de chat em uma conversa existente de chat de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="cce57-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="cce57-135">Listar chatMessages em um chat</span><span class="sxs-lookup"><span data-stu-id="cce57-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="cce57-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cce57-137">Listar mensagens de chat em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="cce57-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="cce57-138">Obter chat no chat</span><span class="sxs-lookup"><span data-stu-id="cce57-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="cce57-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="cce57-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="cce57-140">Obter uma única mensagem de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="cce57-141">Listar todo o conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="cce57-141">List all hosted content</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | <span data-ttu-id="cce57-142">coleção [chatMessageHostedContent](../resources/chatmessagehostedcontent.md)</span><span class="sxs-lookup"><span data-stu-id="cce57-142">[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection</span></span>| <span data-ttu-id="cce57-143">Obter todo o conteúdo hospedado em uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-143">Get all hosted content in a chat message.</span></span>|
|[<span data-ttu-id="cce57-144">Obter conteúdo hospedado</span><span class="sxs-lookup"><span data-stu-id="cce57-144">Get hosted content</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="cce57-145">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="cce57-145">chatMessageHostedContent</span></span>](../resources/chatmessagehostedcontent.md) | <span data-ttu-id="cce57-146">Obter conteúdo hospedado de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-146">Get hosted content from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="cce57-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cce57-147">Properties</span></span>

| <span data-ttu-id="cce57-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cce57-148">Property</span></span>   | <span data-ttu-id="cce57-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="cce57-149">Type</span></span> |<span data-ttu-id="cce57-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="cce57-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cce57-151">id</span><span class="sxs-lookup"><span data-stu-id="cce57-151">id</span></span>|<span data-ttu-id="cce57-152">String</span><span class="sxs-lookup"><span data-stu-id="cce57-152">String</span></span>| <span data-ttu-id="cce57-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-153">Read-only.</span></span> <span data-ttu-id="cce57-154">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="cce57-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="cce57-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="cce57-155">replyToId</span></span>| <span data-ttu-id="cce57-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cce57-156">string</span></span> | <span data-ttu-id="cce57-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-157">Read-only.</span></span> <span data-ttu-id="cce57-158">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="cce57-158">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="cce57-159">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="cce57-159">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="cce57-160">from</span><span class="sxs-lookup"><span data-stu-id="cce57-160">from</span></span>|[<span data-ttu-id="cce57-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="cce57-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="cce57-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-162">Read only.</span></span> <span data-ttu-id="cce57-163">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-163">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="cce57-164">etag</span><span class="sxs-lookup"><span data-stu-id="cce57-164">etag</span></span>| <span data-ttu-id="cce57-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cce57-165">string</span></span> | <span data-ttu-id="cce57-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-166">Read-only.</span></span> <span data-ttu-id="cce57-167">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-167">Version number of the chat message.</span></span> |
|<span data-ttu-id="cce57-168">messageType</span><span class="sxs-lookup"><span data-stu-id="cce57-168">messageType</span></span>|<span data-ttu-id="cce57-169">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="cce57-169">chatMessageType</span></span>|<span data-ttu-id="cce57-170">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-170">The type of chat message.</span></span> <span data-ttu-id="cce57-171">Os valores possíveis são: `message`.</span><span class="sxs-lookup"><span data-stu-id="cce57-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="cce57-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cce57-172">createdDateTime</span></span>|<span data-ttu-id="cce57-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cce57-173">dateTimeOffset</span></span>|<span data-ttu-id="cce57-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-174">Read only.</span></span> <span data-ttu-id="cce57-175">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="cce57-175">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="cce57-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cce57-176">lastModifiedDateTime</span></span>|<span data-ttu-id="cce57-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cce57-177">dateTimeOffset</span></span>|<span data-ttu-id="cce57-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-178">Read only.</span></span> <span data-ttu-id="cce57-179">Carimbo de data/hora de quando a mensagem de chat é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem de chat raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="cce57-179">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="cce57-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="cce57-180">deletedDateTime</span></span>|<span data-ttu-id="cce57-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cce57-181">dateTimeOffset</span></span>|<span data-ttu-id="cce57-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cce57-182">Read only.</span></span> <span data-ttu-id="cce57-183">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="cce57-183">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="cce57-184">assunto</span><span class="sxs-lookup"><span data-stu-id="cce57-184">subject</span></span>|<span data-ttu-id="cce57-185">string</span><span class="sxs-lookup"><span data-stu-id="cce57-185">string</span></span>| <span data-ttu-id="cce57-186">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="cce57-186">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="cce57-187">corpo</span><span class="sxs-lookup"><span data-stu-id="cce57-187">body</span></span>|[<span data-ttu-id="cce57-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="cce57-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="cce57-189">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-189">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="cce57-190">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="cce57-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="cce57-191">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="cce57-191">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="cce57-192">summary</span><span class="sxs-lookup"><span data-stu-id="cce57-192">summary</span></span>|<span data-ttu-id="cce57-193">string</span><span class="sxs-lookup"><span data-stu-id="cce57-193">string</span></span>| <span data-ttu-id="cce57-194">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="cce57-194">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="cce57-195">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-195">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="cce57-196">attachments</span><span class="sxs-lookup"><span data-stu-id="cce57-196">attachments</span></span>|<span data-ttu-id="cce57-197">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="cce57-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="cce57-198">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="cce57-198">Attached files.</span></span> <span data-ttu-id="cce57-199">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="cce57-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="cce57-200">mentions</span><span class="sxs-lookup"><span data-stu-id="cce57-200">mentions</span></span>|<span data-ttu-id="cce57-201">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="cce57-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="cce57-202">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-202">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="cce57-203">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="cce57-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="cce57-204">importância</span><span class="sxs-lookup"><span data-stu-id="cce57-204">importance</span></span>| <span data-ttu-id="cce57-205">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="cce57-205">chatMessageImportance</span></span> | <span data-ttu-id="cce57-206">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="cce57-206">The importance of the chat message.</span></span> <span data-ttu-id="cce57-207">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="cce57-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="cce57-208">reactions</span><span class="sxs-lookup"><span data-stu-id="cce57-208">reactions</span></span>| <span data-ttu-id="cce57-209">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="cce57-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="cce57-210">Reações para esta mensagem de chat (por exemplo, como).</span><span class="sxs-lookup"><span data-stu-id="cce57-210">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="cce57-211">localidade</span><span class="sxs-lookup"><span data-stu-id="cce57-211">locale</span></span>|<span data-ttu-id="cce57-212">string</span><span class="sxs-lookup"><span data-stu-id="cce57-212">string</span></span>|<span data-ttu-id="cce57-213">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cce57-213">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cce57-214">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cce57-214">JSON representation</span></span>

<span data-ttu-id="cce57-215">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cce57-215">The following is a JSON representation of the resource.</span></span>

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
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
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
