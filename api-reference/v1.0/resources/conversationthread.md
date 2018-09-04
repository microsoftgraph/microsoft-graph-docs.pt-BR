# <a name="conversationthread-resource-type"></a><span data-ttu-id="6a079-101">tipo de recurso conversationThread</span><span class="sxs-lookup"><span data-stu-id="6a079-101">conversationThread resource type</span></span>
<span data-ttu-id="6a079-102">Um conversationThread é uma coleção de [postagens](post.md).</span><span class="sxs-lookup"><span data-stu-id="6a079-102">A conversationThread is a collection of [posts](post.md).</span></span>

<span data-ttu-id="6a079-p101">A coleção de destinatários da última postagem são os destinatários agregados do thread inteiro. Um thread pode ter uma coleção crescente de destinatários. Um novo thread é criado quando um destinatário é removido do thread.</span><span class="sxs-lookup"><span data-stu-id="6a079-p101">The last post's recipients collection is the aggregated recipients of the entire thread. A thread can have a growing collection of recipients. A new thread is created when a recipient is removed from the thread.</span></span>

## <a name="methods"></a><span data-ttu-id="6a079-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a079-106">Methods</span></span>

| <span data-ttu-id="6a079-107">Método</span><span class="sxs-lookup"><span data-stu-id="6a079-107">Method</span></span>       | <span data-ttu-id="6a079-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6a079-108">Return Type</span></span>  |<span data-ttu-id="6a079-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a079-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a079-110">Listar threads</span><span class="sxs-lookup"><span data-stu-id="6a079-110">List threads</span></span>](../api/group_list_threads.md) | <span data-ttu-id="6a079-111">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="6a079-111">[conversationThread](conversationthread.md) collection</span></span> |<span data-ttu-id="6a079-112">Obter todos os threads de um grupo.</span><span class="sxs-lookup"><span data-stu-id="6a079-112">Get all the threads of a group.</span></span>|
|[<span data-ttu-id="6a079-113">Criar thread</span><span class="sxs-lookup"><span data-stu-id="6a079-113">Create thread</span></span>](../api/group_post_threads.md) | [<span data-ttu-id="6a079-114">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6a079-114">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6a079-p102">Inicie uma nova conversa criando primeiro um thread. Uma nova conversa, thread de conversas e posts são criados no grupo.</span><span class="sxs-lookup"><span data-stu-id="6a079-p102">Start a new conversation by first creating a thread. A new conversation, conversation thread, and post are created in the group.</span></span>|
|[<span data-ttu-id="6a079-117">Obter conversationThread</span><span class="sxs-lookup"><span data-stu-id="6a079-117">Get conversationThread</span></span>](../api/conversationthread_get.md) | [<span data-ttu-id="6a079-118">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6a079-118">conversationThread</span></span>](conversationthread.md) |<span data-ttu-id="6a079-119">Obtenha um thread específico pertencente a um grupo.</span><span class="sxs-lookup"><span data-stu-id="6a079-119">Get a specific thread that belongs to a group.</span></span> |
|[<span data-ttu-id="6a079-120">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6a079-120">Update</span></span>](../api/conversationthread_update.md) | [<span data-ttu-id="6a079-121">conversationThread</span><span class="sxs-lookup"><span data-stu-id="6a079-121">conversationThread</span></span>](conversationthread.md)  |<span data-ttu-id="6a079-122">Atualize o objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="6a079-122">Update conversationThread object.</span></span> |
|[<span data-ttu-id="6a079-123">Excluir</span><span class="sxs-lookup"><span data-stu-id="6a079-123">Delete</span></span>](../api/conversationthread_delete.md) | <span data-ttu-id="6a079-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a079-124">None</span></span> |<span data-ttu-id="6a079-125">Exclua um objeto conversationThread.</span><span class="sxs-lookup"><span data-stu-id="6a079-125">Delete conversationThread object.</span></span> |
|[<span data-ttu-id="6a079-126">Responder</span><span class="sxs-lookup"><span data-stu-id="6a079-126">Reply</span></span>](../api/conversationthread_reply.md)|<span data-ttu-id="6a079-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6a079-127">None</span></span>|<span data-ttu-id="6a079-128">Responda a este thread criando uma nova entidade Post.</span><span class="sxs-lookup"><span data-stu-id="6a079-128">Reply to this thread by creating a new Post entity.</span></span>|
|[<span data-ttu-id="6a079-129">Listar Postagens</span><span class="sxs-lookup"><span data-stu-id="6a079-129">List Posts</span></span>](../api/conversationthread_list_posts.md) |<span data-ttu-id="6a079-130">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="6a079-130">[post](post.md) collection</span></span>| <span data-ttu-id="6a079-131">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="6a079-131">Get the posts of the specified thread.</span></span> |

## <a name="properties"></a><span data-ttu-id="6a079-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a079-132">Properties</span></span>
| <span data-ttu-id="6a079-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a079-133">Property</span></span>     | <span data-ttu-id="6a079-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a079-134">Type</span></span>   |<span data-ttu-id="6a079-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a079-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a079-136">id</span><span class="sxs-lookup"><span data-stu-id="6a079-136">id</span></span>|<span data-ttu-id="6a079-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a079-137">String</span></span>| <span data-ttu-id="6a079-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a079-138">Read-only.</span></span>|
|<span data-ttu-id="6a079-139">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6a079-139">toRecipients</span></span>|<span data-ttu-id="6a079-140">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6a079-140">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6a079-141">Os destinatários Para: do thread.</span><span class="sxs-lookup"><span data-stu-id="6a079-141">The To: recipients for the thread.</span></span>|
|<span data-ttu-id="6a079-142">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="6a079-142">ccRecipients</span></span>|<span data-ttu-id="6a079-143">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="6a079-143">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="6a079-144">Os destinatários Cc: do thread.</span><span class="sxs-lookup"><span data-stu-id="6a079-144">The Cc: recipients for the thread.</span></span>|
|<span data-ttu-id="6a079-145">topic</span><span class="sxs-lookup"><span data-stu-id="6a079-145">topic</span></span>|<span data-ttu-id="6a079-146">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a079-146">String</span></span>|<span data-ttu-id="6a079-p103">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="6a079-p103">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>||
|<span data-ttu-id="6a079-149">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="6a079-149">hasAttachments</span></span>|<span data-ttu-id="6a079-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a079-150">Boolean</span></span>|<span data-ttu-id="6a079-151">Indica se qualquer uma das postagens neste thread tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="6a079-151">Indicates whether any of the posts within this thread has at least one attachment.</span></span>|
|<span data-ttu-id="6a079-152">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="6a079-152">lastDeliveredDateTime</span></span>|<span data-ttu-id="6a079-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a079-153">DateTimeOffset</span></span>|<span data-ttu-id="6a079-p104">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6a079-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6a079-156">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="6a079-156">uniqueSenders</span></span>|<span data-ttu-id="6a079-157">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a079-157">String collection</span></span>|<span data-ttu-id="6a079-158">Todos os usuários que enviaram uma mensagem para este thread.</span><span class="sxs-lookup"><span data-stu-id="6a079-158">All the users that sent a message to this thread.</span></span>|
|<span data-ttu-id="6a079-159">visualização</span><span class="sxs-lookup"><span data-stu-id="6a079-159">preview</span></span>|<span data-ttu-id="6a079-160">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a079-160">String</span></span>|<span data-ttu-id="6a079-161">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="6a079-161">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="6a079-162">isLocked</span><span class="sxs-lookup"><span data-stu-id="6a079-162">isLocked</span></span>|<span data-ttu-id="6a079-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a079-163">Boolean</span></span>|<span data-ttu-id="6a079-164">Indica se o thread está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="6a079-164">Indicates if the thread is locked.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a079-165">Relações</span><span class="sxs-lookup"><span data-stu-id="6a079-165">Relationships</span></span>
| <span data-ttu-id="6a079-166">Relação</span><span class="sxs-lookup"><span data-stu-id="6a079-166">Relationship</span></span> | <span data-ttu-id="6a079-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a079-167">Type</span></span>   |<span data-ttu-id="6a079-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a079-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a079-169">postagens</span><span class="sxs-lookup"><span data-stu-id="6a079-169">posts</span></span>|<span data-ttu-id="6a079-170">Coleção [post](post.md)</span><span class="sxs-lookup"><span data-stu-id="6a079-170">[post](post.md) collection</span></span>| <span data-ttu-id="6a079-p105">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="6a079-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a079-173">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a079-173">JSON representation</span></span>

<span data-ttu-id="6a079-174">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="6a079-174">Here is a JSON representation of the resource</span></span>

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
