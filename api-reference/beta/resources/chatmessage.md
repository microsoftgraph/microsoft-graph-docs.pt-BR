---
title: tipo de recurso de chatMessage
description: Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de canal. A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: ad381102f7e93a4dcccd7b68435d0687ed6b4837
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855988"
---
# <a name="chatmessage-resource-type"></a><span data-ttu-id="e1a5b-104">tipo de recurso de chatMessage</span><span class="sxs-lookup"><span data-stu-id="e1a5b-104">chatMessage resource type</span></span>

> <span data-ttu-id="e1a5b-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1a5b-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1a5b-107">Representa uma mensagem de bate-papo individuais dentro de uma entidade de bate-papo ou de [canal](channel.md) .</span><span class="sxs-lookup"><span data-stu-id="e1a5b-107">Represents an individual chat message within a [channel](channel.md) or chat entity.</span></span> <span data-ttu-id="e1a5b-108">A mensagem pode ser uma mensagem de raiz ou a parte de um segmento que é definido pela propriedade **replyToId** na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-108">The message can be an root message or part of a thread that is defined by the **replyToId** property in the message.</span></span>

## <a name="methods"></a><span data-ttu-id="e1a5b-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="e1a5b-109">Methods</span></span>

| <span data-ttu-id="e1a5b-110">Método</span><span class="sxs-lookup"><span data-stu-id="e1a5b-110">Method</span></span>       | <span data-ttu-id="e1a5b-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e1a5b-111">Return Type</span></span>  |<span data-ttu-id="e1a5b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a5b-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1a5b-113">Mensagens de canal de lista</span><span class="sxs-lookup"><span data-stu-id="e1a5b-113">List Channel messages</span></span>](../api/channel-list-messages.md) | <span data-ttu-id="e1a5b-114">coleção [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-114">[chatmessage](chatmessage.md) collection</span></span> | <span data-ttu-id="e1a5b-115">Obter a lista de todas as mensagens de raiz em um canal.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-115">Get the list of all root messages in a channel.</span></span>|
|[<span data-ttu-id="e1a5b-116">Mensagem de canal Get</span><span class="sxs-lookup"><span data-stu-id="e1a5b-116">Get Channel message</span></span>](../api/channel-get-message.md) | [<span data-ttu-id="e1a5b-117">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e1a5b-117">chatmessage</span></span>](chatmessage.md) | <span data-ttu-id="e1a5b-118">Obtenha uma mensagem de raiz única de um canal.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-118">Get a single root message from a channel.</span></span>|
|[<span data-ttu-id="e1a5b-119">Lista de respostas a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="e1a5b-119">List replies to a message</span></span>](../api/channel-list-messagereplies.md) | <span data-ttu-id="e1a5b-120">coleção [chatmessage](chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-120">[chatmessage](chatmessage.md) collection</span></span>| <span data-ttu-id="e1a5b-121">Obter a lista de todas as respostas a uma mensagem no canal.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-121">Get the list of all replies to a message in channel.</span></span>|
|[<span data-ttu-id="e1a5b-122">Obtenha uma resposta a uma mensagem</span><span class="sxs-lookup"><span data-stu-id="e1a5b-122">Get a reply to a message</span></span>](../api/channel-get-messagereply.md) | [<span data-ttu-id="e1a5b-123">chatmessage</span><span class="sxs-lookup"><span data-stu-id="e1a5b-123">chatmessage</span></span>](chatmessage.md)| <span data-ttu-id="e1a5b-124">Obtenha uma única resposta a uma mensagem em um canal.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-124">Get a single reply to a message in a channel.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1a5b-125">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1a5b-125">Properties</span></span>
| <span data-ttu-id="e1a5b-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1a5b-126">Property</span></span>     | <span data-ttu-id="e1a5b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1a5b-127">Type</span></span>   |<span data-ttu-id="e1a5b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1a5b-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1a5b-129">id</span><span class="sxs-lookup"><span data-stu-id="e1a5b-129">id</span></span>|<span data-ttu-id="e1a5b-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1a5b-130">String</span></span>| <span data-ttu-id="e1a5b-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-131">Read-only.</span></span> <span data-ttu-id="e1a5b-132">Identificação exclusiva da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-132">Unique ID of the message.</span></span>|
|<span data-ttu-id="e1a5b-133">replyToId</span><span class="sxs-lookup"><span data-stu-id="e1a5b-133">replyToId</span></span>| <span data-ttu-id="e1a5b-134">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-134">string</span></span> | <span data-ttu-id="e1a5b-135">ID da mensagem pai mensagem/raiz do thread</span><span class="sxs-lookup"><span data-stu-id="e1a5b-135">Id of the parent message/root message of the thread</span></span> |
|<span data-ttu-id="e1a5b-136">from</span><span class="sxs-lookup"><span data-stu-id="e1a5b-136">from</span></span>|[<span data-ttu-id="e1a5b-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="e1a5b-137">identitySet</span></span>](identityset.md)| <span data-ttu-id="e1a5b-138">Detalhes do remetente da mensagem</span><span class="sxs-lookup"><span data-stu-id="e1a5b-138">Details of the sender of the message</span></span>|
|<span data-ttu-id="e1a5b-139">etag</span><span class="sxs-lookup"><span data-stu-id="e1a5b-139">etag</span></span>| <span data-ttu-id="e1a5b-140">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-140">string</span></span> | <span data-ttu-id="e1a5b-141">Número de versão da mensagem</span><span class="sxs-lookup"><span data-stu-id="e1a5b-141">Version number of the message</span></span> |
|<span data-ttu-id="e1a5b-142">messageType</span><span class="sxs-lookup"><span data-stu-id="e1a5b-142">messageType</span></span>|<span data-ttu-id="e1a5b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1a5b-143">String</span></span>|<span data-ttu-id="e1a5b-144">Os valores de tipo de mensagem, atual com suporte são: mensagem, chatEvent, digitando</span><span class="sxs-lookup"><span data-stu-id="e1a5b-144">The type of message, current supported values are: message, chatEvent, Typing</span></span>|
|<span data-ttu-id="e1a5b-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a5b-145">createdDateTime</span></span>|<span data-ttu-id="e1a5b-146">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a5b-146">dateTimeOffset</span></span>|<span data-ttu-id="e1a5b-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-147">Read only.</span></span> <span data-ttu-id="e1a5b-148">Carimbo de hora de quando a mensagem foi criada</span><span class="sxs-lookup"><span data-stu-id="e1a5b-148">Timestamp of when the message was created</span></span>|
|<span data-ttu-id="e1a5b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a5b-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e1a5b-150">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a5b-150">dateTimeOffset</span></span>|<span data-ttu-id="e1a5b-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-151">Read only.</span></span> <span data-ttu-id="e1a5b-152">Carimbo de hora de quando a mensagem foi editado/atualizado</span><span class="sxs-lookup"><span data-stu-id="e1a5b-152">Timestamp of when the message was edited/updated</span></span>|
|<span data-ttu-id="e1a5b-153">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e1a5b-153">isDeleted</span></span>|<span data-ttu-id="e1a5b-154">booliano</span><span class="sxs-lookup"><span data-stu-id="e1a5b-154">boolean</span></span>|<span data-ttu-id="e1a5b-155">Representa se uma mensagem tiver sido excluída soft</span><span class="sxs-lookup"><span data-stu-id="e1a5b-155">Represents if a message has been soft deleted</span></span>|
|<span data-ttu-id="e1a5b-156">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1a5b-156">deletedDateTime</span></span>|<span data-ttu-id="e1a5b-157">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1a5b-157">dateTimeOffset</span></span>|<span data-ttu-id="e1a5b-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-158">Read only.</span></span> <span data-ttu-id="e1a5b-159">Carimbo de hora em que a mensagem foi excluída.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-159">Timestamp at which the message was deleted</span></span> |
|<span data-ttu-id="e1a5b-160">subject</span><span class="sxs-lookup"><span data-stu-id="e1a5b-160">subject</span></span>|<span data-ttu-id="e1a5b-161">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-161">string</span></span>|<span data-ttu-id="e1a5b-162">Linha de assunto da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-162">Message subject line.</span></span> <span data-ttu-id="e1a5b-163">Opcional</span><span class="sxs-lookup"><span data-stu-id="e1a5b-163">Optional</span></span>|
|<span data-ttu-id="e1a5b-164">body</span><span class="sxs-lookup"><span data-stu-id="e1a5b-164">body</span></span>|[<span data-ttu-id="e1a5b-165">itemBody</span><span class="sxs-lookup"><span data-stu-id="e1a5b-165">itemBody</span></span>](itembody.md)|<span data-ttu-id="e1a5b-166">Representação em texto sem formatação/HTML do conteúdo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-166">Plaintext/HTML representation of the content of the message.</span></span> <span data-ttu-id="e1a5b-167">Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="e1a5b-167">Returns plain text by default, application can choose HTML as part of a query param</span></span>|
|<span data-ttu-id="e1a5b-168">Resumo</span><span class="sxs-lookup"><span data-stu-id="e1a5b-168">summary</span></span>|<span data-ttu-id="e1a5b-169">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-169">string</span></span>|<span data-ttu-id="e1a5b-170">Texto da mensagem que poderia ser usada para notificações por push e modos de exibição de resumo ou regressivo queda de modos de exibição de resumo</span><span class="sxs-lookup"><span data-stu-id="e1a5b-170">Summary text of the message that could be used for push notifications and summary views or fall back views</span></span>|
|<span data-ttu-id="e1a5b-171">menções</span><span class="sxs-lookup"><span data-stu-id="e1a5b-171">mentions</span></span>|<span data-ttu-id="e1a5b-172">coleção [chatMessageMention](chatmention.md)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-172">[chatMessageMention](chatmention.md) collection</span></span>| <span data-ttu-id="e1a5b-173">Lista de entidades mencionado na mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-173">List of entities mentioned in the message.</span></span> <span data-ttu-id="e1a5b-174">Suporta atualmente o usuário, bot, equipe, de canal</span><span class="sxs-lookup"><span data-stu-id="e1a5b-174">Currently supports user, bot, team, channel</span></span>|
|<span data-ttu-id="e1a5b-175">importance</span><span class="sxs-lookup"><span data-stu-id="e1a5b-175">importance</span></span>| <span data-ttu-id="e1a5b-176">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-176">string</span></span> | <span data-ttu-id="e1a5b-177">A importância da mensagem: Normal, alta</span><span class="sxs-lookup"><span data-stu-id="e1a5b-177">The importance of the message: Normal, High</span></span>|
|<span data-ttu-id="e1a5b-178">reações</span><span class="sxs-lookup"><span data-stu-id="e1a5b-178">reactions</span></span>| <span data-ttu-id="e1a5b-179">coleção [chatMessageReaction](chatreaction.md)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-179">[chatMessageReaction](chatreaction.md) collection</span></span> | <span data-ttu-id="e1a5b-180">Reações para esta mensagem (por exemplo,-Like)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-180">Reactions for this message (for example, Like)</span></span>|
|<span data-ttu-id="e1a5b-181">localidade</span><span class="sxs-lookup"><span data-stu-id="e1a5b-181">locale</span></span>|<span data-ttu-id="e1a5b-182">string</span><span class="sxs-lookup"><span data-stu-id="e1a5b-182">string</span></span>|<span data-ttu-id="e1a5b-183">Localidade da mensagem definida pelo cliente</span><span class="sxs-lookup"><span data-stu-id="e1a5b-183">Locale of the message set by the client</span></span>|
|<span data-ttu-id="e1a5b-184">attachments</span><span class="sxs-lookup"><span data-stu-id="e1a5b-184">attachments</span></span>|<span data-ttu-id="e1a5b-185">coleção [chatMessageAttachment](chatattachment.md)</span><span class="sxs-lookup"><span data-stu-id="e1a5b-185">[chatMessageAttachment](chatattachment.md) collection</span></span> |<span data-ttu-id="e1a5b-186">Arquivos anexados</span><span class="sxs-lookup"><span data-stu-id="e1a5b-186">Attached files</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e1a5b-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1a5b-187">JSON representation</span></span>

<span data-ttu-id="e1a5b-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1a5b-188">The following is a JSON representation of the resource.</span></span>

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
