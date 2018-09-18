# <a name="conversation-resource-type"></a><span data-ttu-id="c70b1-101">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="c70b1-101">conversation resource type</span></span>

<span data-ttu-id="c70b1-p101">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="c70b1-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

<span data-ttu-id="c70b1-104">Este recurso oferece suporte para assinatura de [notificações de alteração](../../../concepts/webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="c70b1-104">This resource supports subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c70b1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c70b1-105">Methods</span></span>

| <span data-ttu-id="c70b1-106">Método</span><span class="sxs-lookup"><span data-stu-id="c70b1-106">Method</span></span>       | <span data-ttu-id="c70b1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c70b1-107">Return Type</span></span>  |<span data-ttu-id="c70b1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70b1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c70b1-109">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="c70b1-109">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="c70b1-110">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="c70b1-110">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="c70b1-111">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="c70b1-111">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="c70b1-112">Criar</span><span class="sxs-lookup"><span data-stu-id="c70b1-112">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="c70b1-113">conversa</span><span class="sxs-lookup"><span data-stu-id="c70b1-113">conversation</span></span>](conversation.md)| <span data-ttu-id="c70b1-114">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="c70b1-114">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="c70b1-115">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="c70b1-115">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="c70b1-116">conversa</span><span class="sxs-lookup"><span data-stu-id="c70b1-116">conversation</span></span>](conversation.md) |<span data-ttu-id="c70b1-117">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c70b1-117">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="c70b1-118">Excluir</span><span class="sxs-lookup"><span data-stu-id="c70b1-118">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="c70b1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c70b1-119">None</span></span> |<span data-ttu-id="c70b1-120">Exclua um objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="c70b1-120">Delete conversation object.</span></span> |
|[<span data-ttu-id="c70b1-121">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="c70b1-121">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="c70b1-122">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c70b1-122">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c70b1-123">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="c70b1-123">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="c70b1-124">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="c70b1-124">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="c70b1-125">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c70b1-125">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="c70b1-126">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="c70b1-126">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="c70b1-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c70b1-127">Properties</span></span>
| <span data-ttu-id="c70b1-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c70b1-128">Property</span></span>     | <span data-ttu-id="c70b1-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c70b1-129">Type</span></span>   |<span data-ttu-id="c70b1-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70b1-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c70b1-131">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c70b1-131">hasAttachments</span></span>|<span data-ttu-id="c70b1-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="c70b1-132">Boolean</span></span>|<span data-ttu-id="c70b1-133">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="c70b1-133">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="c70b1-134">id</span><span class="sxs-lookup"><span data-stu-id="c70b1-134">id</span></span>|<span data-ttu-id="c70b1-135">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c70b1-135">String</span></span>|<span data-ttu-id="c70b1-p102">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c70b1-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="c70b1-138">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="c70b1-138">lastDeliveredDateTime</span></span>|<span data-ttu-id="c70b1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c70b1-139">DateTimeOffset</span></span>|<span data-ttu-id="c70b1-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c70b1-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c70b1-142">visualização</span><span class="sxs-lookup"><span data-stu-id="c70b1-142">preview</span></span>|<span data-ttu-id="c70b1-143">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c70b1-143">String</span></span>|<span data-ttu-id="c70b1-144">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="c70b1-144">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="c70b1-145">tópico</span><span class="sxs-lookup"><span data-stu-id="c70b1-145">topic</span></span>|<span data-ttu-id="c70b1-146">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c70b1-146">String</span></span>|<span data-ttu-id="c70b1-p104">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="c70b1-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="c70b1-149">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="c70b1-149">uniqueSenders</span></span>|<span data-ttu-id="c70b1-150">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c70b1-150">String collection</span></span>|<span data-ttu-id="c70b1-151">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="c70b1-151">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c70b1-152">Relações</span><span class="sxs-lookup"><span data-stu-id="c70b1-152">Relationships</span></span>
| <span data-ttu-id="c70b1-153">Relação</span><span class="sxs-lookup"><span data-stu-id="c70b1-153">Relationship</span></span> | <span data-ttu-id="c70b1-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="c70b1-154">Type</span></span>   |<span data-ttu-id="c70b1-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="c70b1-155">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c70b1-156">threads</span><span class="sxs-lookup"><span data-stu-id="c70b1-156">threads</span></span>|<span data-ttu-id="c70b1-157">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="c70b1-157">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="c70b1-p105">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c70b1-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c70b1-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c70b1-162">JSON representation</span></span>

<span data-ttu-id="c70b1-163">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c70b1-163">Here is a JSON representation of the resource</span></span>

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
