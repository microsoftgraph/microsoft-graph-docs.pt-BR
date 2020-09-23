---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: af025ad2484757626fec08d9131a870cb345e492
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223209"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c87e1-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="c87e1-104">chatMessage resource type</span></span>

<span data-ttu-id="c87e1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c87e1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c87e1-106">Representa uma mensagem de chat individual dentro de um [canal](./channel.md) ou em um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)(na versão beta).</span><span class="sxs-lookup"><span data-stu-id="c87e1-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="c87e1-107">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="c87e1-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c87e1-108">Methods</span></span>

| <span data-ttu-id="c87e1-109">Método</span><span class="sxs-lookup"><span data-stu-id="c87e1-109">Method</span></span>       | <span data-ttu-id="c87e1-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c87e1-110">Return Type</span></span>  |<span data-ttu-id="c87e1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c87e1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c87e1-112">**Mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="c87e1-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="c87e1-113">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="c87e1-113">Create chatMessage in a channel</span></span>](../api/channel-post-messages.md) | [<span data-ttu-id="c87e1-114">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c87e1-114">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="c87e1-115">Criar uma nova mensagem de chat de nível superior em um canal.</span><span class="sxs-lookup"><span data-stu-id="c87e1-115">Create a new top-level chat message in a channel.</span></span>|
|[<span data-ttu-id="c87e1-116">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="c87e1-116">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="c87e1-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c87e1-117">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c87e1-118">Atualizar a propriedade **policyViolation** de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-118">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="c87e1-119">**Respostas de mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="c87e1-119">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="c87e1-120">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="c87e1-120">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c87e1-121">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c87e1-121">chatMessage</span></span>](#chatmessage-resource-type)| <span data-ttu-id="c87e1-122">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="c87e1-122">Reply to an existing chat message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="c87e1-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c87e1-123">Properties</span></span>

| <span data-ttu-id="c87e1-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c87e1-124">Property</span></span>   | <span data-ttu-id="c87e1-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="c87e1-125">Type</span></span> |<span data-ttu-id="c87e1-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c87e1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c87e1-127">id</span><span class="sxs-lookup"><span data-stu-id="c87e1-127">id</span></span>|<span data-ttu-id="c87e1-128">String</span><span class="sxs-lookup"><span data-stu-id="c87e1-128">String</span></span>| <span data-ttu-id="c87e1-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-129">Read-only.</span></span> <span data-ttu-id="c87e1-130">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c87e1-130">Unique Id of the message.</span></span>|
|<span data-ttu-id="c87e1-131">replyToId</span><span class="sxs-lookup"><span data-stu-id="c87e1-131">replyToId</span></span>| <span data-ttu-id="c87e1-132">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-132">string</span></span> | <span data-ttu-id="c87e1-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-133">Read-only.</span></span> <span data-ttu-id="c87e1-134">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="c87e1-134">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="c87e1-135">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="c87e1-135">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="c87e1-136">from</span><span class="sxs-lookup"><span data-stu-id="c87e1-136">from</span></span>|[<span data-ttu-id="c87e1-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="c87e1-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="c87e1-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-138">Read only.</span></span> <span data-ttu-id="c87e1-139">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-139">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="c87e1-140">etag</span><span class="sxs-lookup"><span data-stu-id="c87e1-140">etag</span></span>| <span data-ttu-id="c87e1-141">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-141">string</span></span> | <span data-ttu-id="c87e1-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-142">Read-only.</span></span> <span data-ttu-id="c87e1-143">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-143">Version number of the chat message.</span></span> |
|<span data-ttu-id="c87e1-144">messageType</span><span class="sxs-lookup"><span data-stu-id="c87e1-144">messageType</span></span>|<span data-ttu-id="c87e1-145">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-145">string</span></span>|<span data-ttu-id="c87e1-146">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-146">The type of chat message.</span></span> <span data-ttu-id="c87e1-147">Os valores possíveis são: `message` .</span><span class="sxs-lookup"><span data-stu-id="c87e1-147">The possible values are: `message`.</span></span>|
|<span data-ttu-id="c87e1-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c87e1-148">createdDateTime</span></span>|<span data-ttu-id="c87e1-149">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87e1-149">dateTimeOffset</span></span>|<span data-ttu-id="c87e1-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-150">Read only.</span></span> <span data-ttu-id="c87e1-151">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="c87e1-151">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="c87e1-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c87e1-152">lastModifiedDateTime</span></span>|<span data-ttu-id="c87e1-153">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87e1-153">dateTimeOffset</span></span>|<span data-ttu-id="c87e1-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-154">Read only.</span></span> <span data-ttu-id="c87e1-155">Carimbo de data/hora em que a mensagem de chat é criada (configuração inicial) ou editada, incluindo quando uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="c87e1-155">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="c87e1-156">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="c87e1-156">lastEditedDateTime</span></span>|<span data-ttu-id="c87e1-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87e1-157">dateTimeOffset</span></span>|<span data-ttu-id="c87e1-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-158">Read only.</span></span> <span data-ttu-id="c87e1-159">Carimbo de data/hora em que foram feitas edições na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-159">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="c87e1-160">Dispara um sinalizador "editado" na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c87e1-160">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="c87e1-161">Se não for feita nenhuma edição, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="c87e1-161">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="c87e1-162">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c87e1-162">deletedDateTime</span></span>|<span data-ttu-id="c87e1-163">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c87e1-163">dateTimeOffset</span></span>|<span data-ttu-id="c87e1-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c87e1-164">Read only.</span></span> <span data-ttu-id="c87e1-165">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="c87e1-165">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="c87e1-166">assunto</span><span class="sxs-lookup"><span data-stu-id="c87e1-166">subject</span></span>|<span data-ttu-id="c87e1-167">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-167">string</span></span>| <span data-ttu-id="c87e1-168">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="c87e1-168">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="c87e1-169">body</span><span class="sxs-lookup"><span data-stu-id="c87e1-169">body</span></span>|[<span data-ttu-id="c87e1-170">itemBody</span><span class="sxs-lookup"><span data-stu-id="c87e1-170">itemBody</span></span>](itembody.md)|<span data-ttu-id="c87e1-171">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-171">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="c87e1-172">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="c87e1-172">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="c87e1-173">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="c87e1-173">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="c87e1-174">summary</span><span class="sxs-lookup"><span data-stu-id="c87e1-174">summary</span></span>|<span data-ttu-id="c87e1-175">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-175">string</span></span>| <span data-ttu-id="c87e1-176">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="c87e1-176">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="c87e1-177">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-177">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="c87e1-178">attachments</span><span class="sxs-lookup"><span data-stu-id="c87e1-178">attachments</span></span>|<span data-ttu-id="c87e1-179">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c87e1-179">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="c87e1-180">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="c87e1-180">Attached files.</span></span> <span data-ttu-id="c87e1-181">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="c87e1-181">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="c87e1-182">mentions</span><span class="sxs-lookup"><span data-stu-id="c87e1-182">mentions</span></span>|<span data-ttu-id="c87e1-183">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="c87e1-183">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="c87e1-184">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-184">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="c87e1-185">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="c87e1-185">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="c87e1-186">importância</span><span class="sxs-lookup"><span data-stu-id="c87e1-186">importance</span></span>| <span data-ttu-id="c87e1-187">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-187">string</span></span> | <span data-ttu-id="c87e1-188">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c87e1-188">The importance of the chat message.</span></span> <span data-ttu-id="c87e1-189">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="c87e1-189">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="c87e1-190">policyViolation</span><span class="sxs-lookup"><span data-stu-id="c87e1-190">policyViolation</span></span> | [<span data-ttu-id="c87e1-191">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="c87e1-191">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="c87e1-192">Define as propriedades de uma violação de política definida por um aplicativo DLP (prevenção de perda de dados).</span><span class="sxs-lookup"><span data-stu-id="c87e1-192">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="c87e1-193">localidade</span><span class="sxs-lookup"><span data-stu-id="c87e1-193">locale</span></span>|<span data-ttu-id="c87e1-194">string</span><span class="sxs-lookup"><span data-stu-id="c87e1-194">string</span></span>|<span data-ttu-id="c87e1-195">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c87e1-195">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c87e1-196">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c87e1-196">JSON representation</span></span>

<span data-ttu-id="c87e1-197">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c87e1-197">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "mentions",
    "subject",
    "summary",
    "policyViolation",
    "locale"
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
  "policyViolation": {"@odata.type": "microsoft.graph.chatMessagePolicyViolation"},
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
  "suppressions": []
}
-->
