---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: ef91281eff0cc61f992f659bd33debec03841bb4
ms.sourcegitcommit: a1f1e59ee568340bfabdb524e01cff7860bcc862
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2019
ms.locfileid: "29735576"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="90c1e-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="90c1e-104">chatMessage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90c1e-105">Representa uma mensagem de chat individual dentro de uma entidade de [canal](channel.md) ou chat.</span><span class="sxs-lookup"><span data-stu-id="90c1e-105">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="90c1e-106">A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c1e-106">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="90c1e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="90c1e-107">Methods</span></span>

| <span data-ttu-id="90c1e-108">Método</span><span class="sxs-lookup"><span data-stu-id="90c1e-108">Method</span></span>       | <span data-ttu-id="90c1e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="90c1e-109">Return Type</span></span>  |<span data-ttu-id="90c1e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="90c1e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90c1e-111">List Channel messages</span><span class="sxs-lookup"><span data-stu-id="90c1e-111">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="90c1e-112">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="90c1e-112">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="90c1e-113">Obtenha uma lista de todas as mensagens raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="90c1e-113">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="90c1e-114">Get Channel message</span><span class="sxs-lookup"><span data-stu-id="90c1e-114">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="90c1e-115">chatmessage</span><span class="sxs-lookup"><span data-stu-id="90c1e-115">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="90c1e-116">Obtenha uma mensagem raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="90c1e-116">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="90c1e-117">List replies to a message</span><span class="sxs-lookup"><span data-stu-id="90c1e-117">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="90c1e-118">[chatmessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="90c1e-118">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="90c1e-119">Obtenha a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="90c1e-119">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="90c1e-120">Get a reply to a message</span><span class="sxs-lookup"><span data-stu-id="90c1e-120">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="90c1e-121">chatmessage</span><span class="sxs-lookup"><span data-stu-id="90c1e-121">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="90c1e-122">Obtenha uma resposta a uma mensagem única em um canal.</span><span class="sxs-lookup"><span data-stu-id="90c1e-122">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="90c1e-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90c1e-123">Properties</span></span>
| <span data-ttu-id="90c1e-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90c1e-124">Property</span></span>     | <span data-ttu-id="90c1e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="90c1e-125">Type</span></span>   |<span data-ttu-id="90c1e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="90c1e-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90c1e-127">id</span><span class="sxs-lookup"><span data-stu-id="90c1e-127">id</span></span>|<span data-ttu-id="90c1e-128">String</span><span class="sxs-lookup"><span data-stu-id="90c1e-128">String</span></span>| <span data-ttu-id="90c1e-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90c1e-129">Read-only.</span></span> <span data-ttu-id="90c1e-130">ID única da mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c1e-130">Unique ID of the message.</span></span>|
|<span data-ttu-id="90c1e-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="90c1e-131">replyToId</span></span>| <span data-ttu-id="90c1e-132">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-132">string</span></span> | <span data-ttu-id="90c1e-133">ID da mensagem pai/raiz do thread</span><span class="sxs-lookup"><span data-stu-id="90c1e-133">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="90c1e-134">from</span><span class="sxs-lookup"><span data-stu-id="90c1e-134">from</span></span>|[<span data-ttu-id="90c1e-135">identitySet</span><span class="sxs-lookup"><span data-stu-id="90c1e-135">identitySet</span></span>](identityset.md)| <span data-ttu-id="90c1e-136">Detalhes do remetente da mensagem</span><span class="sxs-lookup"><span data-stu-id="90c1e-136">Details of the sender of the message</span></span>|
|<span data-ttu-id="90c1e-137">etag</span><span class="sxs-lookup"><span data-stu-id="90c1e-137">etag</span></span>| <span data-ttu-id="90c1e-138">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-138">string</span></span> | <span data-ttu-id="90c1e-139">O número de versão da mensagem</span><span class="sxs-lookup"><span data-stu-id="90c1e-139">Version number of the message</span></span> |
|<span data-ttu-id="90c1e-140">messageType</span><span class="sxs-lookup"><span data-stu-id="90c1e-140">messageType</span></span>|<span data-ttu-id="90c1e-141">String</span><span class="sxs-lookup"><span data-stu-id="90c1e-141">String</span></span>|<span data-ttu-id="90c1e-142">Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing</span><span class="sxs-lookup"><span data-stu-id="90c1e-142">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="90c1e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90c1e-143">createdDateTime</span></span>|<span data-ttu-id="90c1e-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c1e-144">dateTimeOffset</span></span>|<span data-ttu-id="90c1e-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90c1e-145">Read only.</span></span> <span data-ttu-id="90c1e-146">Carimbo de data/hora de quando a mensagem foi criada</span><span class="sxs-lookup"><span data-stu-id="90c1e-146">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="90c1e-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90c1e-147">lastModifiedDateTime</span></span>|<span data-ttu-id="90c1e-148">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c1e-148">dateTimeOffset</span></span>|<span data-ttu-id="90c1e-149">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90c1e-149">Read only.</span></span> <span data-ttu-id="90c1e-150">Carimbo de data/hora de quando a mensagem foi editada/atualizada</span><span class="sxs-lookup"><span data-stu-id="90c1e-150">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="90c1e-151">deleted</span><span class="sxs-lookup"><span data-stu-id="90c1e-151">deleted</span></span>|<span data-ttu-id="90c1e-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="90c1e-152">Boolean</span></span>|<span data-ttu-id="90c1e-153">Indica se uma mensagem foi excluída de modo reversível</span><span class="sxs-lookup"><span data-stu-id="90c1e-153">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="90c1e-154">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="90c1e-154">deletedDateTime</span></span>|<span data-ttu-id="90c1e-155">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90c1e-155">dateTimeOffset</span></span>|<span data-ttu-id="90c1e-156">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="90c1e-156">Read only.</span></span> <span data-ttu-id="90c1e-157">Carimbo de data/hora no qual a mensagem foi excluída</span><span class="sxs-lookup"><span data-stu-id="90c1e-157">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="90c1e-158">subject</span><span class="sxs-lookup"><span data-stu-id="90c1e-158">subject</span></span>|<span data-ttu-id="90c1e-159">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-159">string</span></span>|<span data-ttu-id="90c1e-160">Linha de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c1e-160">Message subject line.</span></span> <span data-ttu-id="90c1e-161">Opcional</span><span class="sxs-lookup"><span data-stu-id="90c1e-161">Optional</span></span>|
|<span data-ttu-id="90c1e-162">body</span><span class="sxs-lookup"><span data-stu-id="90c1e-162">body</span></span>|[<span data-ttu-id="90c1e-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="90c1e-163">itemBody</span></span>](itembody.md)|<span data-ttu-id="90c1e-164">Representação de texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c1e-164">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="90c1e-165">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="90c1e-165">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="90c1e-166">summary</span><span class="sxs-lookup"><span data-stu-id="90c1e-166">summary</span></span>|<span data-ttu-id="90c1e-167">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-167">string</span></span>|<span data-ttu-id="90c1e-168">Texto de resumo da mensagem que poderia ser usado para notificações por push e modos de exibição de resumo ou de fallback</span><span class="sxs-lookup"><span data-stu-id="90c1e-168">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="90c1e-169">mentions</span><span class="sxs-lookup"><span data-stu-id="90c1e-169">mentions</span></span>|<span data-ttu-id="90c1e-170">[chatMessageMention](chatmention.md) collection</span><span class="sxs-lookup"><span data-stu-id="90c1e-170">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="90c1e-171">Lista de entidades mencionada na mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c1e-171">List of entities mentioned in the message.</span></span> <span data-ttu-id="90c1e-172">Atualmente, dá suporte a usuário, bot, equipe, canal</span><span class="sxs-lookup"><span data-stu-id="90c1e-172">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="90c1e-173">importance</span><span class="sxs-lookup"><span data-stu-id="90c1e-173">importance</span></span>| <span data-ttu-id="90c1e-174">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-174">string</span></span> | <span data-ttu-id="90c1e-175">A importância da mensagem: Normal, Alta</span><span class="sxs-lookup"><span data-stu-id="90c1e-175">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="90c1e-176">reactions</span><span class="sxs-lookup"><span data-stu-id="90c1e-176">reactions</span></span>| <span data-ttu-id="90c1e-177">[chatMessageReaction](chatreaction.md) collection</span><span class="sxs-lookup"><span data-stu-id="90c1e-177">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="90c1e-178">Reações para essa mensagem (por exemplo, Curtir)</span><span class="sxs-lookup"><span data-stu-id="90c1e-178">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="90c1e-179">locale</span><span class="sxs-lookup"><span data-stu-id="90c1e-179">locale</span></span>|<span data-ttu-id="90c1e-180">string</span><span class="sxs-lookup"><span data-stu-id="90c1e-180">string</span></span>|<span data-ttu-id="90c1e-181">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="90c1e-181">Locale of the message set by the client</span></span>|
|<span data-ttu-id="90c1e-182">attachments</span><span class="sxs-lookup"><span data-stu-id="90c1e-182">attachments</span></span>|<span data-ttu-id="90c1e-183">[chatMessageAttachment](chatattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="90c1e-183">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="90c1e-184">Arquivos anexos</span><span class="sxs-lookup"><span data-stu-id="90c1e-184">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="90c1e-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90c1e-185">JSON representation</span></span>

<span data-ttu-id="90c1e-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90c1e-186">The following is a JSON representation of the resource.</span></span>

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
