---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread que é definido pela propriedade **replyToId** na mensagem de chat.
doc_type: resourcePageType
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 16bcd870ba8d4b97b5951fefab538eb6b6669635
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932574"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="c90d2-104">Tipo de recurso chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-104">chatMessage resource type</span></span>

<span data-ttu-id="c90d2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c90d2-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c90d2-106">Representa uma mensagem de chat individual dentro de um [canal](./channel.md) ou em um [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true)(na versão beta).</span><span class="sxs-lookup"><span data-stu-id="c90d2-106">Represents an individual chat message within a [channel](./channel.md) or (in beta) [chat](/graph/api/resources/chat?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="c90d2-107">A mensagem de chat pode ser uma mensagem de chat raiz ou parte de um thread de resposta definido pela propriedade **replyToId** na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-107">The chat message can be a root chat message or part of a reply thread that is defined by the **replyToId** property in the chat message.</span></span>

## <a name="methods"></a><span data-ttu-id="c90d2-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c90d2-108">Methods</span></span>

| <span data-ttu-id="c90d2-109">Método</span><span class="sxs-lookup"><span data-stu-id="c90d2-109">Method</span></span>       | <span data-ttu-id="c90d2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c90d2-110">Return Type</span></span>  |<span data-ttu-id="c90d2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90d2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c90d2-112">**Mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="c90d2-112">**Channel messages**</span></span>| | |
|[<span data-ttu-id="c90d2-113">Listar canal chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-113">List channel chatMessage</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="c90d2-114">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="c90d2-114">[chatMessage](chatmessage.md) collection</span></span> | <span data-ttu-id="c90d2-115">Lista de todas as mensagens de chat raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-115">List of all root chat messages in a channel.</span></span>|
|[<span data-ttu-id="c90d2-116">Obter chatMessages em um Delta de canal</span><span class="sxs-lookup"><span data-stu-id="c90d2-116">Get chatMessages in a channel delta</span></span>](../api/chatmessage-delta.md)  | [<span data-ttu-id="c90d2-117">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-117">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c90d2-118">Obter mensagens de chat incrementais em um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-118">Get incremental chat messages in a channel.</span></span> |
|[<span data-ttu-id="c90d2-119">Criar assinatura para novas mensagens de canal</span><span class="sxs-lookup"><span data-stu-id="c90d2-119">Create subscription for new channel messages</span></span>](../api/subscription-post-subscriptions.md) | [<span data-ttu-id="c90d2-120">subscription</span><span class="sxs-lookup"><span data-stu-id="c90d2-120">subscription</span></span>](subscription.md) | <span data-ttu-id="c90d2-121">Ouvir mensagens de canal novas e editadas e reações para elas.</span><span class="sxs-lookup"><span data-stu-id="c90d2-121">Listen for new and edited channel messages, and reactions to them.</span></span> |
|[<span data-ttu-id="c90d2-122">Obter canal chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-122">Get channel chatMessage</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="c90d2-123">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-123">chatMessage</span></span>](chatmessage.md) | <span data-ttu-id="c90d2-124">Obtenha uma única mensagem de chat raiz de um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-124">Get a single root chat message from a channel.</span></span>|
|[<span data-ttu-id="c90d2-125">Criar chatMessage em um canal</span><span class="sxs-lookup"><span data-stu-id="c90d2-125">Create chatMessage in a channel</span></span>](../api/channel-post-message.md) | [<span data-ttu-id="c90d2-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-126">chatMessage</span></span>](../resources/chatmessage.md) | <span data-ttu-id="c90d2-127">Envie uma mensagem para um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-127">Send a message to a channel.</span></span> |
|[<span data-ttu-id="c90d2-128">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-128">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="c90d2-129">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-129">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c90d2-130">Atualizar a propriedade **policyViolation** de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-130">Update the **policyViolation** property of a chat message.</span></span>|
|<span data-ttu-id="c90d2-131">**Respostas de mensagens de canal**</span><span class="sxs-lookup"><span data-stu-id="c90d2-131">**Channel message replies**</span></span>| | |
|[<span data-ttu-id="c90d2-132">Listar respostas a um chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-132">List replies to a chatMessage</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="c90d2-133">[chatMessage](chatmessage.md) collection</span><span class="sxs-lookup"><span data-stu-id="c90d2-133">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="c90d2-134">Lista de todas as respostas para uma mensagem de chat no canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-134">List of all replies to a chat message in channel.</span></span>|
|[<span data-ttu-id="c90d2-135">Obter uma resposta para um chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-135">Get a reply to a chatMessage</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="c90d2-136">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-136">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c90d2-137">Obter uma única resposta para uma mensagem de chat em um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-137">Get a single reply to a chat message in a channel.</span></span>|
|[<span data-ttu-id="c90d2-138">Responder a um chat em um canal</span><span class="sxs-lookup"><span data-stu-id="c90d2-138">Reply to a chatMessage in a channel</span></span>](../api/channel-post-messagereply.md) | [<span data-ttu-id="c90d2-139">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-139">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c90d2-140">Responder a uma mensagem de chat existente em um canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-140">Reply to an existing chat message in a channel.</span></span>|
|[<span data-ttu-id="c90d2-141">Atualizar chat</span><span class="sxs-lookup"><span data-stu-id="c90d2-141">Update chatMessage</span></span>](../api/chatmessage-update.md)|[<span data-ttu-id="c90d2-142">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c90d2-142">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="c90d2-143">Atualizar a propriedade **policyViolation** de uma mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-143">Update the **policyViolation** property of a chat message.</span></span>|

## <a name="properties"></a><span data-ttu-id="c90d2-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c90d2-144">Properties</span></span>

| <span data-ttu-id="c90d2-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c90d2-145">Property</span></span>   | <span data-ttu-id="c90d2-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="c90d2-146">Type</span></span> |<span data-ttu-id="c90d2-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="c90d2-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c90d2-148">id</span><span class="sxs-lookup"><span data-stu-id="c90d2-148">id</span></span>|<span data-ttu-id="c90d2-149">String</span><span class="sxs-lookup"><span data-stu-id="c90d2-149">String</span></span>| <span data-ttu-id="c90d2-150">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-150">Read-only.</span></span> <span data-ttu-id="c90d2-151">ID exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="c90d2-151">Unique Id of the message.</span></span>|
|<span data-ttu-id="c90d2-152">replyToId</span><span class="sxs-lookup"><span data-stu-id="c90d2-152">replyToId</span></span>| <span data-ttu-id="c90d2-153">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-153">string</span></span> | <span data-ttu-id="c90d2-154">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-154">Read-only.</span></span> <span data-ttu-id="c90d2-155">ID da mensagem de chat pai ou mensagem de chat raiz do thread.</span><span class="sxs-lookup"><span data-stu-id="c90d2-155">Id of the parent chat message or root chat message of the thread.</span></span> <span data-ttu-id="c90d2-156">(Aplicável somente a mensagens de chat em canais que não sejam chats)</span><span class="sxs-lookup"><span data-stu-id="c90d2-156">(Only applies to chat messages in channels not chats)</span></span> |
|<span data-ttu-id="c90d2-157">from</span><span class="sxs-lookup"><span data-stu-id="c90d2-157">from</span></span>|[<span data-ttu-id="c90d2-158">identitySet</span><span class="sxs-lookup"><span data-stu-id="c90d2-158">identitySet</span></span>](identityset.md)| <span data-ttu-id="c90d2-159">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-159">Read only.</span></span> <span data-ttu-id="c90d2-160">Detalhes do remetente da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-160">Details of the sender of the chat message.</span></span>|
|<span data-ttu-id="c90d2-161">etag</span><span class="sxs-lookup"><span data-stu-id="c90d2-161">etag</span></span>| <span data-ttu-id="c90d2-162">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-162">string</span></span> | <span data-ttu-id="c90d2-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-163">Read-only.</span></span> <span data-ttu-id="c90d2-164">Número de versão da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-164">Version number of the chat message.</span></span> |
|<span data-ttu-id="c90d2-165">messageType</span><span class="sxs-lookup"><span data-stu-id="c90d2-165">messageType</span></span>|<span data-ttu-id="c90d2-166">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-166">string</span></span>|<span data-ttu-id="c90d2-167">O tipo de mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-167">The type of chat message.</span></span> <span data-ttu-id="c90d2-168">Os valores possíveis são: `message` .</span><span class="sxs-lookup"><span data-stu-id="c90d2-168">The possible values are: `message`.</span></span>|
|<span data-ttu-id="c90d2-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d2-169">createdDateTime</span></span>|<span data-ttu-id="c90d2-170">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d2-170">dateTimeOffset</span></span>|<span data-ttu-id="c90d2-171">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-171">Read only.</span></span> <span data-ttu-id="c90d2-172">Carimbo de data/hora de quando a mensagem de chat foi criada.</span><span class="sxs-lookup"><span data-stu-id="c90d2-172">Timestamp of when the chat message was created.</span></span>|
|<span data-ttu-id="c90d2-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d2-173">lastModifiedDateTime</span></span>|<span data-ttu-id="c90d2-174">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d2-174">dateTimeOffset</span></span>|<span data-ttu-id="c90d2-175">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-175">Read only.</span></span> <span data-ttu-id="c90d2-176">Carimbo de data/hora em que a mensagem de chat é criada (configuração inicial) ou editada, incluindo quando uma reação é adicionada ou removida.</span><span class="sxs-lookup"><span data-stu-id="c90d2-176">Timestamp when the chat message is created (initial setting) or edited, including when a reaction is added or removed.</span></span> |
|<span data-ttu-id="c90d2-177">lastEditedDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d2-177">lastEditedDateTime</span></span>|<span data-ttu-id="c90d2-178">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d2-178">dateTimeOffset</span></span>|<span data-ttu-id="c90d2-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-179">Read only.</span></span> <span data-ttu-id="c90d2-180">Carimbo de data/hora em que foram feitas edições na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-180">Timestamp when edits to the chat message were made.</span></span> <span data-ttu-id="c90d2-181">Dispara um sinalizador "editado" na interface do usuário do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c90d2-181">Triggers an "Edited" flag in the Microsoft Teams UI.</span></span> <span data-ttu-id="c90d2-182">Se não for feita nenhuma edição, o valor será `null` .</span><span class="sxs-lookup"><span data-stu-id="c90d2-182">If no edits are made the value is `null`.</span></span>|
|<span data-ttu-id="c90d2-183">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c90d2-183">deletedDateTime</span></span>|<span data-ttu-id="c90d2-184">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c90d2-184">dateTimeOffset</span></span>|<span data-ttu-id="c90d2-185">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c90d2-185">Read only.</span></span> <span data-ttu-id="c90d2-186">Carimbo de data/hora em que a mensagem de chat foi excluída ou nula se não for excluída.</span><span class="sxs-lookup"><span data-stu-id="c90d2-186">Timestamp at which the chat message was deleted, or null if not deleted.</span></span> |
|<span data-ttu-id="c90d2-187">assunto</span><span class="sxs-lookup"><span data-stu-id="c90d2-187">subject</span></span>|<span data-ttu-id="c90d2-188">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-188">string</span></span>| <span data-ttu-id="c90d2-189">O assunto da mensagem de chat, em texto não criptografado.</span><span class="sxs-lookup"><span data-stu-id="c90d2-189">The subject of the chat message, in plaintext.</span></span>|
|<span data-ttu-id="c90d2-190">body</span><span class="sxs-lookup"><span data-stu-id="c90d2-190">body</span></span>|[<span data-ttu-id="c90d2-191">itemBody</span><span class="sxs-lookup"><span data-stu-id="c90d2-191">itemBody</span></span>](itembody.md)|<span data-ttu-id="c90d2-192">Representação de texto não criptografado/HTML do conteúdo da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-192">Plaintext/HTML representation of the content of the chat message.</span></span> <span data-ttu-id="c90d2-193">A representação é especificada pelo contentType dentro do corpo.</span><span class="sxs-lookup"><span data-stu-id="c90d2-193">Representation is specified by the contentType inside the body.</span></span> <span data-ttu-id="c90d2-194">O conteúdo estará sempre em HTML se a mensagem de chat contiver um [chatMessageMention](chatmessagemention.md).</span><span class="sxs-lookup"><span data-stu-id="c90d2-194">The content is always in HTML if the chat message contains a [chatMessageMention](chatmessagemention.md).</span></span> |
|<span data-ttu-id="c90d2-195">summary</span><span class="sxs-lookup"><span data-stu-id="c90d2-195">summary</span></span>|<span data-ttu-id="c90d2-196">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c90d2-196">string</span></span>| <span data-ttu-id="c90d2-197">Texto de resumo da mensagem de chat que pode ser usado para notificações por push e visualizações de resumo ou exibições de retorno.</span><span class="sxs-lookup"><span data-stu-id="c90d2-197">Summary text of the chat message that could be used for push notifications and summary views or fall back views.</span></span> <span data-ttu-id="c90d2-198">Aplica-se somente a mensagens de chat de canal, e não a mensagens de chat em um chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-198">Only applies to channel chat messages, not chat messages in a chat.</span></span> |
|<span data-ttu-id="c90d2-199">attachments</span><span class="sxs-lookup"><span data-stu-id="c90d2-199">attachments</span></span>|<span data-ttu-id="c90d2-200">[chatMessageAttachment](chatmessageattachment.md) collection</span><span class="sxs-lookup"><span data-stu-id="c90d2-200">[chatMessageAttachment](chatmessageattachment.md) collection</span></span> |<span data-ttu-id="c90d2-201">Arquivos anexos.</span><span class="sxs-lookup"><span data-stu-id="c90d2-201">Attached files.</span></span> <span data-ttu-id="c90d2-202">No momento, os anexos são somente leitura, não há suporte para o envio de anexos.</span><span class="sxs-lookup"><span data-stu-id="c90d2-202">Attachments are currently read-only – sending attachments is not supported.</span></span> |
|<span data-ttu-id="c90d2-203">mentions</span><span class="sxs-lookup"><span data-stu-id="c90d2-203">mentions</span></span>|<span data-ttu-id="c90d2-204">[chatMessageMention](chatmessagemention.md) collection</span><span class="sxs-lookup"><span data-stu-id="c90d2-204">[chatMessageMention](chatmessagemention.md) collection</span></span>| <span data-ttu-id="c90d2-205">Lista de entidades mencionadas na mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-205">List of entities mentioned in the chat message.</span></span> <span data-ttu-id="c90d2-206">Atualmente, dá suporte a usuário, bot, equipe, canal.</span><span class="sxs-lookup"><span data-stu-id="c90d2-206">Currently supports user, bot, team, channel.</span></span>|
|<span data-ttu-id="c90d2-207">importância</span><span class="sxs-lookup"><span data-stu-id="c90d2-207">importance</span></span>| <span data-ttu-id="c90d2-208">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-208">string</span></span> | <span data-ttu-id="c90d2-209">A importância da mensagem de chat.</span><span class="sxs-lookup"><span data-stu-id="c90d2-209">The importance of the chat message.</span></span> <span data-ttu-id="c90d2-210">Os valores possíveis são: `normal`, `high`, `urgent`.</span><span class="sxs-lookup"><span data-stu-id="c90d2-210">The possible values are: `normal`, `high`, `urgent`.</span></span>|
| <span data-ttu-id="c90d2-211">policyViolation</span><span class="sxs-lookup"><span data-stu-id="c90d2-211">policyViolation</span></span> | [<span data-ttu-id="c90d2-212">chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="c90d2-212">chatMessagePolicyViolation</span></span>](../resources/chatmessagepolicyviolation.md) |<span data-ttu-id="c90d2-213">Define as propriedades de uma violação de política definida por um aplicativo DLP (prevenção de perda de dados).</span><span class="sxs-lookup"><span data-stu-id="c90d2-213">Defines the properties of a policy violation set by a data loss prevention (DLP) application.</span></span>|
|<span data-ttu-id="c90d2-214">localidade</span><span class="sxs-lookup"><span data-stu-id="c90d2-214">locale</span></span>|<span data-ttu-id="c90d2-215">string</span><span class="sxs-lookup"><span data-stu-id="c90d2-215">string</span></span>|<span data-ttu-id="c90d2-216">Local da mensagem de chat definida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c90d2-216">Locale of the chat message set by the client.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c90d2-217">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c90d2-217">JSON representation</span></span>

<span data-ttu-id="c90d2-218">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c90d2-218">The following is a JSON representation of the resource.</span></span>

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
