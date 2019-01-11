---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 89f57e90551efbea435181c35751d54168c498f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886426"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="46795-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="46795-103">conversationThread resource type</span></span>
<span data-ttu-id="46795-104">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="46795-104">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="46795-p101">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="46795-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="46795-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="46795-108">Methods</span></span>

| <span data-ttu-id="46795-109">Método</span><span class="sxs-lookup"><span data-stu-id="46795-109">Method</span></span>       | <span data-ttu-id="46795-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46795-110">Return Type</span></span>  |<span data-ttu-id="46795-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="46795-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46795-112">Listar threads</span><span class="sxs-lookup"><span data-stu-id="46795-112">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="46795-113">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="46795-113">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="46795-114">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="46795-114">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="46795-115">Criar thread</span><span class="sxs-lookup"><span data-stu-id="46795-115">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="46795-116">conversationThread</span><span class="sxs-lookup"><span data-stu-id="46795-116">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="46795-p102">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="46795-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="46795-119">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="46795-119">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="46795-120">conversationThread</span><span class="sxs-lookup"><span data-stu-id="46795-120">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="46795-121">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="46795-121">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="46795-122">Update</span><span class="sxs-lookup"><span data-stu-id="46795-122">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="46795-123">conversationThread</span><span class="sxs-lookup"><span data-stu-id="46795-123">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="46795-124">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="46795-124">Update conversationThread object.</span></span> |
|[<span data-ttu-id="46795-125">Delete</span><span class="sxs-lookup"><span data-stu-id="46795-125">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="46795-126">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="46795-126">None</span></span> |<span data-ttu-id="46795-127">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="46795-127">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="46795-128">Responder</span><span class="sxs-lookup"><span data-stu-id="46795-128">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="46795-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="46795-129">None</span></span>|<span data-ttu-id="46795-130">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="46795-130">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="46795-131">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="46795-131">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="46795-132">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="46795-132">[post](post.md) collection</span></span>| <span data-ttu-id="46795-133">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="46795-133">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="46795-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46795-134">Properties</span></span>
| <span data-ttu-id="46795-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46795-135">Property</span></span>     | <span data-ttu-id="46795-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="46795-136">Type</span></span>   |<span data-ttu-id="46795-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="46795-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46795-138">id</span><span class="sxs-lookup"><span data-stu-id="46795-138">id</span></span>|<span data-ttu-id="46795-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46795-139">String</span></span>| <span data-ttu-id="46795-140">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46795-140">Read-only.</span></span>|
|<span data-ttu-id="46795-141">toRecipients</span><span class="sxs-lookup"><span data-stu-id="46795-141">toRecipients</span></span>|<span data-ttu-id="46795-142">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="46795-142">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="46795-143">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="46795-143">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="46795-144">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="46795-144">ccRecipients</span></span>|<span data-ttu-id="46795-145">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="46795-145">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="46795-146">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="46795-146">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="46795-147">topic</span><span class="sxs-lookup"><span data-stu-id="46795-147">topic</span></span>|<span data-ttu-id="46795-148">String</span><span class="sxs-lookup"><span data-stu-id="46795-148">String</span></span>|<span data-ttu-id="46795-p103">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="46795-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="46795-151">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="46795-151">hasAttachments</span></span>|<span data-ttu-id="46795-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="46795-152">Boolean</span></span>|<span data-ttu-id="46795-153">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="46795-153">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="46795-154">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="46795-154">lastDeliveredDateTime</span></span>|<span data-ttu-id="46795-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46795-155">DateTimeOffset</span></span>|<span data-ttu-id="46795-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="46795-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="46795-158">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="46795-158">uniqueSenders</span></span>|<span data-ttu-id="46795-159">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="46795-159">String collection</span></span>|<span data-ttu-id="46795-160">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="46795-160">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="46795-161">visualização</span><span class="sxs-lookup"><span data-stu-id="46795-161">preview</span></span>|<span data-ttu-id="46795-162">String</span><span class="sxs-lookup"><span data-stu-id="46795-162">String</span></span>|<span data-ttu-id="46795-163">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="46795-163">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="46795-164">isLocked</span><span class="sxs-lookup"><span data-stu-id="46795-164">isLocked</span></span>|<span data-ttu-id="46795-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="46795-165">Boolean</span></span>|<span data-ttu-id="46795-166">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="46795-166">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46795-167">Relações</span><span class="sxs-lookup"><span data-stu-id="46795-167">Relationships</span></span>
| <span data-ttu-id="46795-168">Relação</span><span class="sxs-lookup"><span data-stu-id="46795-168">Relationship</span></span> | <span data-ttu-id="46795-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="46795-169">Type</span></span>   |<span data-ttu-id="46795-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="46795-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46795-171">postagens</span><span class="sxs-lookup"><span data-stu-id="46795-171">posts</span></span>|<span data-ttu-id="46795-172">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="46795-172">[post](post.md) collection</span></span>| <span data-ttu-id="46795-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="46795-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46795-175">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46795-175">JSON representation</span></span>

<span data-ttu-id="46795-176">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="46795-176">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationThread",
  "@odata.annotations": [
    {
      "property": "posts",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
