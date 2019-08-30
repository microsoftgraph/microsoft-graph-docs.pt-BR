---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: a29afea30f0ea1d75f5c7ce1a0713976f10cc298
ms.sourcegitcommit: cca4f96414aededa03bb45e07e19bb20b7327563
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2019
ms.locfileid: "36677117"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="500d4-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="500d4-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="500d4-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span> <span data-ttu-id="500d4-106">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-106">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="500d4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="500d4-107">Methods</span></span>

| <span data-ttu-id="500d4-108">Método</span><span class="sxs-lookup"><span data-stu-id="500d4-108">Method</span></span>       | <span data-ttu-id="500d4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="500d4-109">Return Type</span></span>  |<span data-ttu-id="500d4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="500d4-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="500d4-111">Listar canal chat</span><span class="sxs-lookup"><span data-stu-id="500d4-111">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="500d4-112">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="500d4-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="500d4-113">Lista de todas as mensagens de chat raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-113">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="500d4-114">Obter chatMessages em um Delta de canal</span><span class="sxs-lookup"><span data-stu-id="500d4-114">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="500d4-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-115">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="500d4-116">Obter mensagens de chat incrementais em um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-116">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="500d4-117">Obter canal chat</span><span class="sxs-lookup"><span data-stu-id="500d4-117">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="500d4-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-118">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="500d4-119">Obtenha uma única mensagem de chat raiz de um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-119">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="500d4-120">Listar respostas a um chat</span><span class="sxs-lookup"><span data-stu-id="500d4-120">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="500d4-121">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="500d4-121">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="500d4-122">Lista de todas as respostas para uma mensagem de chat no canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-122">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="500d4-123">Obter uma resposta para um chat</span><span class="sxs-lookup"><span data-stu-id="500d4-123">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="500d4-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="500d4-125">Obter uma única resposta para uma mensagem de chat em um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-125">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="500d4-126">Criar chat em um canal</span><span class="sxs-lookup"><span data-stu-id="500d4-126">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="500d4-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="500d4-128">Criar uma nova mensagem de chat de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-128">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="500d4-129">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="500d4-129">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="500d4-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="500d4-131">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-131">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="500d4-132">Criar chat em um chat</span><span class="sxs-lookup"><span data-stu-id="500d4-132">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="500d4-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-133">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="500d4-134">Envie uma mensagem de chat em uma conversa existente de chat de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="500d4-134">Send a chat message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="500d4-135">Listar chatMessages em um chat</span><span class="sxs-lookup"><span data-stu-id="500d4-135">List chatMessages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="500d4-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="500d4-137">Listar mensagens de chat em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="500d4-137">List chat messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="500d4-138">Obter chat no chat</span><span class="sxs-lookup"><span data-stu-id="500d4-138">Get chatMessage in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="500d4-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="500d4-139">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="500d4-140">Obter uma única mensagem de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-140">Get a single chat message in a chat.</span></span> |
|[<span data-ttu-id="500d4-141">Listar todas as imagens hospedadas</span><span class="sxs-lookup"><span data-stu-id="500d4-141">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="500d4-142">coleção [hostedImage](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="500d4-142">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="500d4-143">Obter todas as imagens hospedadas em uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-143">Get all hosted images in a chat message.</span></span>|
|[<span data-ttu-id="500d4-144">Obter imagem hospedada</span><span class="sxs-lookup"><span data-stu-id="500d4-144">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="500d4-145">hostedImage</span><span class="sxs-lookup"><span data-stu-id="500d4-145">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="500d4-146">Obter uma imagem hospedada de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-146">Get a hosted image from a chat message.</span></span>|
|[<span data-ttu-id="500d4-147">Obter bytes de imagem hospedado</span><span class="sxs-lookup"><span data-stu-id="500d4-147">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="500d4-148">dados de imagem binária</span><span class="sxs-lookup"><span data-stu-id="500d4-148">binary image data</span></span> | <span data-ttu-id="500d4-149">Obter dados de imagem binária de uma imagem hospedada de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-149">Get binary image data of a hosted image from a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="500d4-150">Propriedades</span><span class="sxs-lookup"><span data-stu-id="500d4-150">Properties</span></span>

| <span data-ttu-id="500d4-151">Propriedade</span><span class="sxs-lookup"><span data-stu-id="500d4-151">Property</span></span>   | <span data-ttu-id="500d4-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="500d4-152">Type</span></span> |<span data-ttu-id="500d4-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="500d4-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="500d4-154">id</span><span class="sxs-lookup"><span data-stu-id="500d4-154">id</span></span>|<span data-ttu-id="500d4-155">String</span><span class="sxs-lookup"><span data-stu-id="500d4-155">String</span></span>| <span data-ttu-id="500d4-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-156">Read-only.</span></span> <span data-ttu-id="500d4-157">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="500d4-157">Unique Id of the message.</span></span>|
|<span data-ttu-id="500d4-158">replyToId</span><span class="sxs-lookup"><span data-stu-id="500d4-158">replyToId</span></span>| <span data-ttu-id="500d4-159">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="500d4-159">string</span></span> | <span data-ttu-id="500d4-160">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-160">Read-only.</span></span> <span data-ttu-id="500d4-161">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="500d4-161">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="500d4-162">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="500d4-162">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="500d4-163">from</span><span class="sxs-lookup"><span data-stu-id="500d4-163">from</span></span>|[<span data-ttu-id="500d4-164">identitySet</span><span class="sxs-lookup"><span data-stu-id="500d4-164">identitySet</span></span>](identityset.md)| <span data-ttu-id="500d4-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-165">Read only.</span></span> <span data-ttu-id="500d4-166">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-166">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="500d4-167">etag</span><span class="sxs-lookup"><span data-stu-id="500d4-167">etag</span></span>| <span data-ttu-id="500d4-168">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="500d4-168">string</span></span> | <span data-ttu-id="500d4-169">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-169">Read-only.</span></span> <span data-ttu-id="500d4-170">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-170">Version number of the chat message.</span></span> |
|<span data-ttu-id="500d4-171">messageType</span><span class="sxs-lookup"><span data-stu-id="500d4-171">messageType</span></span>|<span data-ttu-id="500d4-172">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="500d4-172">chatMessageType</span></span>|<span data-ttu-id="500d4-173">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-173">The type of chat message.</span></span> <span data-ttu-id="500d4-174">Os valores possíveis são: `message`.</span><span class="sxs-lookup"><span data-stu-id="500d4-174">The possible values are: `message`.</span></span>|
|<span data-ttu-id="500d4-175">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="500d4-175">createdDateTime</span></span>|<span data-ttu-id="500d4-176">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="500d4-176">dateTimeOffset</span></span>|<span data-ttu-id="500d4-177">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-177">Read only.</span></span> <span data-ttu-id="500d4-178">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="500d4-178">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="500d4-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="500d4-179">lastModifiedDateTime</span></span>|<span data-ttu-id="500d4-180">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="500d4-180">dateTimeOffset</span></span>|<span data-ttu-id="500d4-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-181">Read only.</span></span> <span data-ttu-id="500d4-182">Carimbo de data/hora de quando a mensagem de chat é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem de chat raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="500d4-182">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="500d4-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="500d4-183">deletedDateTime</span></span>|<span data-ttu-id="500d4-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="500d4-184">dateTimeOffset</span></span>|<span data-ttu-id="500d4-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="500d4-185">Read only.</span></span> <span data-ttu-id="500d4-186">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="500d4-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="500d4-187">subject</span><span class="sxs-lookup"><span data-stu-id="500d4-187">subject</span></span>|<span data-ttu-id="500d4-188">string</span><span class="sxs-lookup"><span data-stu-id="500d4-188">string</span></span>| <span data-ttu-id="500d4-189">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="500d4-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="500d4-190">corpo</span><span class="sxs-lookup"><span data-stu-id="500d4-190">body</span></span>|[<span data-ttu-id="500d4-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="500d4-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="500d4-192">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="500d4-193">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="500d4-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="500d4-194">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="500d4-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="500d4-195">summary</span><span class="sxs-lookup"><span data-stu-id="500d4-195">summary</span></span>|<span data-ttu-id="500d4-196">string</span><span class="sxs-lookup"><span data-stu-id="500d4-196">string</span></span>| <span data-ttu-id="500d4-197">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="500d4-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="500d4-198">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="500d4-199">attachments</span><span class="sxs-lookup"><span data-stu-id="500d4-199">attachments</span></span>|<span data-ttu-id="500d4-200">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="500d4-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="500d4-201">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="500d4-201">Attached files.</span></span> <span data-ttu-id="500d4-202">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="500d4-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="500d4-203">mentions</span><span class="sxs-lookup"><span data-stu-id="500d4-203">mentions</span></span>|<span data-ttu-id="500d4-204">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="500d4-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="500d4-205">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="500d4-206">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="500d4-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="500d4-207">importância</span><span class="sxs-lookup"><span data-stu-id="500d4-207">importance</span></span>| <span data-ttu-id="500d4-208">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="500d4-208">chatMessageImportance</span></span> | <span data-ttu-id="500d4-209">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="500d4-209">The importance of the chat message.</span></span> <span data-ttu-id="500d4-210">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="500d4-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="500d4-211">reactions</span><span class="sxs-lookup"><span data-stu-id="500d4-211">reactions</span></span>| <span data-ttu-id="500d4-212">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="500d4-212">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="500d4-213">Reações para esta mensagem de chat (por exemplo, como).</span><span class="sxs-lookup"><span data-stu-id="500d4-213">Reactions for this chat message (for example, Like).</span></span>|
|<span data-ttu-id="500d4-214">localidade</span><span class="sxs-lookup"><span data-stu-id="500d4-214">locale</span></span>|<span data-ttu-id="500d4-215">string</span><span class="sxs-lookup"><span data-stu-id="500d4-215">string</span></span>|<span data-ttu-id="500d4-216">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="500d4-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="500d4-217">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="500d4-217">JSON representation</span></span>

<span data-ttu-id="500d4-218">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="500d4-218">The following is a JSON representation of the resource.</span></span>

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
