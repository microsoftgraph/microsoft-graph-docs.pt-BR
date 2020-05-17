---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2030a208ed61b7137d22c29eee2743b67556c92d
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272739"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="41b21-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="41b21-104">chatMessage resource type</span></span>

<span data-ttu-id="41b21-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41b21-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41b21-106">Representa uma mensagem de chat individual dentro de um [canal](./channel.md) ou em um [chat](/graph/api/resources/chat?view=graph-rest-beta)(na versão beta).</span><span class="sxs-lookup"><span data-stu-id="41b21-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta).</span></span> <span data-ttu-id="41b21-107">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="41b21-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="41b21-108">Methods</span></span>

| <span data-ttu-id="41b21-109">Método</span><span class="sxs-lookup"><span data-stu-id="41b21-109">Method</span></span>       | <span data-ttu-id="41b21-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="41b21-110">Return Type</span></span>  |<span data-ttu-id="41b21-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b21-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41b21-112">**Mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="41b21-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="41b21-113">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="41b21-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="41b21-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="41b21-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="41b21-115">Criar uma nova mensagem de chat de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="41b21-115">Create a new top-level chat message in a channel.</span></span>|
|<span data-ttu-id="41b21-116">**Respostas de mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="41b21-116">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="41b21-117">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="41b21-117">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="41b21-118">chatMessage</span><span class="sxs-lookup"><span data-stu-id="41b21-118">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="41b21-119">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="41b21-119">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="41b21-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41b21-120">Properties</span></span>

| <span data-ttu-id="41b21-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41b21-121">Property</span></span>   | <span data-ttu-id="41b21-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="41b21-122">Type</span></span> |<span data-ttu-id="41b21-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="41b21-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41b21-124">id</span><span class="sxs-lookup"><span data-stu-id="41b21-124">id</span></span>|<span data-ttu-id="41b21-125">String</span><span class="sxs-lookup"><span data-stu-id="41b21-125">String</span></span>| <span data-ttu-id="41b21-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-126">Read-only.</span></span> <span data-ttu-id="41b21-127">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="41b21-127">Unique Id of the message.</span></span>|
|<span data-ttu-id="41b21-128">replyToId</span><span class="sxs-lookup"><span data-stu-id="41b21-128">replyToId</span></span>| <span data-ttu-id="41b21-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41b21-129">string</span></span> | <span data-ttu-id="41b21-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-130">Read-only.</span></span> <span data-ttu-id="41b21-131">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="41b21-131">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="41b21-132">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="41b21-132">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="41b21-133">from</span><span class="sxs-lookup"><span data-stu-id="41b21-133">from</span></span>|[<span data-ttu-id="41b21-134">identitySet</span><span class="sxs-lookup"><span data-stu-id="41b21-134">identitySet</span></span>](identityset.md)| <span data-ttu-id="41b21-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-135">Read only.</span></span> <span data-ttu-id="41b21-136">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-136">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="41b21-137">etag</span><span class="sxs-lookup"><span data-stu-id="41b21-137">etag</span></span>| <span data-ttu-id="41b21-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41b21-138">string</span></span> | <span data-ttu-id="41b21-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-139">Read-only.</span></span> <span data-ttu-id="41b21-140">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-140">Version number of the chat message.</span></span> |
|<span data-ttu-id="41b21-141">messageType</span><span class="sxs-lookup"><span data-stu-id="41b21-141">messageType</span></span>|<span data-ttu-id="41b21-142">string</span><span class="sxs-lookup"><span data-stu-id="41b21-142">string</span></span>|<span data-ttu-id="41b21-143">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-143">The type of chat message.</span></span> <span data-ttu-id="41b21-144">Os valores possíveis são: `message` .</span><span class="sxs-lookup"><span data-stu-id="41b21-144">The possible values are: `message`.</span></span>|
|<span data-ttu-id="41b21-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41b21-145">createdDateTime</span></span>|<span data-ttu-id="41b21-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41b21-146">dateTimeOffset</span></span>|<span data-ttu-id="41b21-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-147">Read only.</span></span> <span data-ttu-id="41b21-148">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="41b21-148">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="41b21-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41b21-149">lastModifiedDateTime</span></span>|<span data-ttu-id="41b21-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41b21-150">dateTimeOffset</span></span>|<span data-ttu-id="41b21-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-151">Read only.</span></span> <span data-ttu-id="41b21-152">Carimbo de data/hora de quando a mensagem de chat é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem de chat raiz em um canal) ou uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="41b21-152">Timestamp of when the chat message is created or edited, including when a reply is made (if it's a root chat message in a channel) or a reaction is added or removed.</span></span> |
|<span data-ttu-id="41b21-153">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="41b21-153">deletedDateTime</span></span>|<span data-ttu-id="41b21-154">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41b21-154">dateTimeOffset</span></span>|<span data-ttu-id="41b21-155">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41b21-155">Read only.</span></span> <span data-ttu-id="41b21-156">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="41b21-156">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="41b21-157">subject</span><span class="sxs-lookup"><span data-stu-id="41b21-157">subject</span></span>|<span data-ttu-id="41b21-158">string</span><span class="sxs-lookup"><span data-stu-id="41b21-158">string</span></span>| <span data-ttu-id="41b21-159">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="41b21-159">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="41b21-160">body</span><span class="sxs-lookup"><span data-stu-id="41b21-160">body</span></span>|[<span data-ttu-id="41b21-161">itemBody</span><span class="sxs-lookup"><span data-stu-id="41b21-161">itemBody</span></span>](itembody.md)|<span data-ttu-id="41b21-162">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-162">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="41b21-163">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="41b21-163">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="41b21-164">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="41b21-164">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="41b21-165">summary</span><span class="sxs-lookup"><span data-stu-id="41b21-165">summary</span></span>|<span data-ttu-id="41b21-166">string</span><span class="sxs-lookup"><span data-stu-id="41b21-166">string</span></span>| <span data-ttu-id="41b21-167">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="41b21-167">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="41b21-168">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-168">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="41b21-169">attachments</span><span class="sxs-lookup"><span data-stu-id="41b21-169">attachments</span></span>|<span data-ttu-id="41b21-170">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="41b21-170">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="41b21-171">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="41b21-171">Attached files.</span></span> <span data-ttu-id="41b21-172">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="41b21-172">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="41b21-173">mentions</span><span class="sxs-lookup"><span data-stu-id="41b21-173">mentions</span></span>|<span data-ttu-id="41b21-174">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="41b21-174">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="41b21-175">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-175">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="41b21-176">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="41b21-176">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="41b21-177">importância</span><span class="sxs-lookup"><span data-stu-id="41b21-177">importance</span></span>| <span data-ttu-id="41b21-178">string</span><span class="sxs-lookup"><span data-stu-id="41b21-178">string</span></span> | <span data-ttu-id="41b21-179">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="41b21-179">The importance of the chat message.</span></span> <span data-ttu-id="41b21-180">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="41b21-180">The possible values are: `normal`, `high`, `urgent`.</span></span>|
|<span data-ttu-id="41b21-181">localidade</span><span class="sxs-lookup"><span data-stu-id="41b21-181">locale</span></span>|<span data-ttu-id="41b21-182">string</span><span class="sxs-lookup"><span data-stu-id="41b21-182">string</span></span>|<span data-ttu-id="41b21-183">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41b21-183">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41b21-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41b21-184">JSON representation</span></span>

<span data-ttu-id="41b21-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41b21-185">The following is a JSON representation of the resource.</span></span>

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
  "locale": "string",
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
