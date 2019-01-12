---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: d541d4ac47272c2825602b28526b2b7c9d5f3fcb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933551"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="c14f9-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="c14f9-103">conversationThread resource type</span></span>

> <span data-ttu-id="c14f9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c14f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c14f9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c14f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c14f9-106">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="c14f9-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="c14f9-p102">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="c14f9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="c14f9-110">Methods</span></span>

| <span data-ttu-id="c14f9-111">Método</span><span class="sxs-lookup"><span data-stu-id="c14f9-111">Method</span></span>       | <span data-ttu-id="c14f9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c14f9-112">Return Type</span></span>  |<span data-ttu-id="c14f9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14f9-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c14f9-114">Listar threads</span><span class="sxs-lookup"><span data-stu-id="c14f9-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="c14f9-115">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c14f9-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="c14f9-116">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c14f9-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="c14f9-117">Criar thread</span><span class="sxs-lookup"><span data-stu-id="c14f9-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="c14f9-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c14f9-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="c14f9-p103">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="c14f9-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="c14f9-121">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="c14f9-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="c14f9-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c14f9-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="c14f9-123">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="c14f9-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="c14f9-124">Update</span><span class="sxs-lookup"><span data-stu-id="c14f9-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="c14f9-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="c14f9-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="c14f9-126">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="c14f9-127">Delete</span><span class="sxs-lookup"><span data-stu-id="c14f9-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="c14f9-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c14f9-128">None</span></span> |<span data-ttu-id="c14f9-129">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="c14f9-130">reply</span><span class="sxs-lookup"><span data-stu-id="c14f9-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="c14f9-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c14f9-131">None</span></span>|<span data-ttu-id="c14f9-132">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="c14f9-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="c14f9-133">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="c14f9-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="c14f9-134">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="c14f9-134">[post](post.md) collection</span></span>| <span data-ttu-id="c14f9-135">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="c14f9-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="c14f9-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c14f9-136">Properties</span></span>
| <span data-ttu-id="c14f9-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c14f9-137">Property</span></span>     | <span data-ttu-id="c14f9-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="c14f9-138">Type</span></span>   |<span data-ttu-id="c14f9-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14f9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c14f9-140">id</span><span class="sxs-lookup"><span data-stu-id="c14f9-140">id</span></span>|<span data-ttu-id="c14f9-141">String</span><span class="sxs-lookup"><span data-stu-id="c14f9-141">String</span></span>| <span data-ttu-id="c14f9-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c14f9-142">Read-only.</span></span>|
|<span data-ttu-id="c14f9-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="c14f9-143">toRecipients</span></span>|<span data-ttu-id="c14f9-144">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c14f9-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c14f9-145">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="c14f9-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="c14f9-146">ccRecipients</span></span>|<span data-ttu-id="c14f9-147">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="c14f9-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="c14f9-148">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="c14f9-149">topic</span><span class="sxs-lookup"><span data-stu-id="c14f9-149">topic</span></span>|<span data-ttu-id="c14f9-150">String</span><span class="sxs-lookup"><span data-stu-id="c14f9-150">String</span></span>|<span data-ttu-id="c14f9-p104">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="c14f9-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="c14f9-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c14f9-153">hasAttachments</span></span>|<span data-ttu-id="c14f9-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="c14f9-154">Boolean</span></span>|<span data-ttu-id="c14f9-155">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="c14f9-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="c14f9-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c14f9-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="c14f9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c14f9-157">DateTimeOffset</span></span>|<span data-ttu-id="c14f9-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c14f9-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c14f9-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c14f9-160">uniqueSenders</span></span>|<span data-ttu-id="c14f9-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c14f9-161">String collection</span></span>|<span data-ttu-id="c14f9-162">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="c14f9-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="c14f9-163">visualização</span><span class="sxs-lookup"><span data-stu-id="c14f9-163">preview</span></span>|<span data-ttu-id="c14f9-164">String</span><span class="sxs-lookup"><span data-stu-id="c14f9-164">String</span></span>|<span data-ttu-id="c14f9-165">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="c14f9-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c14f9-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="c14f9-166">isLocked</span></span>|<span data-ttu-id="c14f9-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="c14f9-167">Boolean</span></span>|<span data-ttu-id="c14f9-168">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c14f9-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c14f9-169">Relações</span><span class="sxs-lookup"><span data-stu-id="c14f9-169">Relationships</span></span>
| <span data-ttu-id="c14f9-170">Relação</span><span class="sxs-lookup"><span data-stu-id="c14f9-170">Relationship</span></span> | <span data-ttu-id="c14f9-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="c14f9-171">Type</span></span>   |<span data-ttu-id="c14f9-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="c14f9-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c14f9-173">postagens</span><span class="sxs-lookup"><span data-stu-id="c14f9-173">posts</span></span>|<span data-ttu-id="c14f9-174">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="c14f9-174">[post](post.md) collection</span></span>| <span data-ttu-id="c14f9-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c14f9-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c14f9-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c14f9-177">JSON representation</span></span>

<span data-ttu-id="c14f9-178">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c14f9-178">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
