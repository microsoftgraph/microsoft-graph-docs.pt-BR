---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 99e69bd51a661b67fd4cb325fffe80db91214714
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778667"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="dd09c-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd09c-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="dd09c-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="dd09c-106">A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="dd09c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd09c-107">Methods</span></span>

| <span data-ttu-id="dd09c-108">Método</span><span class="sxs-lookup"><span data-stu-id="dd09c-108">Method</span></span>       | <span data-ttu-id="dd09c-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd09c-109">Return Type</span></span>  |<span data-ttu-id="dd09c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd09c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd09c-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="dd09c-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="dd09c-112">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd09c-112">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="dd09c-113">Lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-113">List of all root messages in a channel.</span></span>|
|[<span data-ttu-id="dd09c-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="dd09c-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="dd09c-115">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-115">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="dd09c-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="dd09c-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="dd09c-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="dd09c-118">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd09c-118">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="dd09c-119">Lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-119">List of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="dd09c-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="dd09c-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="dd09c-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-121">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="dd09c-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="dd09c-123">Criar chat em um canal</span><span class="sxs-lookup"><span data-stu-id="dd09c-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="dd09c-124">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-124">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="dd09c-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="dd09c-126">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="dd09c-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="dd09c-127">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-127">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="dd09c-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="dd09c-129">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="dd09c-129">List messages in a chat</span></span>](../api/chatmessage-list.md)  | [<span data-ttu-id="dd09c-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="dd09c-131">Listar mensagens em um bate-papo de grupo ou 1:1.</span><span class="sxs-lookup"><span data-stu-id="dd09c-131">List messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="dd09c-132">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="dd09c-132">Get message in chat</span></span>](../api/chatmessage-get.md)  | [<span data-ttu-id="dd09c-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="dd09c-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="dd09c-134">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="dd09c-134">Get a single message in a chat.</span></span> |
|[<span data-ttu-id="dd09c-135">Listar todas as imagens hospedadas</span><span class="sxs-lookup"><span data-stu-id="dd09c-135">List all hosted images</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="dd09c-136">coleção [hostedImage](../resources/chatmessagehostedimage.md)</span><span class="sxs-lookup"><span data-stu-id="dd09c-136">[hostedImage](../resources/chatmessagehostedimage.md) collection</span></span>| <span data-ttu-id="dd09c-137">Obter todas as imagens hospedadas em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-137">Get all hosted images in a message.</span></span>|
|[<span data-ttu-id="dd09c-138">Obter imagem hospedada</span><span class="sxs-lookup"><span data-stu-id="dd09c-138">Get hosted image</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="dd09c-139">hostedImage</span><span class="sxs-lookup"><span data-stu-id="dd09c-139">hostedImage</span></span>](../resources/chatmessagehostedimage.md) | <span data-ttu-id="dd09c-140">Obter uma imagem hospedada de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-140">Get a hosted image from a message.</span></span>|
|[<span data-ttu-id="dd09c-141">Obter bytes de imagem hospedado</span><span class="sxs-lookup"><span data-stu-id="dd09c-141">Get hosted image bytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="dd09c-142">dados de imagem binária</span><span class="sxs-lookup"><span data-stu-id="dd09c-142">binary image data</span></span> | <span data-ttu-id="dd09c-143">Obtém dados de imagem binária de uma imagem hospedada de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-143">Get binary image data of a hosted image from a message.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd09c-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd09c-144">Properties</span></span>

| <span data-ttu-id="dd09c-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd09c-145">Property</span></span>   | <span data-ttu-id="dd09c-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd09c-146">Type</span></span> |<span data-ttu-id="dd09c-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd09c-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd09c-148">id</span><span class="sxs-lookup"><span data-stu-id="dd09c-148">id</span></span>|<span data-ttu-id="dd09c-149">String</span><span class="sxs-lookup"><span data-stu-id="dd09c-149">String</span></span>| <span data-ttu-id="dd09c-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-150">Read-only.</span></span> <span data-ttu-id="dd09c-151">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="dd09c-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="dd09c-152">replyToId</span></span>| <span data-ttu-id="dd09c-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd09c-153">string</span></span> | <span data-ttu-id="dd09c-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-154">Read-only.</span></span> <span data-ttu-id="dd09c-155">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="dd09c-155">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="dd09c-156">(Aplica-se apenas a mensagens em canais e não em bate-papos)</span><span class="sxs-lookup"><span data-stu-id="dd09c-156">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="dd09c-157">from</span><span class="sxs-lookup"><span data-stu-id="dd09c-157">from</span></span>|[<span data-ttu-id="dd09c-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="dd09c-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="dd09c-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-159">Read only.</span></span> <span data-ttu-id="dd09c-160">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-160">Details of the sender of the message.</span></span>|
|<span data-ttu-id="dd09c-161">etag</span><span class="sxs-lookup"><span data-stu-id="dd09c-161">etag</span></span>| <span data-ttu-id="dd09c-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd09c-162">string</span></span> | <span data-ttu-id="dd09c-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-163">Read-only.</span></span> <span data-ttu-id="dd09c-164">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-164">Version number of the message.</span></span> |
|<span data-ttu-id="dd09c-165">messageType</span><span class="sxs-lookup"><span data-stu-id="dd09c-165">messageType</span></span>|<span data-ttu-id="dd09c-166">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="dd09c-166">chatMessageType</span></span>|<span data-ttu-id="dd09c-167">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-167">The type of message.</span></span> <span data-ttu-id="dd09c-168">Os valores possíveis são: `message`.</span><span class="sxs-lookup"><span data-stu-id="dd09c-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="dd09c-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd09c-169">createdDateTime</span></span>|<span data-ttu-id="dd09c-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd09c-170">dateTimeOffset</span></span>|<span data-ttu-id="dd09c-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-171">Read only.</span></span> <span data-ttu-id="dd09c-172">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="dd09c-172">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="dd09c-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd09c-173">lastModifiedDateTime</span></span>|<span data-ttu-id="dd09c-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd09c-174">dateTimeOffset</span></span>|<span data-ttu-id="dd09c-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-175">Read only.</span></span> <span data-ttu-id="dd09c-176">Carimbo de data/hora de quando a mensagem é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="dd09c-176">Timestamp of when the message is created or edited, including when a reply is made (if it's a root message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="dd09c-177">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd09c-177">deletedDateTime</span></span>|<span data-ttu-id="dd09c-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd09c-178">dateTimeOffset</span></span>|<span data-ttu-id="dd09c-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd09c-179">Read only.</span></span> <span data-ttu-id="dd09c-180">Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="dd09c-180">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="dd09c-181">assunto</span><span class="sxs-lookup"><span data-stu-id="dd09c-181">subject</span></span>|<span data-ttu-id="dd09c-182">string</span><span class="sxs-lookup"><span data-stu-id="dd09c-182">string</span></span>| <span data-ttu-id="dd09c-183">O assunto da mensagem, em texto simples.</span><span class="sxs-lookup"><span data-stu-id="dd09c-183">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="dd09c-184">corpo</span><span class="sxs-lookup"><span data-stu-id="dd09c-184">body</span></span>|[<span data-ttu-id="dd09c-185">itemBody</span><span class="sxs-lookup"><span data-stu-id="dd09c-185">itemBody</span></span>](itembody.md)|<span data-ttu-id="dd09c-186">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-186">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="dd09c-187">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="dd09c-187">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="dd09c-188">O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="dd09c-188">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="dd09c-189">summary</span><span class="sxs-lookup"><span data-stu-id="dd09c-189">summary</span></span>|<span data-ttu-id="dd09c-190">string</span><span class="sxs-lookup"><span data-stu-id="dd09c-190">string</span></span>| <span data-ttu-id="dd09c-191">Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback.</span><span class="sxs-lookup"><span data-stu-id="dd09c-191">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="dd09c-192">Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo.</span><span class="sxs-lookup"><span data-stu-id="dd09c-192">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="dd09c-193">attachments</span><span class="sxs-lookup"><span data-stu-id="dd09c-193">attachments</span></span>|<span data-ttu-id="dd09c-194">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd09c-194">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="dd09c-195">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="dd09c-195">Attached files.</span></span> <span data-ttu-id="dd09c-196">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="dd09c-196">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="dd09c-197">mentions</span><span class="sxs-lookup"><span data-stu-id="dd09c-197">mentions</span></span>|<span data-ttu-id="dd09c-198">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd09c-198">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="dd09c-199">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-199">List of entities mentioned in the message.</span></span> <span data-ttu-id="dd09c-200">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="dd09c-200">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="dd09c-201">importância</span><span class="sxs-lookup"><span data-stu-id="dd09c-201">importance</span></span>| <span data-ttu-id="dd09c-202">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="dd09c-202">chatMessageImportance</span></span> | <span data-ttu-id="dd09c-203">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="dd09c-203">The importance of the message.</span></span> <span data-ttu-id="dd09c-204">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="dd09c-204">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="dd09c-205">reactions</span><span class="sxs-lookup"><span data-stu-id="dd09c-205">reactions</span></span>| <span data-ttu-id="dd09c-206">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd09c-206">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="dd09c-207">Reações para esta mensagem (por exemplo, Curtir).</span><span class="sxs-lookup"><span data-stu-id="dd09c-207">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="dd09c-208">localidade</span><span class="sxs-lookup"><span data-stu-id="dd09c-208">locale</span></span>|<span data-ttu-id="dd09c-209">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd09c-209">string</span></span>|<span data-ttu-id="dd09c-210">Local da mensagem definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd09c-210">Locale of the message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd09c-211">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd09c-211">JSON representation</span></span>

<span data-ttu-id="dd09c-212">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd09c-212">The following is a JSON representation of the resource.</span></span>

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
