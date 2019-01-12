---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5cacad2b9539c398251ffd07899df7beb3c2f378
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991437"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="120b1-104">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="120b1-104">conversation resource type</span></span>

> <span data-ttu-id="120b1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="120b1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="120b1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="120b1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="120b1-p103">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="120b1-p103">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="120b1-109">Este recurso oferece suporte a assinatura de [notificações de alteração](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="120b1-109">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="120b1-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="120b1-110">Methods</span></span>

| <span data-ttu-id="120b1-111">Método</span><span class="sxs-lookup"><span data-stu-id="120b1-111">Method</span></span>       | <span data-ttu-id="120b1-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="120b1-112">Return Type</span></span>  |<span data-ttu-id="120b1-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="120b1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="120b1-114">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="120b1-114">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="120b1-115">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="120b1-115">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="120b1-116">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="120b1-116">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="120b1-117">Create</span><span class="sxs-lookup"><span data-stu-id="120b1-117">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="120b1-118">conversation</span><span class="sxs-lookup"><span data-stu-id="120b1-118">conversation</span></span>](conversation.md)| <span data-ttu-id="120b1-119">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="120b1-119">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="120b1-120">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="120b1-120">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="120b1-121">conversation</span><span class="sxs-lookup"><span data-stu-id="120b1-121">conversation</span></span>](conversation.md) |<span data-ttu-id="120b1-122">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="120b1-122">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="120b1-123">Delete</span><span class="sxs-lookup"><span data-stu-id="120b1-123">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="120b1-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="120b1-124">None</span></span> |<span data-ttu-id="120b1-125">Exclua um objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="120b1-125">Delete conversation object.</span></span> |
|[<span data-ttu-id="120b1-126">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="120b1-126">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="120b1-127">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="120b1-127">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="120b1-128">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="120b1-128">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="120b1-129">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="120b1-129">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="120b1-130">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="120b1-130">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="120b1-131">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="120b1-131">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="120b1-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="120b1-132">Properties</span></span>
| <span data-ttu-id="120b1-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="120b1-133">Property</span></span>     | <span data-ttu-id="120b1-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="120b1-134">Type</span></span>   |<span data-ttu-id="120b1-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="120b1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="120b1-136">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="120b1-136">hasAttachments</span></span>|<span data-ttu-id="120b1-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="120b1-137">Boolean</span></span>|<span data-ttu-id="120b1-138">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="120b1-138">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="120b1-139">id</span><span class="sxs-lookup"><span data-stu-id="120b1-139">id</span></span>|<span data-ttu-id="120b1-140">String</span><span class="sxs-lookup"><span data-stu-id="120b1-140">String</span></span>|<span data-ttu-id="120b1-p104">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="120b1-p104">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="120b1-143">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="120b1-143">lastDeliveredDateTime</span></span>|<span data-ttu-id="120b1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="120b1-144">DateTimeOffset</span></span>|<span data-ttu-id="120b1-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="120b1-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="120b1-147">visualização</span><span class="sxs-lookup"><span data-stu-id="120b1-147">preview</span></span>|<span data-ttu-id="120b1-148">String</span><span class="sxs-lookup"><span data-stu-id="120b1-148">String</span></span>|<span data-ttu-id="120b1-149">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="120b1-149">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="120b1-150">topic</span><span class="sxs-lookup"><span data-stu-id="120b1-150">topic</span></span>|<span data-ttu-id="120b1-151">String</span><span class="sxs-lookup"><span data-stu-id="120b1-151">String</span></span>|<span data-ttu-id="120b1-p106">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="120b1-p106">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="120b1-154">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="120b1-154">uniqueSenders</span></span>|<span data-ttu-id="120b1-155">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="120b1-155">String collection</span></span>|<span data-ttu-id="120b1-156">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="120b1-156">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="120b1-157">Relações</span><span class="sxs-lookup"><span data-stu-id="120b1-157">Relationships</span></span>
| <span data-ttu-id="120b1-158">Relação</span><span class="sxs-lookup"><span data-stu-id="120b1-158">Relationship</span></span> | <span data-ttu-id="120b1-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="120b1-159">Type</span></span>   |<span data-ttu-id="120b1-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="120b1-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="120b1-161">threads</span><span class="sxs-lookup"><span data-stu-id="120b1-161">threads</span></span>|<span data-ttu-id="120b1-162">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="120b1-162">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="120b1-p107">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="120b1-p107">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="120b1-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="120b1-167">JSON representation</span></span>

<span data-ttu-id="120b1-168">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="120b1-168">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
