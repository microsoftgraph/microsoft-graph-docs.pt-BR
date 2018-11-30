---
title: tipo de recurso conversationThread
description: Um conversationThread é uma coleção de postagens.
ms.openlocfilehash: a63b208e30372c2cced1e440f3a46e605ea26589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033445"
---
# <a name="conversationthread-resource-type"></a><span data-ttu-id="bfcca-103">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="bfcca-103">conversationThread resource type</span></span>

> <span data-ttu-id="bfcca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bfcca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfcca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bfcca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfcca-106">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="bfcca-106">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="bfcca-p102">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-p102">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="bfcca-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="bfcca-110">Methods</span></span>

| <span data-ttu-id="bfcca-111">Método</span><span class="sxs-lookup"><span data-stu-id="bfcca-111">Method</span></span>       | <span data-ttu-id="bfcca-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfcca-112">Return Type</span></span>  |<span data-ttu-id="bfcca-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcca-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfcca-114">Listar threads</span><span class="sxs-lookup"><span data-stu-id="bfcca-114">List threads</span></span>](../api/group-list-threads.md) | <span data-ttu-id="bfcca-115">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="bfcca-115">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="bfcca-116">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="bfcca-116">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="bfcca-117">Criar thread</span><span class="sxs-lookup"><span data-stu-id="bfcca-117">Create thread</span></span>](../api/group-post-threads.md) | [<span data-ttu-id="bfcca-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="bfcca-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="bfcca-p103">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="bfcca-p103">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="bfcca-121">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="bfcca-121">Get conversationThread</span></span>](../api/conversationthread-get.md) | [<span data-ttu-id="bfcca-122">conversationThread</span><span class="sxs-lookup"><span data-stu-id="bfcca-122">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="bfcca-123">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="bfcca-123">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="bfcca-124">Update</span><span class="sxs-lookup"><span data-stu-id="bfcca-124">Update</span></span>](../api/conversationthread-update.md) | [<span data-ttu-id="bfcca-125">conversationThread</span><span class="sxs-lookup"><span data-stu-id="bfcca-125">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="bfcca-126">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-126">Update conversationThread object.</span></span> |
|[<span data-ttu-id="bfcca-127">Delete</span><span class="sxs-lookup"><span data-stu-id="bfcca-127">Delete</span></span>](../api/conversationthread-delete.md) | <span data-ttu-id="bfcca-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bfcca-128">None</span></span> |<span data-ttu-id="bfcca-129">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-129">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="bfcca-130">reply</span><span class="sxs-lookup"><span data-stu-id="bfcca-130">reply</span></span>](../api/conversationthread-reply.md)|<span data-ttu-id="bfcca-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfcca-131">None</span></span>|<span data-ttu-id="bfcca-132">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="bfcca-132">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="bfcca-133">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="bfcca-133">List Posts</span></span>](../api/conversationthread-list-posts.md) |<span data-ttu-id="bfcca-134">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="bfcca-134">[post](post.md) collection</span></span>| <span data-ttu-id="bfcca-135">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="bfcca-135">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="bfcca-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfcca-136">Properties</span></span>
| <span data-ttu-id="bfcca-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfcca-137">Property</span></span>     | <span data-ttu-id="bfcca-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfcca-138">Type</span></span>   |<span data-ttu-id="bfcca-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcca-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfcca-140">id</span><span class="sxs-lookup"><span data-stu-id="bfcca-140">id</span></span>|<span data-ttu-id="bfcca-141">String</span><span class="sxs-lookup"><span data-stu-id="bfcca-141">String</span></span>| <span data-ttu-id="bfcca-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfcca-142">Read-only.</span></span>|
|<span data-ttu-id="bfcca-143">toRecipients</span><span class="sxs-lookup"><span data-stu-id="bfcca-143">toRecipients</span></span>|<span data-ttu-id="bfcca-144">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="bfcca-144">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="bfcca-145">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-145">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="bfcca-146">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="bfcca-146">ccRecipients</span></span>|<span data-ttu-id="bfcca-147">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="bfcca-147">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="bfcca-148">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-148">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="bfcca-149">topic</span><span class="sxs-lookup"><span data-stu-id="bfcca-149">topic</span></span>|<span data-ttu-id="bfcca-150">String</span><span class="sxs-lookup"><span data-stu-id="bfcca-150">String</span></span>|<span data-ttu-id="bfcca-p104">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="bfcca-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="bfcca-153">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="bfcca-153">hasAttachments</span></span>|<span data-ttu-id="bfcca-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="bfcca-154">Boolean</span></span>|<span data-ttu-id="bfcca-155">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="bfcca-155">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="bfcca-156">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="bfcca-156">lastDeliveredDateTime</span></span>|<span data-ttu-id="bfcca-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfcca-157">DateTimeOffset</span></span>|<span data-ttu-id="bfcca-p105">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bfcca-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bfcca-160">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="bfcca-160">uniqueSenders</span></span>|<span data-ttu-id="bfcca-161">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfcca-161">String collection</span></span>|<span data-ttu-id="bfcca-162">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="bfcca-162">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="bfcca-163">visualização</span><span class="sxs-lookup"><span data-stu-id="bfcca-163">preview</span></span>|<span data-ttu-id="bfcca-164">String</span><span class="sxs-lookup"><span data-stu-id="bfcca-164">String</span></span>|<span data-ttu-id="bfcca-165">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="bfcca-165">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="bfcca-166">isLocked</span><span class="sxs-lookup"><span data-stu-id="bfcca-166">isLocked</span></span>|<span data-ttu-id="bfcca-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="bfcca-167">Boolean</span></span>|<span data-ttu-id="bfcca-168">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="bfcca-168">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfcca-169">Relações</span><span class="sxs-lookup"><span data-stu-id="bfcca-169">Relationships</span></span>
| <span data-ttu-id="bfcca-170">Relação</span><span class="sxs-lookup"><span data-stu-id="bfcca-170">Relationship</span></span> | <span data-ttu-id="bfcca-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfcca-171">Type</span></span>   |<span data-ttu-id="bfcca-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfcca-172">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfcca-173">postagens</span><span class="sxs-lookup"><span data-stu-id="bfcca-173">posts</span></span>|<span data-ttu-id="bfcca-174">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="bfcca-174">[post](post.md) collection</span></span>| <span data-ttu-id="bfcca-p106">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bfcca-p106">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfcca-177">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfcca-177">JSON representation</span></span>

<span data-ttu-id="bfcca-178">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bfcca-178">Here is a JSON representation of the resource</span></span>

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
