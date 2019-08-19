---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
doc_type: resourcePageType
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 17b6912312c66bca8b84ccce9d25ac3c83a2edf9
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36460763"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="50ad7-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50ad7-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="50ad7-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="50ad7-106">A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="50ad7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="50ad7-107">Methods</span></span>

| <span data-ttu-id="50ad7-108">Método</span><span class="sxs-lookup"><span data-stu-id="50ad7-108">Method</span></span>       | <span data-ttu-id="50ad7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50ad7-109">Return Type</span></span>  |<span data-ttu-id="50ad7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50ad7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50ad7-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="50ad7-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="50ad7-112">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="50ad7-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="50ad7-113">Lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="50ad7-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="50ad7-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="50ad7-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="50ad7-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="50ad7-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="50ad7-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="50ad7-118">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="50ad7-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="50ad7-119">Lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="50ad7-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="50ad7-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="50ad7-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50ad7-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="50ad7-123">Criar chat em um canal</span><span class="sxs-lookup"><span data-stu-id="50ad7-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="50ad7-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50ad7-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="50ad7-126">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="50ad7-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="50ad7-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50ad7-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="50ad7-129">Criar chat em um chat</span><span class="sxs-lookup"><span data-stu-id="50ad7-129">Create chatMessage in a chat</span></span>](../api/chat-post-messages.md) | [<span data-ttu-id="50ad7-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-130">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="50ad7-131">Envie uma mensagem em uma conversa existente de chat de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="50ad7-131">Send a message in an existing 1:1 or group chat conversation.</span></span>|
|[<span data-ttu-id="50ad7-132">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="50ad7-132">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="50ad7-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="50ad7-134">Listar mensagens em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="50ad7-134">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="50ad7-135">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="50ad7-135">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="50ad7-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="50ad7-136">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="50ad7-137">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="50ad7-137">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="50ad7-138">Listar todas as imagens hospedadas</span><span class="sxs-lookup"><span data-stu-id="50ad7-138">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="50ad7-139">coleção [hostedImage](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="50ad7-139">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="50ad7-140">Obter todas as imagens hospedadas em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-140">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="50ad7-141">Obter imagem hospedada</span><span class="sxs-lookup"><span data-stu-id="50ad7-141">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="50ad7-142">hostedImage</span><span class="sxs-lookup"><span data-stu-id="50ad7-142">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="50ad7-143">Obter uma imagem hospedada de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-143">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="50ad7-144">Obter bytes de imagem hospedado</span><span class="sxs-lookup"><span data-stu-id="50ad7-144">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="50ad7-145">dados de imagem binária</span><span class="sxs-lookup"><span data-stu-id="50ad7-145">binary image data</span></span> | <span data-ttu-id="50ad7-146">Obtém dados de imagem binária de uma imagem hospedada de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-146">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="50ad7-147">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50ad7-147">Properties</span></span>

| <span data-ttu-id="50ad7-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50ad7-148">Property</span></span>   | <span data-ttu-id="50ad7-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="50ad7-149">Type</span></span> |<span data-ttu-id="50ad7-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="50ad7-150">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50ad7-151">id</span><span class="sxs-lookup"><span data-stu-id="50ad7-151">id</span></span>|<span data-ttu-id="50ad7-152">String</span><span class="sxs-lookup"><span data-stu-id="50ad7-152">String</span></span>| <span data-ttu-id="50ad7-153">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-153">Read-only.</span></span> <span data-ttu-id="50ad7-154">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-154">Unique Id of the message.</span></span>|
|<span data-ttu-id="50ad7-155">replyToId</span><span class="sxs-lookup"><span data-stu-id="50ad7-155">replyToId</span></span>| <span data-ttu-id="50ad7-156">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ad7-156">string</span></span> | <span data-ttu-id="50ad7-157">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-157">Read-only.</span></span> <span data-ttu-id="50ad7-158">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="50ad7-158">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="50ad7-159">(Aplica-se apenas a mensagens em canais e não em bate-papos)</span><span class="sxs-lookup"><span data-stu-id="50ad7-159">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="50ad7-160">from</span><span class="sxs-lookup"><span data-stu-id="50ad7-160">from</span></span>|[<span data-ttu-id="50ad7-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="50ad7-161">identitySet</span></span>](identityset.md)| <span data-ttu-id="50ad7-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-162">Read only.</span></span> <span data-ttu-id="50ad7-163">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-163">Details of the sender of the message.</span></span>|
|<span data-ttu-id="50ad7-164">etag</span><span class="sxs-lookup"><span data-stu-id="50ad7-164">etag</span></span>| <span data-ttu-id="50ad7-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ad7-165">string</span></span> | <span data-ttu-id="50ad7-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-166">Read-only.</span></span> <span data-ttu-id="50ad7-167">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-167">Version number of the message.</span></span> |
|<span data-ttu-id="50ad7-168">messageType</span><span class="sxs-lookup"><span data-stu-id="50ad7-168">messageType</span></span>|<span data-ttu-id="50ad7-169">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="50ad7-169">chatMessageType</span></span>|<span data-ttu-id="50ad7-170">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-170">The type of message.</span></span> <span data-ttu-id="50ad7-171">Os valores possíveis são: `message`.</span><span class="sxs-lookup"><span data-stu-id="50ad7-171">The possible values are: `message`.</span></span>|
|<span data-ttu-id="50ad7-172">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50ad7-172">createdDateTime</span></span>|<span data-ttu-id="50ad7-173">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ad7-173">dateTimeOffset</span></span>|<span data-ttu-id="50ad7-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-174">Read only.</span></span> <span data-ttu-id="50ad7-175">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="50ad7-175">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="50ad7-176">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50ad7-176">lastModifiedDateTime</span></span>|<span data-ttu-id="50ad7-177">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ad7-177">dateTimeOffset</span></span>|<span data-ttu-id="50ad7-178">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-178">Read only.</span></span> <span data-ttu-id="50ad7-179">Carimbo de data/hora de quando a mensagem é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="50ad7-179">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="50ad7-180">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="50ad7-180">deletedDateTime</span></span>|<span data-ttu-id="50ad7-181">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ad7-181">dateTimeOffset</span></span>|<span data-ttu-id="50ad7-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50ad7-182">Read only.</span></span> <span data-ttu-id="50ad7-183">Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="50ad7-183">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="50ad7-184">assunto</span><span class="sxs-lookup"><span data-stu-id="50ad7-184">subject</span></span>|<span data-ttu-id="50ad7-185">string</span><span class="sxs-lookup"><span data-stu-id="50ad7-185">string</span></span>| <span data-ttu-id="50ad7-186">O assunto da mensagem, em texto simples.</span><span class="sxs-lookup"><span data-stu-id="50ad7-186">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="50ad7-187">corpo</span><span class="sxs-lookup"><span data-stu-id="50ad7-187">body</span></span>|[<span data-ttu-id="50ad7-188">itemBody</span><span class="sxs-lookup"><span data-stu-id="50ad7-188">itemBody</span></span>](itembody.md)|<span data-ttu-id="50ad7-189">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-189">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="50ad7-190">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="50ad7-190">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="50ad7-191">O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="50ad7-191">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="50ad7-192">summary</span><span class="sxs-lookup"><span data-stu-id="50ad7-192">summary</span></span>|<span data-ttu-id="50ad7-193">string</span><span class="sxs-lookup"><span data-stu-id="50ad7-193">string</span></span>| <span data-ttu-id="50ad7-194">Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback.</span><span class="sxs-lookup"><span data-stu-id="50ad7-194">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="50ad7-195">Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo.</span><span class="sxs-lookup"><span data-stu-id="50ad7-195">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="50ad7-196">attachments</span><span class="sxs-lookup"><span data-stu-id="50ad7-196">attachments</span></span>|<span data-ttu-id="50ad7-197">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="50ad7-197">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="50ad7-198">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="50ad7-198">Attached files.</span></span> <span data-ttu-id="50ad7-199">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="50ad7-199">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="50ad7-200">mentions</span><span class="sxs-lookup"><span data-stu-id="50ad7-200">mentions</span></span>|<span data-ttu-id="50ad7-201">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="50ad7-201">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="50ad7-202">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-202">List of entities mentioned in the message.</span></span> <span data-ttu-id="50ad7-203">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="50ad7-203">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="50ad7-204">importância</span><span class="sxs-lookup"><span data-stu-id="50ad7-204">importance</span></span>| <span data-ttu-id="50ad7-205">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="50ad7-205">chatMessageImportance</span></span> | <span data-ttu-id="50ad7-206">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="50ad7-206">The importance of the message.</span></span> <span data-ttu-id="50ad7-207">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="50ad7-207">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="50ad7-208">reactions</span><span class="sxs-lookup"><span data-stu-id="50ad7-208">reactions</span></span>| <span data-ttu-id="50ad7-209">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="50ad7-209">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="50ad7-210">Reações para esta mensagem (por exemplo, Curtir).</span><span class="sxs-lookup"><span data-stu-id="50ad7-210">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="50ad7-211">localidade</span><span class="sxs-lookup"><span data-stu-id="50ad7-211">locale</span></span>|<span data-ttu-id="50ad7-212">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50ad7-212">string</span></span>|<span data-ttu-id="50ad7-213">Local da mensagem definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="50ad7-213">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50ad7-214">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50ad7-214">JSON representation</span></span>

<span data-ttu-id="50ad7-215">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50ad7-215">The following is a JSON representation of the resource.</span></span>

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
