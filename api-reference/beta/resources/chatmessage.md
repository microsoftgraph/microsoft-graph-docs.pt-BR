---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: ea21d57134643c83406f449ee7cdad192afc0326
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709408"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="b109a-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="b109a-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b109a-105">Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).</span><span class="sxs-lookup"><span data-stu-id="b109a-105">Represents an individual chat message within a [channel](channel.md) or [chat](chat.md).</span></span>
<span data-ttu-id="b109a-106">A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-106">The message can be a root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="b109a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b109a-107">Methods</span></span>

| <span data-ttu-id="b109a-108">Método</span><span class="sxs-lookup"><span data-stu-id="b109a-108">Method</span></span>       | <span data-ttu-id="b109a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b109a-109">Return Type</span></span>  |<span data-ttu-id="b109a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b109a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b109a-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="b109a-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="b109a-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="b109a-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="b109a-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="b109a-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="b109a-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="b109a-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b109a-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="b109a-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="b109a-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="b109a-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="b109a-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="b109a-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="b109a-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="b109a-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="b109a-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="b109a-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b109a-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b109a-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="b109a-123">Criar uma chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="b109a-123">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="b109a-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b109a-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b109a-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="b109a-126">Criar uma resposta chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="b109a-126">Create chatMessage reply in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="b109a-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="b109a-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="b109a-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-128">Reply to an existing message in a channel.</span></span>|
|[<span data-ttu-id="b109a-129">Listar mensagens em um bate-papo</span><span class="sxs-lookup"><span data-stu-id="b109a-129">List messages in a chat</span></span>](../api/chat-list-messages.md)  | [<span data-ttu-id="b109a-130">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b109a-130">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b109a-131">Receba mensagens em um bate-papo de um para um ou de grupo.</span><span class="sxs-lookup"><span data-stu-id="b109a-131">Get messages in a 1:1 or group chat.</span></span> |
|[<span data-ttu-id="b109a-132">Receba uma mensagem no bate-papo</span><span class="sxs-lookup"><span data-stu-id="b109a-132">Get message in chat</span></span>](../api/chat-get-message.md)  | [<span data-ttu-id="b109a-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="b109a-133">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="b109a-134">Receba uma única mensagem em um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="b109a-134">Get a single message in a chat.</span></span> |

## <a name="properties"></a><span data-ttu-id="b109a-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b109a-135">Properties</span></span>

| <span data-ttu-id="b109a-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b109a-136">Property</span></span>   | <span data-ttu-id="b109a-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="b109a-137">Type</span></span> |<span data-ttu-id="b109a-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="b109a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b109a-139">id</span><span class="sxs-lookup"><span data-stu-id="b109a-139">id</span></span>|<span data-ttu-id="b109a-140">String</span><span class="sxs-lookup"><span data-stu-id="b109a-140">String</span></span>| <span data-ttu-id="b109a-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-141">Read-only.</span></span> <span data-ttu-id="b109a-142">ID exclusivo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-142">Unique ID of the message.</span></span>|
|<span data-ttu-id="b109a-143">replyToId</span><span class="sxs-lookup"><span data-stu-id="b109a-143">replyToId</span></span>| <span data-ttu-id="b109a-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b109a-144">string</span></span> | <span data-ttu-id="b109a-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-145">Read-only.</span></span> <span data-ttu-id="b109a-146">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="b109a-146">Id of the parent message/root message of the thread.</span></span> <span data-ttu-id="b109a-147">(Aplica-se apenas a mensagens em canais e não em bate-papos)</span><span class="sxs-lookup"><span data-stu-id="b109a-147">(Only applies to messages in channels not chats)</span></span> |
|<span data-ttu-id="b109a-148">from</span><span class="sxs-lookup"><span data-stu-id="b109a-148">from</span></span>|[<span data-ttu-id="b109a-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="b109a-149">identitySet</span></span>](identityset.md)| <span data-ttu-id="b109a-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-150">Read only.</span></span> <span data-ttu-id="b109a-151">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-151">Details of the sender of the message.</span></span>|
|<span data-ttu-id="b109a-152">etag</span><span class="sxs-lookup"><span data-stu-id="b109a-152">etag</span></span>| <span data-ttu-id="b109a-153">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b109a-153">string</span></span> | <span data-ttu-id="b109a-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-154">Read-only.</span></span> <span data-ttu-id="b109a-155">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-155">Version number of the message.</span></span> |
|<span data-ttu-id="b109a-156">messageType</span><span class="sxs-lookup"><span data-stu-id="b109a-156">messageType</span></span>|<span data-ttu-id="b109a-157">chatMessageType</span><span class="sxs-lookup"><span data-stu-id="b109a-157">chatMessageType</span></span>|<span data-ttu-id="b109a-158">O tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-158">The type of message.</span></span> <span data-ttu-id="b109a-159">Os valores possíveis são: `message`.</span><span class="sxs-lookup"><span data-stu-id="b109a-159">The possible values are: `message`, , .</span></span>|
|<span data-ttu-id="b109a-160">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b109a-160">createdDateTime</span></span>|<span data-ttu-id="b109a-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b109a-161">dateTimeOffset</span></span>|<span data-ttu-id="b109a-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-162">Read only.</span></span> <span data-ttu-id="b109a-163">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="b109a-163">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="b109a-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b109a-164">lastModifiedDateTime</span></span>|<span data-ttu-id="b109a-165">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b109a-165">dateTimeOffset</span></span>|<span data-ttu-id="b109a-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-166">Read only.</span></span> <span data-ttu-id="b109a-167">Carimbo de data/hora de quando a mensagem foi editada/atualizada.</span><span class="sxs-lookup"><span data-stu-id="b109a-167">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="b109a-168">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="b109a-168">deletedDateTime</span></span>|<span data-ttu-id="b109a-169">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b109a-169">dateTimeOffset</span></span>|<span data-ttu-id="b109a-170">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b109a-170">Read only.</span></span> <span data-ttu-id="b109a-171">Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="b109a-171">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="b109a-172">assunto</span><span class="sxs-lookup"><span data-stu-id="b109a-172">subject</span></span>|<span data-ttu-id="b109a-173">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b109a-173">string</span></span>| <span data-ttu-id="b109a-174">O assunto da mensagem, em texto simples.</span><span class="sxs-lookup"><span data-stu-id="b109a-174">The subject of the message, in plaintext.</span></span>|
|<span data-ttu-id="b109a-175">corpo</span><span class="sxs-lookup"><span data-stu-id="b109a-175">body</span></span>|[<span data-ttu-id="b109a-176">itemBody</span><span class="sxs-lookup"><span data-stu-id="b109a-176">itemBody</span></span>](itembody.md)|<span data-ttu-id="b109a-177">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-177">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="b109a-178">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="b109a-178">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="b109a-179">O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="b109a-179">The content is always in HTML if the message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="b109a-180">summary</span><span class="sxs-lookup"><span data-stu-id="b109a-180">summary</span></span>|<span data-ttu-id="b109a-181">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b109a-181">string</span></span>| <span data-ttu-id="b109a-182">Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback.</span><span class="sxs-lookup"><span data-stu-id="b109a-182">Summary text of the message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="b109a-183">Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo.</span><span class="sxs-lookup"><span data-stu-id="b109a-183">Only applies to channel messages, not chat messages.</span></span> |
|<span data-ttu-id="b109a-184">attachments</span><span class="sxs-lookup"><span data-stu-id="b109a-184">attachments</span></span>|<span data-ttu-id="b109a-185">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="b109a-185">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="b109a-186">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="b109a-186">Attached files.</span></span> <span data-ttu-id="b109a-187">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="b109a-187">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="b109a-188">mentions</span><span class="sxs-lookup"><span data-stu-id="b109a-188">mentions</span></span>|<span data-ttu-id="b109a-189">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="b109a-189">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="b109a-190">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-190">List of entities mentioned in the message.</span></span> <span data-ttu-id="b109a-191">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="b109a-191">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="b109a-192">importância</span><span class="sxs-lookup"><span data-stu-id="b109a-192">importance</span></span>| <span data-ttu-id="b109a-193">chatMessageImportance</span><span class="sxs-lookup"><span data-stu-id="b109a-193">chatMessageImportance</span></span> | <span data-ttu-id="b109a-194">A importância da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b109a-194">The importance of the message.</span></span> <span data-ttu-id="b109a-195">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="b109a-195">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="b109a-196">reactions</span><span class="sxs-lookup"><span data-stu-id="b109a-196">reactions</span></span>| <span data-ttu-id="b109a-197">[chatMessageReaction](chatmessagereaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="b109a-197">[chatMessageReaction](chatmessagereaction.md) collection</span></span> | <span data-ttu-id="b109a-198">Reações para esta mensagem (por exemplo, Curtir).</span><span class="sxs-lookup"><span data-stu-id="b109a-198">Reactions for this message (for example, Like).</span></span>|
|<span data-ttu-id="b109a-199">localidade</span><span class="sxs-lookup"><span data-stu-id="b109a-199">locale</span></span>|<span data-ttu-id="b109a-200">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b109a-200">string</span></span>|<span data-ttu-id="b109a-201">Local da mensagem definido pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b109a-201">Locale of the message set by the client.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b109a-202">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b109a-202">JSON representation</span></span>

<span data-ttu-id="b109a-203">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b109a-203">The following is a JSON representation of the resource.</span></span>

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
