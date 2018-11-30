---
title: tipo de recurso de chatMessage
description: Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de canal. A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033268"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="a9c10-104">tipo de recurso de chatMessage</span><span class="sxs-lookup"><span data-stu-id="a9c10-104">chatMessage resource type</span></span>

> <span data-ttu-id="a9c10-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a9c10-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9c10-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a9c10-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9c10-107">Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de [canal](channel.md) .</span><span class="sxs-lookup"><span data-stu-id="a9c10-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="a9c10-108">A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9c10-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="a9c10-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a9c10-109">Methods</span></span>

| <span data-ttu-id="a9c10-110">Método</span><span class="sxs-lookup"><span data-stu-id="a9c10-110">Method</span></span>       | <span data-ttu-id="a9c10-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a9c10-111">Return Type</span></span>  |<span data-ttu-id="a9c10-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c10-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a9c10-113">Mensagens de canal de lista</span><span class="sxs-lookup"><span data-stu-id="a9c10-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="a9c10-114">coleção [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="a9c10-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="a9c10-115">Obter a lista de todas as mensagens de raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="a9c10-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="a9c10-116">Mensagem de canal Get</span><span class="sxs-lookup"><span data-stu-id="a9c10-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="a9c10-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="a9c10-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="a9c10-118">Obtenha uma mensagem de raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="a9c10-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="a9c10-119">Lista de respostas a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="a9c10-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="a9c10-120">coleção [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="a9c10-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="a9c10-121">Obter a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="a9c10-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="a9c10-122">Obtenha uma resposta a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="a9c10-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="a9c10-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="a9c10-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="a9c10-124">Obtenha uma única resposta a uma mensagem em um canal.</span><span class="sxs-lookup"><span data-stu-id="a9c10-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="a9c10-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9c10-125">Properties</span></span>
| <span data-ttu-id="a9c10-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9c10-126">Property</span></span>     | <span data-ttu-id="a9c10-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9c10-127">Type</span></span>   |<span data-ttu-id="a9c10-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9c10-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9c10-129">id</span><span class="sxs-lookup"><span data-stu-id="a9c10-129">id</span></span>|<span data-ttu-id="a9c10-130">String</span><span class="sxs-lookup"><span data-stu-id="a9c10-130">String</span></span>| <span data-ttu-id="a9c10-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c10-131">Read-only.</span></span> <span data-ttu-id="a9c10-132">Identificação exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9c10-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="a9c10-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="a9c10-133">replyToId</span></span>| <span data-ttu-id="a9c10-134">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-134">string</span></span> | <span data-ttu-id="a9c10-135">ID da mensagem pai mensagem/raiz do thread</span><span class="sxs-lookup"><span data-stu-id="a9c10-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="a9c10-136">from</span><span class="sxs-lookup"><span data-stu-id="a9c10-136">from</span></span>|[<span data-ttu-id="a9c10-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9c10-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="a9c10-138">Detalhes do remetente da mensagem</span><span class="sxs-lookup"><span data-stu-id="a9c10-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="a9c10-139">etag</span><span class="sxs-lookup"><span data-stu-id="a9c10-139">etag</span></span>| <span data-ttu-id="a9c10-140">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-140">string</span></span> | <span data-ttu-id="a9c10-141">Número de versão da mensagem</span><span class="sxs-lookup"><span data-stu-id="a9c10-141">Version number of the message</span></span> |
|<span data-ttu-id="a9c10-142">messageType</span><span class="sxs-lookup"><span data-stu-id="a9c10-142">messageType</span></span>|<span data-ttu-id="a9c10-143">String</span><span class="sxs-lookup"><span data-stu-id="a9c10-143">String</span></span>|<span data-ttu-id="a9c10-144">Os valores de tipo de mensagem, atual com suporte são: mensagem, chatEvent, digitando</span><span class="sxs-lookup"><span data-stu-id="a9c10-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="a9c10-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c10-145">createdDateTime</span></span>|<span data-ttu-id="a9c10-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c10-146">dateTimeOffset</span></span>|<span data-ttu-id="a9c10-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c10-147">Read only.</span></span> <span data-ttu-id="a9c10-148">Carimbo de hora de quando a mensagem foi criada</span><span class="sxs-lookup"><span data-stu-id="a9c10-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="a9c10-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c10-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a9c10-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c10-150">dateTimeOffset</span></span>|<span data-ttu-id="a9c10-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c10-151">Read only.</span></span> <span data-ttu-id="a9c10-152">Carimbo de hora de quando a mensagem foi editado/atualizado</span><span class="sxs-lookup"><span data-stu-id="a9c10-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="a9c10-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a9c10-153">isDeleted</span></span>|<span data-ttu-id="a9c10-154">booliano</span><span class="sxs-lookup"><span data-stu-id="a9c10-154">boolean</span></span>|<span data-ttu-id="a9c10-155">Representa se uma mensagem tiver sido excluída soft</span><span class="sxs-lookup"><span data-stu-id="a9c10-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="a9c10-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c10-156">deletedDateTime</span></span>|<span data-ttu-id="a9c10-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c10-157">dateTimeOffset</span></span>|<span data-ttu-id="a9c10-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c10-158">Read only.</span></span> <span data-ttu-id="a9c10-159">Carimbo de hora em que a mensagem foi excluída.</span><span class="sxs-lookup"><span data-stu-id="a9c10-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="a9c10-160">subject</span><span class="sxs-lookup"><span data-stu-id="a9c10-160">subject</span></span>|<span data-ttu-id="a9c10-161">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-161">string</span></span>|<span data-ttu-id="a9c10-162">Linha de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9c10-162">Message subject line.</span></span> <span data-ttu-id="a9c10-163">Opcional</span><span class="sxs-lookup"><span data-stu-id="a9c10-163">Optional</span></span>|
|<span data-ttu-id="a9c10-164">body</span><span class="sxs-lookup"><span data-stu-id="a9c10-164">body</span></span>|[<span data-ttu-id="a9c10-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="a9c10-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="a9c10-166">Representação em texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9c10-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="a9c10-167">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="a9c10-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="a9c10-168">Resumo</span><span class="sxs-lookup"><span data-stu-id="a9c10-168">summary</span></span>|<span data-ttu-id="a9c10-169">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-169">string</span></span>|<span data-ttu-id="a9c10-170">Texto da mensagem que poderia ser usada para notificações por push e modos de exibição de resumo ou regressivo queda de modos de exibição de resumo</span><span class="sxs-lookup"><span data-stu-id="a9c10-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="a9c10-171">menções</span><span class="sxs-lookup"><span data-stu-id="a9c10-171">mentions</span></span>|<span data-ttu-id="a9c10-172">coleção [chatMessageMention](chatmention.md)</span><span class="sxs-lookup"><span data-stu-id="a9c10-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="a9c10-173">Lista de entidades mencionado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="a9c10-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="a9c10-174">Suporta atualmente o usuário, bot, equipe, de canal</span><span class="sxs-lookup"><span data-stu-id="a9c10-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="a9c10-175">importance</span><span class="sxs-lookup"><span data-stu-id="a9c10-175">importance</span></span>| <span data-ttu-id="a9c10-176">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-176">string</span></span> | <span data-ttu-id="a9c10-177">A importância da mensagem: Normal, alta</span><span class="sxs-lookup"><span data-stu-id="a9c10-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="a9c10-178">reações</span><span class="sxs-lookup"><span data-stu-id="a9c10-178">reactions</span></span>| <span data-ttu-id="a9c10-179">coleção [chatMessageReaction](chatreaction.md)</span><span class="sxs-lookup"><span data-stu-id="a9c10-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="a9c10-180">Reações para esta mensagem (por exemplo,-Like)</span><span class="sxs-lookup"><span data-stu-id="a9c10-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="a9c10-181">localidade</span><span class="sxs-lookup"><span data-stu-id="a9c10-181">locale</span></span>|<span data-ttu-id="a9c10-182">string</span><span class="sxs-lookup"><span data-stu-id="a9c10-182">string</span></span>|<span data-ttu-id="a9c10-183">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="a9c10-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="a9c10-184">attachments</span><span class="sxs-lookup"><span data-stu-id="a9c10-184">attachments</span></span>|<span data-ttu-id="a9c10-185">coleção [chatMessageAttachment](chatattachment.md)</span><span class="sxs-lookup"><span data-stu-id="a9c10-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="a9c10-186">Arquivos anexados</span><span class="sxs-lookup"><span data-stu-id="a9c10-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a9c10-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9c10-187">JSON representation</span></span>

<span data-ttu-id="a9c10-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9c10-188">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
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
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
