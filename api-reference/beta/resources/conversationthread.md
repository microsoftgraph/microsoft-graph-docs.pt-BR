---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 55a8b414022a338628264fe09e58559a52c3fbcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507391"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="c78cd-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="c78cd-103">conversationThread resource type</span></span>

<span data-ttu-id="c78cd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c78cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c78cd-105">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="c78cd-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="c78cd-p101">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="c78cd-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c78cd-109">Methods</span></span>

| <span data-ttu-id="c78cd-110">Método</span><span class="sxs-lookup"><span data-stu-id="c78cd-110">Method</span></span>       | <span data-ttu-id="c78cd-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c78cd-111">Return Type</span></span>  |<span data-ttu-id="c78cd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c78cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c78cd-113">Listar threads</span><span class="sxs-lookup"><span data-stu-id="c78cd-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="c78cd-114">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c78cd-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="c78cd-115">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c78cd-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="c78cd-116">Criar thread</span><span class="sxs-lookup"><span data-stu-id="c78cd-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="c78cd-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c78cd-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="c78cd-p102">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="c78cd-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="c78cd-120">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="c78cd-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="c78cd-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c78cd-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="c78cd-122">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="c78cd-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="c78cd-123">Update</span><span class="sxs-lookup"><span data-stu-id="c78cd-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="c78cd-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c78cd-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="c78cd-125">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="c78cd-126">Delete</span><span class="sxs-lookup"><span data-stu-id="c78cd-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="c78cd-127">None</span><span class="sxs-lookup"><span data-stu-id="c78cd-127">None</span></span> |<span data-ttu-id="c78cd-128">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="c78cd-129">reply</span><span class="sxs-lookup"><span data-stu-id="c78cd-129">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="c78cd-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c78cd-130">None</span></span>|<span data-ttu-id="c78cd-131">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="c78cd-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="c78cd-132">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="c78cd-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="c78cd-133">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="c78cd-133">[post](post.md) collection</span></span>| <span data-ttu-id="c78cd-134">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="c78cd-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="c78cd-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c78cd-135">Properties</span></span>
| <span data-ttu-id="c78cd-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c78cd-136">Property</span></span>     | <span data-ttu-id="c78cd-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="c78cd-137">Type</span></span>   |<span data-ttu-id="c78cd-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c78cd-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c78cd-139">id</span><span class="sxs-lookup"><span data-stu-id="c78cd-139">id</span></span>|<span data-ttu-id="c78cd-140">String</span><span class="sxs-lookup"><span data-stu-id="c78cd-140">String</span></span>| <span data-ttu-id="c78cd-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c78cd-141">Read-only.</span></span>|
|<span data-ttu-id="c78cd-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c78cd-142">toRecipients</span></span>|<span data-ttu-id="c78cd-143">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c78cd-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c78cd-144">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-144">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="c78cd-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="c78cd-145">ccRecipients</span></span>|<span data-ttu-id="c78cd-146">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c78cd-146">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c78cd-147">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-147">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="c78cd-148">topic</span><span class="sxs-lookup"><span data-stu-id="c78cd-148">topic</span></span>|<span data-ttu-id="c78cd-149">String</span><span class="sxs-lookup"><span data-stu-id="c78cd-149">String</span></span>|<span data-ttu-id="c78cd-p103">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="c78cd-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="c78cd-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c78cd-152">hasAttachments</span></span>|<span data-ttu-id="c78cd-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="c78cd-153">Boolean</span></span>|<span data-ttu-id="c78cd-154">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="c78cd-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="c78cd-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c78cd-155">lastDeliveredDateTime</span></span>|<span data-ttu-id="c78cd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c78cd-156">DateTimeOffset</span></span>|<span data-ttu-id="c78cd-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c78cd-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c78cd-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c78cd-159">uniqueSenders</span></span>|<span data-ttu-id="c78cd-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c78cd-160">String collection</span></span>|<span data-ttu-id="c78cd-161">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="c78cd-161">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="c78cd-162">visualização</span><span class="sxs-lookup"><span data-stu-id="c78cd-162">preview</span></span>|<span data-ttu-id="c78cd-163">String</span><span class="sxs-lookup"><span data-stu-id="c78cd-163">String</span></span>|<span data-ttu-id="c78cd-164">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="c78cd-164">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c78cd-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="c78cd-165">isLocked</span></span>|<span data-ttu-id="c78cd-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="c78cd-166">Boolean</span></span>|<span data-ttu-id="c78cd-167">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c78cd-167">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c78cd-168">Relações</span><span class="sxs-lookup"><span data-stu-id="c78cd-168">Relationships</span></span>
| <span data-ttu-id="c78cd-169">Relação</span><span class="sxs-lookup"><span data-stu-id="c78cd-169">Relationship</span></span> | <span data-ttu-id="c78cd-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="c78cd-170">Type</span></span>   |<span data-ttu-id="c78cd-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="c78cd-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c78cd-172">postagens</span><span class="sxs-lookup"><span data-stu-id="c78cd-172">posts</span></span>|<span data-ttu-id="c78cd-173">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="c78cd-173">[post](post.md) collection</span></span>| <span data-ttu-id="c78cd-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c78cd-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c78cd-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c78cd-176">JSON representation</span></span>

<span data-ttu-id="c78cd-177">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c78cd-177">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationThread"
}-->

```json
{
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": true,
  "id": "string (identifier)",
  "isLocked": true,
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
