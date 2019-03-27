---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: 1f1e38e53a7c7ad1b0452c9facc6d7f97314094e
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799995"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="efcb0-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="efcb0-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efcb0-105">Representa uma mensagem de chat individual dentro de uma entidade de [canal](channel.md) ou chat.</span><span class="sxs-lookup"><span data-stu-id="efcb0-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="efcb0-106">A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="efcb0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="efcb0-107">Methods</span></span>

| <span data-ttu-id="efcb0-108">Método</span><span class="sxs-lookup"><span data-stu-id="efcb0-108">Method</span></span>       | <span data-ttu-id="efcb0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="efcb0-109">Return Type</span></span>  |<span data-ttu-id="efcb0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="efcb0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efcb0-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="efcb0-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="efcb0-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="efcb0-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="efcb0-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="efcb0-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="efcb0-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="efcb0-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="efcb0-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="efcb0-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="efcb0-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="efcb0-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="efcb0-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="efcb0-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="efcb0-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="efcb0-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="efcb0-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="efcb0-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="efcb0-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="efcb0-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="efcb0-123">Enviar uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="efcb0-123">Send a message in a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="efcb0-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="efcb0-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="efcb0-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-125">Create a new top-level message in a channel.</span></span>|
|[<span data-ttu-id="efcb0-126">Responder a uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="efcb0-126">Reply to a message in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="efcb0-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="efcb0-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="efcb0-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="efcb0-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efcb0-129">Properties</span></span>
| <span data-ttu-id="efcb0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efcb0-130">Property</span></span>     | <span data-ttu-id="efcb0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="efcb0-131">Type</span></span>   |<span data-ttu-id="efcb0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="efcb0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efcb0-133">id</span><span class="sxs-lookup"><span data-stu-id="efcb0-133">id</span></span>|<span data-ttu-id="efcb0-134">String</span><span class="sxs-lookup"><span data-stu-id="efcb0-134">String</span></span>| <span data-ttu-id="efcb0-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efcb0-135">Read-only.</span></span> <span data-ttu-id="efcb0-136">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="efcb0-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="efcb0-137">replyToId</span></span>| <span data-ttu-id="efcb0-138">string</span><span class="sxs-lookup"><span data-stu-id="efcb0-138">string</span></span> | <span data-ttu-id="efcb0-139">ID da mensagem pai/raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="efcb0-139">Id of the parent message/root message of the thread.</span></span> |
|<span data-ttu-id="efcb0-140">from</span><span class="sxs-lookup"><span data-stu-id="efcb0-140">from</span></span>|[<span data-ttu-id="efcb0-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="efcb0-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="efcb0-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efcb0-142">Read only.</span></span> <span data-ttu-id="efcb0-143">Detalhes do remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-143">Details of the sender of the message.</span></span>|
|<span data-ttu-id="efcb0-144">etag</span><span class="sxs-lookup"><span data-stu-id="efcb0-144">etag</span></span>| <span data-ttu-id="efcb0-145">string</span><span class="sxs-lookup"><span data-stu-id="efcb0-145">string</span></span> | <span data-ttu-id="efcb0-146">O número de versão da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-146">Version number of the message.</span></span> |
|<span data-ttu-id="efcb0-147">messageType</span><span class="sxs-lookup"><span data-stu-id="efcb0-147">messageType</span></span>|<span data-ttu-id="efcb0-148">String</span><span class="sxs-lookup"><span data-stu-id="efcb0-148">String</span></span>|<span data-ttu-id="efcb0-149">Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing.</span><span class="sxs-lookup"><span data-stu-id="efcb0-149">The type of message, current supported values are: message, chatEvent, Typing.</span></span>|
|<span data-ttu-id="efcb0-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efcb0-150">createdDateTime</span></span>|<span data-ttu-id="efcb0-151">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcb0-151">dateTimeOffset</span></span>|<span data-ttu-id="efcb0-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efcb0-152">Read only.</span></span> <span data-ttu-id="efcb0-153">Carimbo de data/hora de quando a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="efcb0-153">Timestamp of when the message was created.</span></span>|
|<span data-ttu-id="efcb0-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efcb0-154">lastModifiedDateTime</span></span>|<span data-ttu-id="efcb0-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcb0-155">dateTimeOffset</span></span>|<span data-ttu-id="efcb0-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efcb0-156">Read only.</span></span> <span data-ttu-id="efcb0-157">Carimbo de data/hora de quando a mensagem foi editada/atualizada.</span><span class="sxs-lookup"><span data-stu-id="efcb0-157">Timestamp of when the message was edited/updated.</span></span>|
|<span data-ttu-id="efcb0-158">deleted</span><span class="sxs-lookup"><span data-stu-id="efcb0-158">deleted</span></span>|<span data-ttu-id="efcb0-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="efcb0-159">Boolean</span></span>|<span data-ttu-id="efcb0-160">Indica se uma mensagem foi excluída de modo reversível.</span><span class="sxs-lookup"><span data-stu-id="efcb0-160">Indicates whether a message has been soft deleted.</span></span>|
|<span data-ttu-id="efcb0-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="efcb0-161">deletedDateTime</span></span>|<span data-ttu-id="efcb0-162">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efcb0-162">dateTimeOffset</span></span>|<span data-ttu-id="efcb0-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efcb0-163">Read only.</span></span> <span data-ttu-id="efcb0-164">Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="efcb0-164">Timestamp at which the message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="efcb0-165">corpo</span><span class="sxs-lookup"><span data-stu-id="efcb0-165">body</span></span>|[<span data-ttu-id="efcb0-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="efcb0-166">itemBody</span></span>](itembody.md)|<span data-ttu-id="efcb0-167">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-167">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="efcb0-168">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="efcb0-168">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="efcb0-169">summary</span><span class="sxs-lookup"><span data-stu-id="efcb0-169">summary</span></span>|<span data-ttu-id="efcb0-170">string</span><span class="sxs-lookup"><span data-stu-id="efcb0-170">string</span></span>|<span data-ttu-id="efcb0-171">Texto de resumo da mensagem que poderia ser usado para notificações por push e modos de exibição de resumo ou de fallback</span><span class="sxs-lookup"><span data-stu-id="efcb0-171">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="efcb0-172">mentions</span><span class="sxs-lookup"><span data-stu-id="efcb0-172">mentions</span></span>|<span data-ttu-id="efcb0-173">[chatMessageMention](chatmention.md) collection</span><span class="sxs-lookup"><span data-stu-id="efcb0-173">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="efcb0-174">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="efcb0-174">List of entities mentioned in the message.</span></span> <span data-ttu-id="efcb0-175">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="efcb0-175">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="efcb0-176">importância</span><span class="sxs-lookup"><span data-stu-id="efcb0-176">importance</span></span>| <span data-ttu-id="efcb0-177">string</span><span class="sxs-lookup"><span data-stu-id="efcb0-177">string</span></span> | <span data-ttu-id="efcb0-178">A importância da mensagem: Normal, Alta.</span><span class="sxs-lookup"><span data-stu-id="efcb0-178">The importance of the message: Normal, High.</span></span>|
|<span data-ttu-id="efcb0-179">reactions</span><span class="sxs-lookup"><span data-stu-id="efcb0-179">reactions</span></span>| <span data-ttu-id="efcb0-180">[chatMessageReaction](chatreaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="efcb0-180">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="efcb0-181">Reações para essa mensagem (por exemplo, Curtir)</span><span class="sxs-lookup"><span data-stu-id="efcb0-181">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="efcb0-182">locale</span><span class="sxs-lookup"><span data-stu-id="efcb0-182">locale</span></span>|<span data-ttu-id="efcb0-183">string</span><span class="sxs-lookup"><span data-stu-id="efcb0-183">string</span></span>|<span data-ttu-id="efcb0-184">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="efcb0-184">Locale of the message set by the client</span></span>|
|<span data-ttu-id="efcb0-185">attachments</span><span class="sxs-lookup"><span data-stu-id="efcb0-185">attachments</span></span>|<span data-ttu-id="efcb0-186">[chatMessageAttachment](chatattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="efcb0-186">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="efcb0-187">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="efcb0-187">Attached files.</span></span> <span data-ttu-id="efcb0-188">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="efcb0-188">Attachments are currently read-only – sending attachments is not supported.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="efcb0-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efcb0-189">JSON representation</span></span>

<span data-ttu-id="efcb0-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efcb0-190">The following is a JSON representation of the resource.</span></span>

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
