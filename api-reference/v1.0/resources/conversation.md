# <a name="conversation-resource-type"></a><span data-ttu-id="be520-101">tipo de recurso conversation</span><span class="sxs-lookup"><span data-stu-id="be520-101">conversation resource type</span></span>

<span data-ttu-id="be520-p101">Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.</span><span class="sxs-lookup"><span data-stu-id="be520-p101">A conversation is a collection of [threads](conversationthread.md), and a thread contains posts to that thread. All threads and posts in a conversation share the same subject.</span></span>

## <a name="methods"></a><span data-ttu-id="be520-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="be520-104">Methods</span></span>

| <span data-ttu-id="be520-105">Método</span><span class="sxs-lookup"><span data-stu-id="be520-105">Method</span></span>       | <span data-ttu-id="be520-106">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="be520-106">Return Type</span></span>  |<span data-ttu-id="be520-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="be520-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="be520-108">Listar conversas</span><span class="sxs-lookup"><span data-stu-id="be520-108">List conversations</span></span>](../api/group_list_conversations.md) | <span data-ttu-id="be520-109">Coleção [conversation](conversation.md)</span><span class="sxs-lookup"><span data-stu-id="be520-109">[conversation](conversation.md) collection</span></span> |<span data-ttu-id="be520-110">Obtenha a lista de conversas desse grupo.</span><span class="sxs-lookup"><span data-stu-id="be520-110">Get the list of conversations in this group.</span></span>|
|[<span data-ttu-id="be520-111">Criar</span><span class="sxs-lookup"><span data-stu-id="be520-111">Create</span></span>](../api/group_post_conversations.md) |[<span data-ttu-id="be520-112">conversa</span><span class="sxs-lookup"><span data-stu-id="be520-112">conversation</span></span>](conversation.md)| <span data-ttu-id="be520-113">Crie uma nova conversa incluindo um thread e uma postagem.</span><span class="sxs-lookup"><span data-stu-id="be520-113">Create a new conversation by including a thread and a post.</span></span>|
|[<span data-ttu-id="be520-114">Obter conversa</span><span class="sxs-lookup"><span data-stu-id="be520-114">Get conversation</span></span>](../api/conversation_get.md) | [<span data-ttu-id="be520-115">conversa</span><span class="sxs-lookup"><span data-stu-id="be520-115">conversation</span></span>](conversation.md) |<span data-ttu-id="be520-116">Leia as propriedades e os relacionamentos do objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="be520-116">Read properties and relationships of conversation object.</span></span>|
|[<span data-ttu-id="be520-117">Excluir</span><span class="sxs-lookup"><span data-stu-id="be520-117">Delete</span></span>](../api/conversation_delete.md) | <span data-ttu-id="be520-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="be520-118">None</span></span> |<span data-ttu-id="be520-119">Exclua um objeto conversation.</span><span class="sxs-lookup"><span data-stu-id="be520-119">Delete conversation object.</span></span> |
|[<span data-ttu-id="be520-120">Listar threads de conversas</span><span class="sxs-lookup"><span data-stu-id="be520-120">List conversation threads</span></span>](../api/conversation_list_threads.md) |<span data-ttu-id="be520-121">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="be520-121">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="be520-122">Obtenha todos os threads em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="be520-122">Get all the threads in a group conversation.</span></span>|
|[<span data-ttu-id="be520-123">Criar thread de conversas</span><span class="sxs-lookup"><span data-stu-id="be520-123">Create conversation thread</span></span>](../api/conversation_post_threads.md) |<span data-ttu-id="be520-124">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="be520-124">[conversationThread](conversationthread.md) collection</span></span>| <span data-ttu-id="be520-125">Crie um thread na conversa especificada.</span><span class="sxs-lookup"><span data-stu-id="be520-125">Create a thread in the specified conversation.</span></span>|

## <a name="properties"></a><span data-ttu-id="be520-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="be520-126">Properties</span></span>
| <span data-ttu-id="be520-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="be520-127">Property</span></span>     | <span data-ttu-id="be520-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="be520-128">Type</span></span>   |<span data-ttu-id="be520-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="be520-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be520-130">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="be520-130">hasAttachments</span></span>|<span data-ttu-id="be520-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="be520-131">Boolean</span></span>|<span data-ttu-id="be520-132">Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.</span><span class="sxs-lookup"><span data-stu-id="be520-132">Indicates whether any of the posts within this Conversation has at least one attachment.</span></span>|
|<span data-ttu-id="be520-133">id</span><span class="sxs-lookup"><span data-stu-id="be520-133">id</span></span>|<span data-ttu-id="be520-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="be520-134">String</span></span>|<span data-ttu-id="be520-p102">Identificador exclusivo de conversas. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="be520-p102">The conversations's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="be520-137">lastDeliveredDateTime</span><span class="sxs-lookup"><span data-stu-id="be520-137">lastDeliveredDateTime</span></span>|<span data-ttu-id="be520-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be520-138">DateTimeOffset</span></span>|<span data-ttu-id="be520-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="be520-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="be520-141">visualização</span><span class="sxs-lookup"><span data-stu-id="be520-141">preview</span></span>|<span data-ttu-id="be520-142">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="be520-142">String</span></span>|<span data-ttu-id="be520-143">Um breve resumo do corpo da última postagem nesta conversa.</span><span class="sxs-lookup"><span data-stu-id="be520-143">A short summary from the body of the latest post in this converstaion.</span></span>|
|<span data-ttu-id="be520-144">tópico</span><span class="sxs-lookup"><span data-stu-id="be520-144">topic</span></span>|<span data-ttu-id="be520-145">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="be520-145">String</span></span>|<span data-ttu-id="be520-p104">O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="be520-p104">The topic of the conversation. This property can be set when the conversation is created, but it cannot be updated.</span></span>|
|<span data-ttu-id="be520-148">uniqueSenders</span><span class="sxs-lookup"><span data-stu-id="be520-148">uniqueSenders</span></span>|<span data-ttu-id="be520-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="be520-149">String collection</span></span>|<span data-ttu-id="be520-150">Todos os usuários que enviaram uma mensagem para esta conversa.</span><span class="sxs-lookup"><span data-stu-id="be520-150">All the users that sent a message to this Conversation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be520-151">Relações</span><span class="sxs-lookup"><span data-stu-id="be520-151">Relationships</span></span>
| <span data-ttu-id="be520-152">Relação</span><span class="sxs-lookup"><span data-stu-id="be520-152">Relationship</span></span> | <span data-ttu-id="be520-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="be520-153">Type</span></span>   |<span data-ttu-id="be520-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="be520-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be520-155">threads</span><span class="sxs-lookup"><span data-stu-id="be520-155">threads</span></span>|<span data-ttu-id="be520-156">Coleção [conversationThread](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="be520-156">[conversationThread](conversationthread.md) collection</span></span>|<span data-ttu-id="be520-p105">Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="be520-p105">A collection of all the conversation threads in the conversation. A navigation property. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be520-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="be520-161">JSON representation</span></span>

<span data-ttu-id="be520-162">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="be520-162">Here is a JSON representation of the resource</span></span>

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
