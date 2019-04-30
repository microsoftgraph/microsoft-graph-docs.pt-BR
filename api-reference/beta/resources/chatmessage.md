---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 4c2631d0ba4883160c443000fa2ecb0e1853523d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339837"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="2a4e7-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a4e7-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="2a4e7-105">Represents an individual chat message within a channel or chat entity.</span></span> <span data-ttu-id="2a4e7-106">A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="2a4e7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a4e7-107">Methods</span></span>

| <span data-ttu-id="2a4e7-108">Método</span><span class="sxs-lookup"><span data-stu-id="2a4e7-108">Method</span></span>       | <span data-ttu-id="2a4e7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a4e7-109">Return Type</span></span>  |<span data-ttu-id="2a4e7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4e7-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a4e7-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="2a4e7-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="2a4e7-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="2a4e7-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="2a4e7-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="2a4e7-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="2a4e7-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="2a4e7-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="2a4e7-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="2a4e7-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="2a4e7-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="2a4e7-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="2a4e7-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="2a4e7-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="2a4e7-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="2a4e7-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="2a4e7-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="2a4e7-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="2a4e7-123">Enviar uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="2a4e7-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="2a4e7-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="2a4e7-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="2a4e7-126">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="2a4e7-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="2a4e7-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="2a4e7-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="2a4e7-129">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="2a4e7-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="2a4e7-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2a4e7-131">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="2a4e7-132">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="2a4e7-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="2a4e7-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2a4e7-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="2a4e7-134">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-134">Get a single reply to a message in a channel.</span></span> |


## <a name="properties"></a><span data-ttu-id="2a4e7-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a4e7-135">Properties</span></span>
| <span data-ttu-id="2a4e7-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a4e7-136">Property</span></span>     | <span data-ttu-id="2a4e7-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a4e7-137">Type</span></span>   |<span data-ttu-id="2a4e7-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4e7-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a4e7-139">id</span><span class="sxs-lookup"><span data-stu-id="2a4e7-139">id</span></span>|<span data-ttu-id="2a4e7-140">String</span><span class="sxs-lookup"><span data-stu-id="2a4e7-140">String</span></span>| <span data-ttu-id="2a4e7-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-141">Read-only.</span></span> <span data-ttu-id="2a4e7-142">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="2a4e7-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="2a4e7-143">replyToId</span></span>| <span data-ttu-id="2a4e7-144">string</span><span class="sxs-lookup"><span data-stu-id="2a4e7-144">string</span></span> | <span data-ttu-id="2a4e7-145">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-145">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="2a4e7-146">(Aplica-se apenas a mensagens em canais e não em bate-papos)</span><span class="sxs-lookup"><span data-stu-id="2a4e7-146">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="2a4e7-147">from</span><span class="sxs-lookup"><span data-stu-id="2a4e7-147">from</span></span>|[<span data-ttu-id="2a4e7-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="2a4e7-148">identitySet</span></span>](identityset.md)| <span data-ttu-id="2a4e7-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-149">Read only.</span></span> <span data-ttu-id="2a4e7-150">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-150">Details of the sender of the message.</span></span>|
|<span data-ttu-id="2a4e7-151">etag</span><span class="sxs-lookup"><span data-stu-id="2a4e7-151">etag</span></span>| <span data-ttu-id="2a4e7-152">string</span><span class="sxs-lookup"><span data-stu-id="2a4e7-152">string</span></span> | <span data-ttu-id="2a4e7-153">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-153">Version number of the message.</span></span> |
|<span data-ttu-id="2a4e7-154">messageType</span><span class="sxs-lookup"><span data-stu-id="2a4e7-154">messageType</span></span>|<span data-ttu-id="2a4e7-155">String</span><span class="sxs-lookup"><span data-stu-id="2a4e7-155">String</span></span>|<span data-ttu-id="2a4e7-156">Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-156">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="2a4e7-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4e7-157">createdDateTime</span></span>|<span data-ttu-id="2a4e7-158">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4e7-158">dateTimeOffset</span></span>|<span data-ttu-id="2a4e7-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-159">Read only.</span></span> <span data-ttu-id="2a4e7-160">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-160">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="2a4e7-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4e7-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2a4e7-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4e7-162">dateTimeOffset</span></span>|<span data-ttu-id="2a4e7-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-163">Read only.</span></span> <span data-ttu-id="2a4e7-164">Carimbo de data/hora de quando a mensagem foi editada/atualizada.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-164">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="2a4e7-165">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a4e7-165">deletedDateTime</span></span>|<span data-ttu-id="2a4e7-166">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a4e7-166">dateTimeOffset</span></span>|<span data-ttu-id="2a4e7-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-167">Read only.</span></span> <span data-ttu-id="2a4e7-168">Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-168">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="2a4e7-169">assunto</span><span class="sxs-lookup"><span data-stu-id="2a4e7-169">subject</span></span>|<span data-ttu-id="2a4e7-170">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a4e7-170">string</span></span>| <span data-ttu-id="2a4e7-171">O assunto da mensagem, em texto simples.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-171">The subject of the message.</span></span>|
|<span data-ttu-id="2a4e7-172">corpo</span><span class="sxs-lookup"><span data-stu-id="2a4e7-172">body</span></span>|[<span data-ttu-id="2a4e7-173">itemBody</span><span class="sxs-lookup"><span data-stu-id="2a4e7-173">itemBody</span></span>](itembody.md)|<span data-ttu-id="2a4e7-174">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-174">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="2a4e7-175">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-175">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="2a4e7-176">O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="2a4e7-176">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="2a4e7-177">summary</span><span class="sxs-lookup"><span data-stu-id="2a4e7-177">summary</span></span>|<span data-ttu-id="2a4e7-178">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a4e7-178">string</span></span>| <span data-ttu-id="2a4e7-179">Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-179">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span> <span data-ttu-id="2a4e7-180">Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-180">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="2a4e7-181">attachments</span><span class="sxs-lookup"><span data-stu-id="2a4e7-181">attachments</span></span>|<span data-ttu-id="2a4e7-182">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="2a4e7-182">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="2a4e7-183">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-183">Attached files.</span></span> <span data-ttu-id="2a4e7-184">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-184">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="2a4e7-185">mentions</span><span class="sxs-lookup"><span data-stu-id="2a4e7-185">mentions</span></span>|<span data-ttu-id="2a4e7-186">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="2a4e7-186">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="2a4e7-187">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-187">List of entities mentioned in the message.</span></span> <span data-ttu-id="2a4e7-188">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-188">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="2a4e7-189">importância</span><span class="sxs-lookup"><span data-stu-id="2a4e7-189">importance</span></span>| <span data-ttu-id="2a4e7-190">string</span><span class="sxs-lookup"><span data-stu-id="2a4e7-190">string</span></span> | <span data-ttu-id="2a4e7-191">A importância da mensagem: Normal, Alta.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-191">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="2a4e7-192">reactions</span><span class="sxs-lookup"><span data-stu-id="2a4e7-192">reactions</span></span>| <span data-ttu-id="2a4e7-193">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="2a4e7-193">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="2a4e7-194">Reações para esta mensagem (por exemplo, Curtir).</span><span class="sxs-lookup"><span data-stu-id="2a4e7-194">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="2a4e7-195">localidade</span><span class="sxs-lookup"><span data-stu-id="2a4e7-195">locale</span></span>|<span data-ttu-id="2a4e7-196">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a4e7-196">string</span></span>|<span data-ttu-id="2a4e7-197">Local da mensagem definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-197">Locale of the message set by the client</span></span>|


## <a name="json-representation"></a><span data-ttu-id="2a4e7-198">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a4e7-198">JSON representation</span></span>

<span data-ttu-id="2a4e7-199">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a4e7-199">The following is a JSON representation of the resource.</span></span>

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
