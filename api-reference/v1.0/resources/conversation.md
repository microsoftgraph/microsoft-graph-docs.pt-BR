---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 4c34f6f0d55cb27e5ce7f5f2ba6459cfbb4d5291
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029593"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="48f2b-104">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="48f2b-104">conversation resource type</span></span>

<span data-ttu-id="48f2b-p102">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="48f2b-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="48f2b-107">Esse recurso oferece suporte à assinatura de [alteração de notificações](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="48f2b-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="48f2b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="48f2b-108">Methods</span></span>

| <span data-ttu-id="48f2b-109">Método</span><span class="sxs-lookup"><span data-stu-id="48f2b-109">Method</span></span>       | <span data-ttu-id="48f2b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="48f2b-110">Return Type</span></span>  |<span data-ttu-id="48f2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f2b-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="48f2b-112">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="48f2b-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="48f2b-113">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="48f2b-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="48f2b-114">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="48f2b-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="48f2b-115">Create</span><span class="sxs-lookup"><span data-stu-id="48f2b-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="48f2b-116">conversation</span><span class="sxs-lookup"><span data-stu-id="48f2b-116">conversation</span></span>](conversation.md)| <span data-ttu-id="48f2b-117">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="48f2b-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="48f2b-118">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="48f2b-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="48f2b-119">conversation</span><span class="sxs-lookup"><span data-stu-id="48f2b-119">conversation</span></span>](conversation.md) |<span data-ttu-id="48f2b-120">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="48f2b-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="48f2b-121">Delete</span><span class="sxs-lookup"><span data-stu-id="48f2b-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="48f2b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48f2b-122">None</span></span> |<span data-ttu-id="48f2b-123">Excluir objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="48f2b-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="48f2b-124">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="48f2b-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="48f2b-125">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="48f2b-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="48f2b-126">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="48f2b-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="48f2b-127">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="48f2b-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="48f2b-128">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="48f2b-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="48f2b-129">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="48f2b-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="48f2b-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48f2b-130">Properties</span></span>
| <span data-ttu-id="48f2b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48f2b-131">Property</span></span>     | <span data-ttu-id="48f2b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f2b-132">Type</span></span>   |<span data-ttu-id="48f2b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f2b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f2b-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="48f2b-134">hasAttachments</span></span>|<span data-ttu-id="48f2b-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="48f2b-135">Boolean</span></span>|<span data-ttu-id="48f2b-136">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="48f2b-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="48f2b-137">id</span><span class="sxs-lookup"><span data-stu-id="48f2b-137">id</span></span>|<span data-ttu-id="48f2b-138">String</span><span class="sxs-lookup"><span data-stu-id="48f2b-138">String</span></span>|<span data-ttu-id="48f2b-p103">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="48f2b-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="48f2b-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="48f2b-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="48f2b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48f2b-142">DateTimeOffset</span></span>|<span data-ttu-id="48f2b-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="48f2b-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="48f2b-145">visualização</span><span class="sxs-lookup"><span data-stu-id="48f2b-145">preview</span></span>|<span data-ttu-id="48f2b-146">String</span><span class="sxs-lookup"><span data-stu-id="48f2b-146">String</span></span>|<span data-ttu-id="48f2b-147">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="48f2b-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="48f2b-148">topic</span><span class="sxs-lookup"><span data-stu-id="48f2b-148">topic</span></span>|<span data-ttu-id="48f2b-149">String</span><span class="sxs-lookup"><span data-stu-id="48f2b-149">String</span></span>|<span data-ttu-id="48f2b-p105">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="48f2b-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="48f2b-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="48f2b-152">uniqueSenders</span></span>|<span data-ttu-id="48f2b-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="48f2b-153">String collection</span></span>|<span data-ttu-id="48f2b-154">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="48f2b-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f2b-155">Relações</span><span class="sxs-lookup"><span data-stu-id="48f2b-155">Relationships</span></span>
| <span data-ttu-id="48f2b-156">Relação</span><span class="sxs-lookup"><span data-stu-id="48f2b-156">Relationship</span></span> | <span data-ttu-id="48f2b-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="48f2b-157">Type</span></span>   |<span data-ttu-id="48f2b-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="48f2b-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48f2b-159">threads</span><span class="sxs-lookup"><span data-stu-id="48f2b-159">threads</span></span>|<span data-ttu-id="48f2b-160">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="48f2b-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="48f2b-p106">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="48f2b-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48f2b-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48f2b-165">JSON representation</span></span>

<span data-ttu-id="48f2b-166">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="48f2b-166">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversation",
  "@odata.annotations": [
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"],

  "threads": [{"@odata.type": "microsoft.graph.conversationThread"}]
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
