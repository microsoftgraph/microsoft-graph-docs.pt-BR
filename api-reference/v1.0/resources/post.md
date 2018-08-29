# <a name="post-resource-type"></a><span data-ttu-id="96b90-101">tipo de recurso post</span><span class="sxs-lookup"><span data-stu-id="96b90-101">post resource type</span></span>
<span data-ttu-id="96b90-102">Representa um item Post individual em uma entidade [conversationThread](conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="96b90-102">Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="96b90-103">Embora você não possa criar explicitamente uma postagem, seguir um destes procedimentos criaria uma postagem:</span><span class="sxs-lookup"><span data-stu-id="96b90-103">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="96b90-104">Responder a uma postagem existente</span><span class="sxs-lookup"><span data-stu-id="96b90-104">Reply to an existing post</span></span>](../api/post_reply.md) 
- [<span data-ttu-id="96b90-105">Responder a um thread existente</span><span class="sxs-lookup"><span data-stu-id="96b90-105">Reply to an existing thread</span></span>](../api/conversationthread_reply.md) 
- [<span data-ttu-id="96b90-106">Criar um thread em uma nova conversa</span><span class="sxs-lookup"><span data-stu-id="96b90-106">Create a thread in a new conversation</span></span>](../api/group_post_threads.md)
- [<span data-ttu-id="96b90-107">Criar uma nova conversa</span><span class="sxs-lookup"><span data-stu-id="96b90-107">Create a new conversation</span></span>](../api/group_post_conversations.md)

<span data-ttu-id="96b90-108">Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).</span><span class="sxs-lookup"><span data-stu-id="96b90-108">This resource lets you add your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>

## <a name="methods"></a><span data-ttu-id="96b90-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="96b90-109">Methods</span></span>

| <span data-ttu-id="96b90-110">Método</span><span class="sxs-lookup"><span data-stu-id="96b90-110">Method</span></span>       | <span data-ttu-id="96b90-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="96b90-111">Return Type</span></span>  |<span data-ttu-id="96b90-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b90-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96b90-113">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="96b90-113">List posts</span></span>](../api/conversationthread_list_posts.md) | [<span data-ttu-id="96b90-114">post</span><span class="sxs-lookup"><span data-stu-id="96b90-114">post</span></span>](post.md) |<span data-ttu-id="96b90-115">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="96b90-115">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="96b90-116">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="96b90-116">Get post</span></span>](../api/post_get.md) | [<span data-ttu-id="96b90-117">post</span><span class="sxs-lookup"><span data-stu-id="96b90-117">post</span></span>](post.md) |<span data-ttu-id="96b90-118">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado.</span><span class="sxs-lookup"><span data-stu-id="96b90-118">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="96b90-119">Responder</span><span class="sxs-lookup"><span data-stu-id="96b90-119">Reply</span></span>](../api/post_reply.md)|<span data-ttu-id="96b90-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="96b90-120">None</span></span>|<span data-ttu-id="96b90-121">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="96b90-121">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="96b90-122">Encaminhar</span><span class="sxs-lookup"><span data-stu-id="96b90-122">Forward</span></span>](../api/post_forward.md)|<span data-ttu-id="96b90-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="96b90-123">None</span></span>|<span data-ttu-id="96b90-124">Encaminhe uma postagem para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="96b90-124">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="96b90-125">**Anexos**</span><span class="sxs-lookup"><span data-stu-id="96b90-125">**Attachments**</span></span>| | |
|[<span data-ttu-id="96b90-126">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="96b90-126">List attachments</span></span>](../api/post_list_attachments.md) |<span data-ttu-id="96b90-127">Coleção [attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-127">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="96b90-128">Obtenha todos os anexos em uma postagem.</span><span class="sxs-lookup"><span data-stu-id="96b90-128">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="96b90-129">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="96b90-129">Add attachment</span></span>](../api/post_post_attachments.md) |[<span data-ttu-id="96b90-130">attachment</span><span class="sxs-lookup"><span data-stu-id="96b90-130">attachment</span></span>](attachment.md)| <span data-ttu-id="96b90-131">Adicione um anexo a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="96b90-131">Add an attachment to a post.</span></span> |
|<span data-ttu-id="96b90-132">**Extensões abertas**</span><span class="sxs-lookup"><span data-stu-id="96b90-132">**Open extensions**</span></span>| | |
|[<span data-ttu-id="96b90-133">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="96b90-133">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="96b90-134">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="96b90-134">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="96b90-135">Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="96b90-135">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="96b90-136">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="96b90-136">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="96b90-137">Coleção [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-137">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="96b90-138">Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="96b90-138">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="96b90-139">**Extensões de esquema**</span><span class="sxs-lookup"><span data-stu-id="96b90-139">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="96b90-140">Adicionar valores de extensões de esquema</span><span class="sxs-lookup"><span data-stu-id="96b90-140">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="96b90-141">Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.</span><span class="sxs-lookup"><span data-stu-id="96b90-141">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="96b90-142">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="96b90-142">**Extended properties**</span></span>| | |
|[<span data-ttu-id="96b90-143">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="96b90-143">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="96b90-144">post</span><span class="sxs-lookup"><span data-stu-id="96b90-144">post</span></span>](post.md)  |<span data-ttu-id="96b90-145">Criar uma ou mais propriedades estendidas de valor único em uma postagem nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="96b90-145">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="96b90-146">Obter postagem com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="96b90-146">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="96b90-147">post</span><span class="sxs-lookup"><span data-stu-id="96b90-147">post</span></span>](post.md) | <span data-ttu-id="96b90-148">Obtenha postagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="96b90-148">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="96b90-149">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="96b90-149">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="96b90-150">post</span><span class="sxs-lookup"><span data-stu-id="96b90-150">post</span></span>](post.md) | <span data-ttu-id="96b90-151">Crie uma ou mais propriedades estendidas de vários valores em uma postagem nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="96b90-151">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="96b90-152">Obter postagem com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="96b90-152">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="96b90-153">post</span><span class="sxs-lookup"><span data-stu-id="96b90-153">post</span></span>](post.md) | <span data-ttu-id="96b90-154">Obtenha uma postagem que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="96b90-154">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="96b90-155">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96b90-155">Properties</span></span>
| <span data-ttu-id="96b90-156">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96b90-156">Property</span></span>     | <span data-ttu-id="96b90-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="96b90-157">Type</span></span>   |<span data-ttu-id="96b90-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b90-158">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96b90-159">body</span><span class="sxs-lookup"><span data-stu-id="96b90-159">body</span></span>|[<span data-ttu-id="96b90-160">itemBody</span><span class="sxs-lookup"><span data-stu-id="96b90-160">itemBody</span></span>](itembody.md)|<span data-ttu-id="96b90-p101">O conteúdo da postagem. Esta é uma propriedade padrão. Esta propriedade pode ser nula.</span><span class="sxs-lookup"><span data-stu-id="96b90-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="96b90-164">categories</span><span class="sxs-lookup"><span data-stu-id="96b90-164">categories</span></span>|<span data-ttu-id="96b90-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="96b90-165">String collection</span></span>|<span data-ttu-id="96b90-166">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="96b90-166">The categories associated with the post.</span></span>|
|<span data-ttu-id="96b90-167">changeKey</span><span class="sxs-lookup"><span data-stu-id="96b90-167">changeKey</span></span>|<span data-ttu-id="96b90-168">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="96b90-168">String</span></span>|<span data-ttu-id="96b90-p102">Identifica a versão da postagem. Toda vez que a postagem muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="96b90-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="96b90-172">conversationId</span><span class="sxs-lookup"><span data-stu-id="96b90-172">conversationId</span></span>|<span data-ttu-id="96b90-173">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="96b90-173">String</span></span>|<span data-ttu-id="96b90-p103">ID exclusiva da conversa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96b90-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="96b90-176">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="96b90-176">conversationThreadId</span></span>|<span data-ttu-id="96b90-177">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="96b90-177">String</span></span>|<span data-ttu-id="96b90-p104">ID exclusiva do thread de conversa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96b90-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="96b90-180">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96b90-180">createdDateTime</span></span>|<span data-ttu-id="96b90-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b90-181">DateTimeOffset</span></span>|<span data-ttu-id="96b90-p105">Especifica quando a postagem foi criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96b90-p105">Specifies when the post was created. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96b90-185">from</span><span class="sxs-lookup"><span data-stu-id="96b90-185">from</span></span>|[<span data-ttu-id="96b90-186">recipient</span><span class="sxs-lookup"><span data-stu-id="96b90-186">recipient</span></span>](recipient.md)|<span data-ttu-id="96b90-p106">Usado em cenários de acesso de representante. Indica quem postou a mensagem em nome de outro usuário. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="96b90-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="96b90-190">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="96b90-190">hasAttachments</span></span>|<span data-ttu-id="96b90-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="96b90-191">Boolean</span></span>|<span data-ttu-id="96b90-p107">Indica se a postagem tem pelo menos um anexo. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="96b90-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="96b90-194">id</span><span class="sxs-lookup"><span data-stu-id="96b90-194">id</span></span>|<span data-ttu-id="96b90-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96b90-195">String</span></span>| <span data-ttu-id="96b90-196">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96b90-196">Read-only.</span></span>|
|<span data-ttu-id="96b90-197">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96b90-197">lastModifiedDateTime</span></span>|<span data-ttu-id="96b90-198">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b90-198">DateTimeOffset</span></span>|<span data-ttu-id="96b90-p108">Especifica quando a postagem foi modificada pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96b90-p108">Specifies when the post was last modified. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96b90-202">newParticipants</span><span class="sxs-lookup"><span data-stu-id="96b90-202">newParticipants</span></span>|<span data-ttu-id="96b90-203">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-203">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="96b90-204">Participantes da conversa que foram adicionados ao thread como parte desta postagem.</span><span class="sxs-lookup"><span data-stu-id="96b90-204">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="96b90-205">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="96b90-205">receivedDateTime</span></span>|<span data-ttu-id="96b90-206">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b90-206">DateTimeOffset</span></span>|<span data-ttu-id="96b90-p109">Especifica quando a postagem foi recebida. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="96b90-p109">Specifies when the post was received. The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="96b90-210">sender</span><span class="sxs-lookup"><span data-stu-id="96b90-210">sender</span></span>|[<span data-ttu-id="96b90-211">recipient</span><span class="sxs-lookup"><span data-stu-id="96b90-211">recipient</span></span>](recipient.md)|<span data-ttu-id="96b90-p110">Contém o endereço do remetente. O valor de Sender será considerado o endereço do usuário autenticado caso o remetente não seja especificado. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="96b90-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96b90-215">Relações</span><span class="sxs-lookup"><span data-stu-id="96b90-215">Relationships</span></span>
| <span data-ttu-id="96b90-216">Relação</span><span class="sxs-lookup"><span data-stu-id="96b90-216">Relationship</span></span> | <span data-ttu-id="96b90-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="96b90-217">Type</span></span>   |<span data-ttu-id="96b90-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b90-218">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96b90-219">attachments</span><span class="sxs-lookup"><span data-stu-id="96b90-219">attachments</span></span>|<span data-ttu-id="96b90-220">Coleção [Attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-220">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="96b90-p111">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="96b90-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="96b90-223">extensions</span><span class="sxs-lookup"><span data-stu-id="96b90-223">extensions</span></span>|<span data-ttu-id="96b90-224">Coleção [Extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-224">[Extension](extension.md) collection</span></span>|<span data-ttu-id="96b90-p112">A coleção de extensões abertas definidas para a postagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="96b90-p112">The collection of open extensions defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="96b90-228">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="96b90-228">inReplyTo</span></span>|[<span data-ttu-id="96b90-229">post</span><span class="sxs-lookup"><span data-stu-id="96b90-229">post</span></span>](post.md)| <span data-ttu-id="96b90-230">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96b90-230">Read-only.</span></span>|
|<span data-ttu-id="96b90-231">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="96b90-231">multiValueExtendedProperties</span></span>|<span data-ttu-id="96b90-232">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-232">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="96b90-p113">A coleção de propriedades estendidas de vários valores definidas para a postagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="96b90-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="96b90-236">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="96b90-236">singleValueExtendedProperties</span></span>|<span data-ttu-id="96b90-237">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="96b90-237">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="96b90-p114">A coleção de propriedades estendidas de valor único definidas para a postagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="96b90-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96b90-241">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96b90-241">JSON representation</span></span>

<span data-ttu-id="96b90-242">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="96b90-242">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.post",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "inReplyTo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a><span data-ttu-id="96b90-243">Confira também</span><span class="sxs-lookup"><span data-stu-id="96b90-243">See also</span></span>

- [<span data-ttu-id="96b90-244">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="96b90-244">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="96b90-245">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="96b90-245">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="96b90-246">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="96b90-246">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
