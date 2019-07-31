---
title: tipo de recurso conversation
description: Uma conversa é uma coleção de threads e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 60add8177bcbf4f667f251dd853109bdef4db11b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973977"
---
# <a name="conversation-resource-type"></a><span data-ttu-id="c5431-104">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="c5431-104">conversation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5431-p102">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="c5431-p102">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="c5431-107">Esse recurso oferece suporte à assinatura de [alteração de notificações](/graph/webhooks).</span><span class="sxs-lookup"><span data-stu-id="c5431-107">This resource supports subscribing to [change notifications](/graph/webhooks).</span></span>

## <a name="methods"></a><span data-ttu-id="c5431-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c5431-108">Methods</span></span>

| <span data-ttu-id="c5431-109">Método</span><span class="sxs-lookup"><span data-stu-id="c5431-109">Method</span></span>       | <span data-ttu-id="c5431-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c5431-110">Return Type</span></span>  |<span data-ttu-id="c5431-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5431-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5431-112">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="c5431-112">List conversations</span></span>](../api/group-list-conversations.md) | <span data-ttu-id="c5431-113">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="c5431-113">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="c5431-114">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="c5431-114">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="c5431-115">Create</span><span class="sxs-lookup"><span data-stu-id="c5431-115">Create</span></span>](../api/group-post-conversations.md) |[<span data-ttu-id="c5431-116">conversation</span><span class="sxs-lookup"><span data-stu-id="c5431-116">conversation</span></span>](conversation.md)| <span data-ttu-id="c5431-117">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="c5431-117">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="c5431-118">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="c5431-118">Get conversation</span></span>](../api/conversation-get.md) | [<span data-ttu-id="c5431-119">conversation</span><span class="sxs-lookup"><span data-stu-id="c5431-119">conversation</span></span>](conversation.md) |<span data-ttu-id="c5431-120">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c5431-120">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="c5431-121">Delete</span><span class="sxs-lookup"><span data-stu-id="c5431-121">Delete</span></span>](../api/conversation-delete.md) | <span data-ttu-id="c5431-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5431-122">None</span></span> |<span data-ttu-id="c5431-123">Excluir objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c5431-123">Delete conversation object.</span></span> |
|[<span data-ttu-id="c5431-124">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="c5431-124">List conversation threads</span></span>](../api/conversation-list-threads.md) |<span data-ttu-id="c5431-125">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c5431-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c5431-126">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="c5431-126">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="c5431-127">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="c5431-127">Create conversation thread</span></span>](../api/conversation-post-threads.md) |<span data-ttu-id="c5431-128">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c5431-128">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c5431-129">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="c5431-129">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5431-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c5431-130">Properties</span></span>
| <span data-ttu-id="c5431-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c5431-131">Property</span></span>     | <span data-ttu-id="c5431-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5431-132">Type</span></span>   |<span data-ttu-id="c5431-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5431-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5431-134">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c5431-134">hasAttachments</span></span>|<span data-ttu-id="c5431-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="c5431-135">Boolean</span></span>|<span data-ttu-id="c5431-136">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="c5431-136">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="c5431-137">id</span><span class="sxs-lookup"><span data-stu-id="c5431-137">id</span></span>|<span data-ttu-id="c5431-138">String</span><span class="sxs-lookup"><span data-stu-id="c5431-138">String</span></span>|<span data-ttu-id="c5431-p103">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c5431-p103">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c5431-141">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c5431-141">lastDeliveredDateTime</span></span>|<span data-ttu-id="c5431-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5431-142">DateTimeOffset</span></span>|<span data-ttu-id="c5431-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c5431-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c5431-145">visualização</span><span class="sxs-lookup"><span data-stu-id="c5431-145">preview</span></span>|<span data-ttu-id="c5431-146">String</span><span class="sxs-lookup"><span data-stu-id="c5431-146">String</span></span>|<span data-ttu-id="c5431-147">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="c5431-147">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c5431-148">topic</span><span class="sxs-lookup"><span data-stu-id="c5431-148">topic</span></span>|<span data-ttu-id="c5431-149">String</span><span class="sxs-lookup"><span data-stu-id="c5431-149">String</span></span>|<span data-ttu-id="c5431-p105">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="c5431-p105">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="c5431-152">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c5431-152">uniqueSenders</span></span>|<span data-ttu-id="c5431-153">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c5431-153">String collection</span></span>|<span data-ttu-id="c5431-154">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="c5431-154">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5431-155">Relações</span><span class="sxs-lookup"><span data-stu-id="c5431-155">Relationships</span></span>
| <span data-ttu-id="c5431-156">Relação</span><span class="sxs-lookup"><span data-stu-id="c5431-156">Relationship</span></span> | <span data-ttu-id="c5431-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="c5431-157">Type</span></span>   |<span data-ttu-id="c5431-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5431-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5431-159">threads</span><span class="sxs-lookup"><span data-stu-id="c5431-159">threads</span></span>|<span data-ttu-id="c5431-160">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c5431-160">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="c5431-p106">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c5431-p106">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5431-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c5431-165">JSON representation</span></span>

<span data-ttu-id="c5431-166">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c5431-166">Here is a JSON representation of the resource</span></span>

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
