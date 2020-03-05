---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: f6e1a7078616e0c02bf300503c94f780ced44484
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507405"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="c452c-104">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="c452c-104">conversation resource type</span></span>

<span data-ttu-id="c452c-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c452c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c452c-p102">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="c452c-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="c452c-108">Esse recurso oferece suporte à assinatura de [alteração de notificações](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="c452c-108">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="c452c-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c452c-109">Methods</span></span>

| <span data-ttu-id="c452c-110">Método</span><span class="sxs-lookup"><span data-stu-id="c452c-110">Method</span></span>       | <span data-ttu-id="c452c-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c452c-111">Return Type</span></span>  |<span data-ttu-id="c452c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c452c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c452c-113">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="c452c-113">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="c452c-114">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="c452c-114">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="c452c-115">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="c452c-115">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="c452c-116">Create</span><span class="sxs-lookup"><span data-stu-id="c452c-116">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="c452c-117">conversation</span><span class="sxs-lookup"><span data-stu-id="c452c-117">conversation</span></span>](conversation.md)| <span data-ttu-id="c452c-118">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="c452c-118">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="c452c-119">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="c452c-119">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="c452c-120">conversation</span><span class="sxs-lookup"><span data-stu-id="c452c-120">conversation</span></span>](conversation.md) |<span data-ttu-id="c452c-121">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c452c-121">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="c452c-122">Delete</span><span class="sxs-lookup"><span data-stu-id="c452c-122">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="c452c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c452c-123">None</span></span> |<span data-ttu-id="c452c-124">Excluir objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c452c-124">Delete conversation object.</span></span> |
|[<span data-ttu-id="c452c-125">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="c452c-125">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="c452c-126">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c452c-126">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c452c-127">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="c452c-127">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="c452c-128">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="c452c-128">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="c452c-129">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c452c-129">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c452c-130">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="c452c-130">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="c452c-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c452c-131">Properties</span></span>
| <span data-ttu-id="c452c-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c452c-132">Property</span></span>     | <span data-ttu-id="c452c-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c452c-133">Type</span></span>   |<span data-ttu-id="c452c-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c452c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c452c-135">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c452c-135">hasAttachments</span></span>|<span data-ttu-id="c452c-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="c452c-136">Boolean</span></span>|<span data-ttu-id="c452c-137">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="c452c-137">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="c452c-138">id</span><span class="sxs-lookup"><span data-stu-id="c452c-138">id</span></span>|<span data-ttu-id="c452c-139">String</span><span class="sxs-lookup"><span data-stu-id="c452c-139">String</span></span>|<span data-ttu-id="c452c-p103">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c452c-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c452c-142">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c452c-142">lastDeliveredDateTime</span></span>|<span data-ttu-id="c452c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c452c-143">DateTimeOffset</span></span>|<span data-ttu-id="c452c-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c452c-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c452c-146">visualização</span><span class="sxs-lookup"><span data-stu-id="c452c-146">preview</span></span>|<span data-ttu-id="c452c-147">String</span><span class="sxs-lookup"><span data-stu-id="c452c-147">String</span></span>|<span data-ttu-id="c452c-148">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="c452c-148">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c452c-149">topic</span><span class="sxs-lookup"><span data-stu-id="c452c-149">topic</span></span>|<span data-ttu-id="c452c-150">String</span><span class="sxs-lookup"><span data-stu-id="c452c-150">String</span></span>|<span data-ttu-id="c452c-p105">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="c452c-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="c452c-153">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c452c-153">uniqueSenders</span></span>|<span data-ttu-id="c452c-154">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c452c-154">String collection</span></span>|<span data-ttu-id="c452c-155">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="c452c-155">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c452c-156">Relações</span><span class="sxs-lookup"><span data-stu-id="c452c-156">Relationships</span></span>
| <span data-ttu-id="c452c-157">Relação</span><span class="sxs-lookup"><span data-stu-id="c452c-157">Relationship</span></span> | <span data-ttu-id="c452c-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="c452c-158">Type</span></span>   |<span data-ttu-id="c452c-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c452c-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c452c-160">threads</span><span class="sxs-lookup"><span data-stu-id="c452c-160">threads</span></span>|<span data-ttu-id="c452c-161">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c452c-161">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="c452c-p106">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c452c-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c452c-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c452c-166">JSON representation</span></span>

<span data-ttu-id="c452c-167">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c452c-167">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
