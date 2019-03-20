---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644318"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c239a-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="c239a-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c239a-105">Representa uma mensagem de chat individual dentro de uma entidade de [canal](channel.md) ou chat.</span><span class="sxs-lookup"><span data-stu-id="c239a-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="c239a-106">A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="c239a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="c239a-107">Methods</span></span>

| <span data-ttu-id="c239a-108">Método</span><span class="sxs-lookup"><span data-stu-id="c239a-108">Method</span></span>       | <span data-ttu-id="c239a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c239a-109">Return Type</span></span>  |<span data-ttu-id="c239a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c239a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c239a-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="c239a-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c239a-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="c239a-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c239a-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="c239a-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="c239a-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c239a-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c239a-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="c239a-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="c239a-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="c239a-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c239a-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="c239a-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c239a-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="c239a-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="c239a-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c239a-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c239a-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c239a-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="c239a-123">Enviar uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="c239a-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="c239a-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c239a-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c239a-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="c239a-126">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="c239a-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c239a-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="c239a-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="c239a-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="c239a-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c239a-129">Properties</span></span>
| <span data-ttu-id="c239a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c239a-130">Property</span></span>     | <span data-ttu-id="c239a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c239a-131">Type</span></span>   |<span data-ttu-id="c239a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c239a-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c239a-133">id</span><span class="sxs-lookup"><span data-stu-id="c239a-133">id</span></span>|<span data-ttu-id="c239a-134">String</span><span class="sxs-lookup"><span data-stu-id="c239a-134">String</span></span>| <span data-ttu-id="c239a-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c239a-135">Read-only.</span></span> <span data-ttu-id="c239a-136">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="c239a-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="c239a-137">replyToId</span></span>| <span data-ttu-id="c239a-138">string</span><span class="sxs-lookup"><span data-stu-id="c239a-138">string</span></span> | <span data-ttu-id="c239a-139">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="c239a-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="c239a-140">from</span><span class="sxs-lookup"><span data-stu-id="c239a-140">from</span></span>|[<span data-ttu-id="c239a-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="c239a-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="c239a-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c239a-142">Read only.</span></span> <span data-ttu-id="c239a-143">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-143">Details of the sender of the message</span></span>|
|<span data-ttu-id="c239a-144">etag</span><span class="sxs-lookup"><span data-stu-id="c239a-144">etag</span></span>| <span data-ttu-id="c239a-145">string</span><span class="sxs-lookup"><span data-stu-id="c239a-145">string</span></span> | <span data-ttu-id="c239a-146">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-146">Version number of the message</span></span> |
|<span data-ttu-id="c239a-147">messageType</span><span class="sxs-lookup"><span data-stu-id="c239a-147">messageType</span></span>|<span data-ttu-id="c239a-148">String</span><span class="sxs-lookup"><span data-stu-id="c239a-148">String</span></span>|<span data-ttu-id="c239a-149">Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="c239a-149">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="c239a-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c239a-150">createdDateTime</span></span>|<span data-ttu-id="c239a-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c239a-151">dateTimeOffset</span></span>|<span data-ttu-id="c239a-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c239a-152">Read only.</span></span> <span data-ttu-id="c239a-153">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="c239a-153">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="c239a-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c239a-154">lastModifiedDateTime</span></span>|<span data-ttu-id="c239a-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c239a-155">dateTimeOffset</span></span>|<span data-ttu-id="c239a-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c239a-156">Read only.</span></span> <span data-ttu-id="c239a-157">Carimbo de data/hora de quando a mensagem foi editada/atualizada.</span><span class="sxs-lookup"><span data-stu-id="c239a-157">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="c239a-158">deleted</span><span class="sxs-lookup"><span data-stu-id="c239a-158">deleted</span></span>|<span data-ttu-id="c239a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="c239a-159">Boolean</span></span>|<span data-ttu-id="c239a-160">Indica se uma mensagem foi excluída de modo reversível.</span><span class="sxs-lookup"><span data-stu-id="c239a-160">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="c239a-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c239a-161">deletedDateTime</span></span>|<span data-ttu-id="c239a-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c239a-162">dateTimeOffset</span></span>|<span data-ttu-id="c239a-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c239a-163">Read only.</span></span> <span data-ttu-id="c239a-164">Carimbo de data/hora em que a mensagem foi excluída.</span><span class="sxs-lookup"><span data-stu-id="c239a-164">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="c239a-165">Assunto</span><span class="sxs-lookup"><span data-stu-id="c239a-165">subject</span></span>|<span data-ttu-id="c239a-166">string</span><span class="sxs-lookup"><span data-stu-id="c239a-166">string</span></span>|<span data-ttu-id="c239a-167">Linha de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-167">Message subject line.</span></span> <span data-ttu-id="c239a-168">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c239a-168">Optional.</span></span>|
|<span data-ttu-id="c239a-169">corpo</span><span class="sxs-lookup"><span data-stu-id="c239a-169">body</span></span>|[<span data-ttu-id="c239a-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="c239a-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="c239a-171">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-171">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="c239a-172">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="c239a-172">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="c239a-173">summary</span><span class="sxs-lookup"><span data-stu-id="c239a-173">summary</span></span>|<span data-ttu-id="c239a-174">string</span><span class="sxs-lookup"><span data-stu-id="c239a-174">string</span></span>|<span data-ttu-id="c239a-175">Texto de resumo da mensagem que poderia ser usado para notificações por push e modos de exibição de resumo ou de fallback</span><span class="sxs-lookup"><span data-stu-id="c239a-175">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="c239a-176">mentions</span><span class="sxs-lookup"><span data-stu-id="c239a-176">mentions</span></span>|<span data-ttu-id="c239a-177">[chatMessageMention](chatmention.md) collection</span><span class="sxs-lookup"><span data-stu-id="c239a-177">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="c239a-178">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="c239a-178">List of entities mentioned in the message.</span></span> <span data-ttu-id="c239a-179">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="c239a-179">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="c239a-180">importância</span><span class="sxs-lookup"><span data-stu-id="c239a-180">importance</span></span>| <span data-ttu-id="c239a-181">string</span><span class="sxs-lookup"><span data-stu-id="c239a-181">string</span></span> | <span data-ttu-id="c239a-182">A importância da mensagem: Normal, Alta.</span><span class="sxs-lookup"><span data-stu-id="c239a-182">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="c239a-183">reactions</span><span class="sxs-lookup"><span data-stu-id="c239a-183">reactions</span></span>| <span data-ttu-id="c239a-184">[chatMessageReaction](chatreaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="c239a-184">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="c239a-185">Reações para essa mensagem (por exemplo, Curtir)</span><span class="sxs-lookup"><span data-stu-id="c239a-185">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="c239a-186">locale</span><span class="sxs-lookup"><span data-stu-id="c239a-186">locale</span></span>|<span data-ttu-id="c239a-187">string</span><span class="sxs-lookup"><span data-stu-id="c239a-187">string</span></span>|<span data-ttu-id="c239a-188">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="c239a-188">Locale of the message set by the client</span></span>|
|<span data-ttu-id="c239a-189">attachments</span><span class="sxs-lookup"><span data-stu-id="c239a-189">attachments</span></span>|<span data-ttu-id="c239a-190">[chatMessageAttachment](chatattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c239a-190">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="c239a-191">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="c239a-191">Attached files</span></span> <span data-ttu-id="c239a-192">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="c239a-192">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c239a-193">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c239a-193">JSON representation</span></span>

<span data-ttu-id="c239a-194">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c239a-194">The following is a JSON representation of the resource.</span></span>

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
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
