# <a name="conversationthread-resource-type"></a><span data-ttu-id="a1ae9-101">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-101">conversationThread resource type</span></span>
<span data-ttu-id="a1ae9-102">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="a1ae9-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="a1ae9-p101">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="a1ae9-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a1ae9-106">Methods</span></span>

| <span data-ttu-id="a1ae9-107">Método</span><span class="sxs-lookup"><span data-stu-id="a1ae9-107">Method</span></span>       | <span data-ttu-id="a1ae9-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a1ae9-108">Return Type</span></span>  |<span data-ttu-id="a1ae9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ae9-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a1ae9-110">Listar threads</span><span class="sxs-lookup"><span data-stu-id="a1ae9-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="a1ae9-111">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="a1ae9-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="a1ae9-112">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="a1ae9-113">Criar thread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="a1ae9-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="a1ae9-p102">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="a1ae9-117">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="a1ae9-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="a1ae9-119">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="a1ae9-120">Update</span><span class="sxs-lookup"><span data-stu-id="a1ae9-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="a1ae9-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="a1ae9-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="a1ae9-122">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="a1ae9-123">Delete</span><span class="sxs-lookup"><span data-stu-id="a1ae9-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="a1ae9-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a1ae9-124">None</span></span> |<span data-ttu-id="a1ae9-125">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="a1ae9-126">Responder</span><span class="sxs-lookup"><span data-stu-id="a1ae9-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="a1ae9-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a1ae9-127">None</span></span>|<span data-ttu-id="a1ae9-128">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="a1ae9-129">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="a1ae9-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="a1ae9-130">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="a1ae9-130">[post](post.md) collection</span></span>| <span data-ttu-id="a1ae9-131">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="a1ae9-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1ae9-132">Properties</span></span>
| <span data-ttu-id="a1ae9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1ae9-133">Property</span></span>     | <span data-ttu-id="a1ae9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1ae9-134">Type</span></span>   |<span data-ttu-id="a1ae9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ae9-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ae9-136">id</span><span class="sxs-lookup"><span data-stu-id="a1ae9-136">id</span></span>|<span data-ttu-id="a1ae9-137">String</span><span class="sxs-lookup"><span data-stu-id="a1ae9-137">String</span></span>| <span data-ttu-id="a1ae9-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-138">Read-only.</span></span>|
|<span data-ttu-id="a1ae9-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a1ae9-139">toRecipients</span></span>|<span data-ttu-id="a1ae9-140">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a1ae9-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="a1ae9-141">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="a1ae9-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="a1ae9-142">ccRecipients</span></span>|<span data-ttu-id="a1ae9-143">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="a1ae9-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="a1ae9-144">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="a1ae9-145">topic</span><span class="sxs-lookup"><span data-stu-id="a1ae9-145">topic</span></span>|<span data-ttu-id="a1ae9-146">String</span><span class="sxs-lookup"><span data-stu-id="a1ae9-146">String</span></span>|<span data-ttu-id="a1ae9-p103">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="a1ae9-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="a1ae9-149">hasAttachments</span></span>|<span data-ttu-id="a1ae9-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1ae9-150">Boolean</span></span>|<span data-ttu-id="a1ae9-151">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="a1ae9-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="a1ae9-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="a1ae9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1ae9-153">DateTimeOffset</span></span>|<span data-ttu-id="a1ae9-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a1ae9-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a1ae9-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="a1ae9-156">uniqueSenders</span></span>|<span data-ttu-id="a1ae9-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1ae9-157">String collection</span></span>|<span data-ttu-id="a1ae9-158">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="a1ae9-159">visualização</span><span class="sxs-lookup"><span data-stu-id="a1ae9-159">preview</span></span>|<span data-ttu-id="a1ae9-160">String</span><span class="sxs-lookup"><span data-stu-id="a1ae9-160">String</span></span>|<span data-ttu-id="a1ae9-161">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="a1ae9-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="a1ae9-162">isLocked</span></span>|<span data-ttu-id="a1ae9-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="a1ae9-163">Boolean</span></span>|<span data-ttu-id="a1ae9-164">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1ae9-165">Relações</span><span class="sxs-lookup"><span data-stu-id="a1ae9-165">Relationships</span></span>
| <span data-ttu-id="a1ae9-166">Relação</span><span class="sxs-lookup"><span data-stu-id="a1ae9-166">Relationship</span></span> | <span data-ttu-id="a1ae9-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1ae9-167">Type</span></span>   |<span data-ttu-id="a1ae9-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ae9-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ae9-169">postagens</span><span class="sxs-lookup"><span data-stu-id="a1ae9-169">posts</span></span>|<span data-ttu-id="a1ae9-170">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="a1ae9-170">[post](post.md) collection</span></span>| <span data-ttu-id="a1ae9-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="a1ae9-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1ae9-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1ae9-173">JSON representation</span></span>

<span data-ttu-id="a1ae9-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a1ae9-174">Here is a JSON representation of the resource</span></span>

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
