---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: fa9ce48f9b0dd0dd1869a1e31937b70cf4edb975
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720148"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="40b97-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="40b97-103">conversationThread resource type</span></span>

<span data-ttu-id="40b97-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40b97-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40b97-105">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="40b97-105">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="40b97-p101">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="40b97-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="40b97-109">Methods</span><span class="sxs-lookup"><span data-stu-id="40b97-109">Methods</span></span>

| <span data-ttu-id="40b97-110">Método</span><span class="sxs-lookup"><span data-stu-id="40b97-110">Method</span></span>       | <span data-ttu-id="40b97-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="40b97-111">Return Type</span></span>  |<span data-ttu-id="40b97-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b97-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="40b97-113">Listar threads</span><span class="sxs-lookup"><span data-stu-id="40b97-113">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="40b97-114">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="40b97-114">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="40b97-115">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="40b97-115">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="40b97-116">Criar thread</span><span class="sxs-lookup"><span data-stu-id="40b97-116">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="40b97-117">conversationThread</span><span class="sxs-lookup"><span data-stu-id="40b97-117">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="40b97-p102">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="40b97-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="40b97-120">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="40b97-120">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="40b97-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="40b97-121">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="40b97-122">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="40b97-122">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="40b97-123">Update</span><span class="sxs-lookup"><span data-stu-id="40b97-123">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="40b97-124">conversationThread</span><span class="sxs-lookup"><span data-stu-id="40b97-124">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="40b97-125">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="40b97-125">Update conversationThread object.</span></span> |
|[<span data-ttu-id="40b97-126">Delete</span><span class="sxs-lookup"><span data-stu-id="40b97-126">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="40b97-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40b97-127">None</span></span> |<span data-ttu-id="40b97-128">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="40b97-128">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="40b97-129">Responder</span><span class="sxs-lookup"><span data-stu-id="40b97-129">Reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="40b97-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="40b97-130">None</span></span>|<span data-ttu-id="40b97-131">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="40b97-131">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="40b97-132">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="40b97-132">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="40b97-133">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="40b97-133">[post](post.md) collection</span></span>| <span data-ttu-id="40b97-134">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="40b97-134">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="40b97-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40b97-135">Properties</span></span>
| <span data-ttu-id="40b97-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40b97-136">Property</span></span>              | <span data-ttu-id="40b97-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b97-137">Type</span></span>                                 | <span data-ttu-id="40b97-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b97-138">Description</span></span>                                                                                                                                                                                      |
|:----------------------|:-------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="40b97-139">id</span><span class="sxs-lookup"><span data-stu-id="40b97-139">id</span></span>                    | <span data-ttu-id="40b97-140">String</span><span class="sxs-lookup"><span data-stu-id="40b97-140">String</span></span>                               | <span data-ttu-id="40b97-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="40b97-141">Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="40b97-142">toRecipients</span><span class="sxs-lookup"><span data-stu-id="40b97-142">toRecipients</span></span>          | <span data-ttu-id="40b97-143">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="40b97-143">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="40b97-144">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="40b97-144">The To: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="40b97-145">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="40b97-145">ccRecipients</span></span>          | <span data-ttu-id="40b97-146">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="40b97-146">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="40b97-147">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="40b97-147">The Cc: recipients for the thread.</span></span>                                                                                                                                                               |
| <span data-ttu-id="40b97-148">topic</span><span class="sxs-lookup"><span data-stu-id="40b97-148">topic</span></span>                 | <span data-ttu-id="40b97-149">String</span><span class="sxs-lookup"><span data-stu-id="40b97-149">String</span></span>                               | <span data-ttu-id="40b97-p103">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="40b97-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>                                                                              |
| <span data-ttu-id="40b97-152">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="40b97-152">hasAttachments</span></span>        | <span data-ttu-id="40b97-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="40b97-153">Boolean</span></span>                              | <span data-ttu-id="40b97-154">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="40b97-154">Indicates whether any of the posts within this thread has at least one attachment.</span></span>                                                                                                               |
| <span data-ttu-id="40b97-155">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="40b97-155">lastDeliveredDateTime</span></span> | <span data-ttu-id="40b97-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40b97-156">DateTimeOffset</span></span>                       | <span data-ttu-id="40b97-157">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="40b97-157">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40b97-158">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="40b97-158">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="40b97-159">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="40b97-159">uniqueSenders</span></span>         | <span data-ttu-id="40b97-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="40b97-160">String collection</span></span>                    | <span data-ttu-id="40b97-161">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="40b97-161">All the users that sent a message to this thread.</span></span>                                                                                                                                                |
| <span data-ttu-id="40b97-162">visualização</span><span class="sxs-lookup"><span data-stu-id="40b97-162">preview</span></span>               | <span data-ttu-id="40b97-163">String</span><span class="sxs-lookup"><span data-stu-id="40b97-163">String</span></span>                               | <span data-ttu-id="40b97-164">Um breve resumo do corpo da postagem mais recente nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="40b97-164">A short summary from the body of the latest post in this conversation.</span></span>                                                                                                                           |
| <span data-ttu-id="40b97-165">isLocked</span><span class="sxs-lookup"><span data-stu-id="40b97-165">isLocked</span></span>              | <span data-ttu-id="40b97-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="40b97-166">Boolean</span></span>                              | <span data-ttu-id="40b97-167">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="40b97-167">Indicates if the thread is locked.</span></span>                                                                                                                                                               |

## <a name="relationships"></a><span data-ttu-id="40b97-168">Relações</span><span class="sxs-lookup"><span data-stu-id="40b97-168">Relationships</span></span>
| <span data-ttu-id="40b97-169">Relação</span><span class="sxs-lookup"><span data-stu-id="40b97-169">Relationship</span></span> | <span data-ttu-id="40b97-170">Tipo</span><span class="sxs-lookup"><span data-stu-id="40b97-170">Type</span></span>   |<span data-ttu-id="40b97-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="40b97-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40b97-172">postagens</span><span class="sxs-lookup"><span data-stu-id="40b97-172">posts</span></span>|<span data-ttu-id="40b97-173">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="40b97-173">[post](post.md) collection</span></span>| <span data-ttu-id="40b97-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="40b97-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40b97-176">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40b97-176">JSON representation</span></span>

<span data-ttu-id="40b97-177">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="40b97-177">Here is a JSON representation of the resource</span></span>

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

