---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: f61668d8c3892482043dd7531a6699974a964527
ms.sourcegitcommit: d1a9e7c8e1376a99c5a5416257889ec113613a77
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/07/2019
ms.locfileid: "30458656"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="e0a00-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="e0a00-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0a00-105">Representa uma mensagem de chat individual dentro de uma entidade de [canal](channel.md) ou chat.</span><span class="sxs-lookup"><span data-stu-id="e0a00-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="e0a00-106">A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0a00-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="e0a00-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e0a00-107">Methods</span></span>

| <span data-ttu-id="e0a00-108">Método</span><span class="sxs-lookup"><span data-stu-id="e0a00-108">Method</span></span>       | <span data-ttu-id="e0a00-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e0a00-109">Return Type</span></span>  |<span data-ttu-id="e0a00-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a00-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0a00-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="e0a00-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="e0a00-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0a00-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e0a00-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="e0a00-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="e0a00-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="e0a00-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e0a00-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="e0a00-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="e0a00-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="e0a00-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="e0a00-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0a00-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="e0a00-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="e0a00-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="e0a00-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="e0a00-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e0a00-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="e0a00-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-122">Get a single reply to a message in a channel.</span></span>|
|[<span data-ttu-id="e0a00-123">Enviar uma mensagem em um canal</span><span class="sxs-lookup"><span data-stu-id="e0a00-123">Send a message to a channel</span></span>](../api/channel-post-chatmessage.md) | [<span data-ttu-id="e0a00-124">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e0a00-124">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="e0a00-125">Crie uma nova mensagem de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-125">Use Create a message in a channel instead.</span></span>|
|<span data-ttu-id="e0a00-126">[Responder a uma mensagem em um canal](../api/channel-post-messagereply.md)</span><span class="sxs-lookup"><span data-stu-id="e0a00-126">Introduced the [Reply to a message in a channel](../api/channel-post-messagereply.md) API.</span></span> | [<span data-ttu-id="e0a00-127">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e0a00-127">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="e0a00-128">Responder a uma mensagem existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="e0a00-128">Reply to an existing message in a channel.</span></span>|


## <a name="properties"></a><span data-ttu-id="e0a00-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e0a00-129">Properties</span></span>
| <span data-ttu-id="e0a00-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0a00-130">Property</span></span>     | <span data-ttu-id="e0a00-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0a00-131">Type</span></span>   |<span data-ttu-id="e0a00-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0a00-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0a00-133">id</span><span class="sxs-lookup"><span data-stu-id="e0a00-133">id</span></span>|<span data-ttu-id="e0a00-134">String</span><span class="sxs-lookup"><span data-stu-id="e0a00-134">String</span></span>| <span data-ttu-id="e0a00-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0a00-135">Read-only.</span></span> <span data-ttu-id="e0a00-136">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0a00-136">Unique ID of the message.</span></span>|
|<span data-ttu-id="e0a00-137">replyToId</span><span class="sxs-lookup"><span data-stu-id="e0a00-137">replyToId</span></span>| <span data-ttu-id="e0a00-138">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-138">string</span></span> | <span data-ttu-id="e0a00-139">ID da mensagem pai/raiz do thread</span><span class="sxs-lookup"><span data-stu-id="e0a00-139">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="e0a00-140">from</span><span class="sxs-lookup"><span data-stu-id="e0a00-140">from</span></span>|[<span data-ttu-id="e0a00-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="e0a00-141">identitySet</span></span>](identityset.md)| <span data-ttu-id="e0a00-142">Detalhes do remetente da mensagem</span><span class="sxs-lookup"><span data-stu-id="e0a00-142">Details of the sender of the message</span></span>|
|<span data-ttu-id="e0a00-143">etag</span><span class="sxs-lookup"><span data-stu-id="e0a00-143">etag</span></span>| <span data-ttu-id="e0a00-144">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-144">string</span></span> | <span data-ttu-id="e0a00-145">O número de versão da mensagem</span><span class="sxs-lookup"><span data-stu-id="e0a00-145">Version number of the message</span></span> |
|<span data-ttu-id="e0a00-146">messageType</span><span class="sxs-lookup"><span data-stu-id="e0a00-146">messageType</span></span>|<span data-ttu-id="e0a00-147">String</span><span class="sxs-lookup"><span data-stu-id="e0a00-147">String</span></span>|<span data-ttu-id="e0a00-148">Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="e0a00-148">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="e0a00-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0a00-149">createdDateTime</span></span>|<span data-ttu-id="e0a00-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0a00-150">dateTimeOffset</span></span>|<span data-ttu-id="e0a00-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0a00-151">Read only.</span></span> <span data-ttu-id="e0a00-152">Carimbo de data/hora de quando a mensagem foi criada</span><span class="sxs-lookup"><span data-stu-id="e0a00-152">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="e0a00-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0a00-153">lastModifiedDateTime</span></span>|<span data-ttu-id="e0a00-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0a00-154">dateTimeOffset</span></span>|<span data-ttu-id="e0a00-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0a00-155">Read only.</span></span> <span data-ttu-id="e0a00-156">Carimbo de data/hora de quando a mensagem foi editada/atualizada</span><span class="sxs-lookup"><span data-stu-id="e0a00-156">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="e0a00-157">deleted</span><span class="sxs-lookup"><span data-stu-id="e0a00-157">deleted</span></span>|<span data-ttu-id="e0a00-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0a00-158">Boolean</span></span>|<span data-ttu-id="e0a00-159">Indica se uma mensagem foi excluída de modo reversível</span><span class="sxs-lookup"><span data-stu-id="e0a00-159">Indicates whether a message has been soft deleted</span></span>|
|<span data-ttu-id="e0a00-160">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0a00-160">deletedDateTime</span></span>|<span data-ttu-id="e0a00-161">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0a00-161">dateTimeOffset</span></span>|<span data-ttu-id="e0a00-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e0a00-162">Read only.</span></span> <span data-ttu-id="e0a00-163">Carimbo de data/hora no qual a mensagem foi excluída</span><span class="sxs-lookup"><span data-stu-id="e0a00-163">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="e0a00-164">subject</span><span class="sxs-lookup"><span data-stu-id="e0a00-164">subject</span></span>|<span data-ttu-id="e0a00-165">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-165">string</span></span>|<span data-ttu-id="e0a00-166">Linha de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0a00-166">Message subject line.</span></span> <span data-ttu-id="e0a00-167">Opcional</span><span class="sxs-lookup"><span data-stu-id="e0a00-167">Optional</span></span>|
|<span data-ttu-id="e0a00-168">body</span><span class="sxs-lookup"><span data-stu-id="e0a00-168">body</span></span>|[<span data-ttu-id="e0a00-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="e0a00-169">itemBody</span></span>](itembody.md)|<span data-ttu-id="e0a00-170">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0a00-170">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="e0a00-171">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="e0a00-171">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="e0a00-172">summary</span><span class="sxs-lookup"><span data-stu-id="e0a00-172">summary</span></span>|<span data-ttu-id="e0a00-173">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-173">string</span></span>|<span data-ttu-id="e0a00-174">Texto de resumo da mensagem que poderia ser usado para notificações por push e modos de exibição de resumo ou de fallback</span><span class="sxs-lookup"><span data-stu-id="e0a00-174">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="e0a00-175">mentions</span><span class="sxs-lookup"><span data-stu-id="e0a00-175">mentions</span></span>|<span data-ttu-id="e0a00-176">[chatMessageMention](chatmention.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0a00-176">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="e0a00-177">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e0a00-177">List of entities mentioned in the message.</span></span> <span data-ttu-id="e0a00-178">Atualmente, dá suporte a usuário, bot, equipe, canal</span><span class="sxs-lookup"><span data-stu-id="e0a00-178">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="e0a00-179">importance</span><span class="sxs-lookup"><span data-stu-id="e0a00-179">importance</span></span>| <span data-ttu-id="e0a00-180">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-180">string</span></span> | <span data-ttu-id="e0a00-181">A importância da mensagem: Normal, Alta</span><span class="sxs-lookup"><span data-stu-id="e0a00-181">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="e0a00-182">reactions</span><span class="sxs-lookup"><span data-stu-id="e0a00-182">reactions</span></span>| <span data-ttu-id="e0a00-183">[chatMessageReaction](chatreaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0a00-183">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="e0a00-184">Reações para essa mensagem (por exemplo, Curtir)</span><span class="sxs-lookup"><span data-stu-id="e0a00-184">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="e0a00-185">locale</span><span class="sxs-lookup"><span data-stu-id="e0a00-185">locale</span></span>|<span data-ttu-id="e0a00-186">string</span><span class="sxs-lookup"><span data-stu-id="e0a00-186">string</span></span>|<span data-ttu-id="e0a00-187">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="e0a00-187">Locale of the message set by the client</span></span>|
|<span data-ttu-id="e0a00-188">attachments</span><span class="sxs-lookup"><span data-stu-id="e0a00-188">attachments</span></span>|<span data-ttu-id="e0a00-189">[chatMessageAttachment](chatattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="e0a00-189">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="e0a00-190">Arquivos anexos</span><span class="sxs-lookup"><span data-stu-id="e0a00-190">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e0a00-191">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e0a00-191">JSON representation</span></span>

<span data-ttu-id="e0a00-192">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e0a00-192">The following is a JSON representation of the resource.</span></span>

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
