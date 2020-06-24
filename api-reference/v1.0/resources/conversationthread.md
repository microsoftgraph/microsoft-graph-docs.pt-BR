---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8608ea72c8c136b54f94c73f99ca0f79fbc7ec0b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845264"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="22160-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="22160-103">conversationThread resource type</span></span>

<span data-ttu-id="22160-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22160-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22160-105">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="22160-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="22160-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span><span class="sxs-lookup"><span data-stu-id="22160-106">The last post's recipients collection is the aggregated recipients of the entire thread.</span></span> <span data-ttu-id="22160-107">A thread can have a growing collection of recipients.</span><span class="sxs-lookup"><span data-stu-id="22160-107">A thread can have a growing collection of recipients.</span></span>
<span data-ttu-id="22160-108">A new thread is created when a recipient is removed from the thread.</span><span class="sxs-lookup"><span data-stu-id="22160-108">A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="22160-109">Methods</span><span class="sxs-lookup"><span data-stu-id="22160-109">Methods</span></span>

| <span data-ttu-id="22160-110">Método</span><span class="sxs-lookup"><span data-stu-id="22160-110">Method</span></span>       | <span data-ttu-id="22160-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22160-111">Return Type</span></span>  |<span data-ttu-id="22160-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="22160-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22160-113">Listar threads</span><span class="sxs-lookup"><span data-stu-id="22160-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="22160-114">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="22160-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="22160-115">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="22160-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="22160-116">Criar thread</span><span class="sxs-lookup"><span data-stu-id="22160-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="22160-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="22160-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="22160-118">Start a new conversation by first creating a thread.</span><span class="sxs-lookup"><span data-stu-id="22160-118">Start a new conversation by first creating a thread.</span></span> <span data-ttu-id="22160-119">A new conversation, conversation thread, and post are created in the group.</span><span class="sxs-lookup"><span data-stu-id="22160-119">A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="22160-120">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="22160-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="22160-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="22160-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="22160-122">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="22160-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="22160-123">Update</span><span class="sxs-lookup"><span data-stu-id="22160-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="22160-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="22160-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="22160-125">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="22160-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="22160-126">Delete</span><span class="sxs-lookup"><span data-stu-id="22160-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="22160-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22160-127">None</span></span> |<span data-ttu-id="22160-128">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="22160-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="22160-129">Responder</span><span class="sxs-lookup"><span data-stu-id="22160-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="22160-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="22160-130">None</span></span>|<span data-ttu-id="22160-131">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="22160-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="22160-132">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="22160-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="22160-133">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="22160-133">[post](post.md) collection</span></span>| <span data-ttu-id="22160-134">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="22160-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="22160-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22160-135">Properties</span></span>
| <span data-ttu-id="22160-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22160-136">Property</span></span>              | <span data-ttu-id="22160-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="22160-137">Type</span></span>                                 | <span data-ttu-id="22160-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="22160-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="22160-139">id</span><span class="sxs-lookup"><span data-stu-id="22160-139">id</span></span>                    | <span data-ttu-id="22160-140">String</span><span class="sxs-lookup"><span data-stu-id="22160-140">String</span></span>                               | <span data-ttu-id="22160-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22160-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="22160-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="22160-142">toRecipients</span></span>          | <span data-ttu-id="22160-143">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="22160-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="22160-144">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="22160-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="22160-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="22160-145">ccRecipients</span></span>          | <span data-ttu-id="22160-146">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="22160-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="22160-147">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="22160-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="22160-148">topic</span><span class="sxs-lookup"><span data-stu-id="22160-148">topic</span></span>                 | <span data-ttu-id="22160-149">String</span><span class="sxs-lookup"><span data-stu-id="22160-149">String</span></span>                               | <span data-ttu-id="22160-150">The topic of the conversation.</span><span class="sxs-lookup"><span data-stu-id="22160-150">The topic of the conversation.</span></span> <span data-ttu-id="22160-151">This property can be set when the conversation is created, but it cannot be updated.</span><span class="sxs-lookup"><span data-stu-id="22160-151">This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="22160-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="22160-152">hasAttachments</span></span>        | <span data-ttu-id="22160-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="22160-153">Boolean</span></span>                              | <span data-ttu-id="22160-154">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="22160-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="22160-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="22160-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="22160-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22160-156">DateTimeOffset</span></span>                       | <span data-ttu-id="22160-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span><span class="sxs-lookup"><span data-stu-id="22160-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22160-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22160-158">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="22160-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="22160-159">uniqueSenders</span></span>         | <span data-ttu-id="22160-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="22160-160">String collection</span></span>                    | <span data-ttu-id="22160-161">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="22160-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="22160-162">visualização</span><span class="sxs-lookup"><span data-stu-id="22160-162">preview</span></span>               | <span data-ttu-id="22160-163">String</span><span class="sxs-lookup"><span data-stu-id="22160-163">String</span></span>                               | <span data-ttu-id="22160-164">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="22160-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="22160-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="22160-165">isLocked</span></span>              | <span data-ttu-id="22160-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="22160-166">Boolean</span></span>                              | <span data-ttu-id="22160-167">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="22160-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="22160-168">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="22160-168">Relationships</span></span>
| <span data-ttu-id="22160-169">Relação</span><span class="sxs-lookup"><span data-stu-id="22160-169">Relationship</span></span> | <span data-ttu-id="22160-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="22160-170">Type</span></span>   |<span data-ttu-id="22160-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="22160-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22160-172">postagens</span><span class="sxs-lookup"><span data-stu-id="22160-172">posts</span></span>|<span data-ttu-id="22160-173">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="22160-173">[post](post.md) collection</span></span>| <span data-ttu-id="22160-174">Read-only.</span><span class="sxs-lookup"><span data-stu-id="22160-174">Read-only.</span></span> <span data-ttu-id="22160-175">Nullable.</span><span class="sxs-lookup"><span data-stu-id="22160-175">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22160-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22160-176">JSON representation</span></span>

<span data-ttu-id="22160-177">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="22160-177">Here is a JSON representation of the resource</span></span>

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
