---
title: tipo de recurso post
description: Representa um item Post individual em uma entidade conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 838be4b5a21e2117fd06d33c62c94f1ae6488794
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720785"
---
# <a name="post-resource-type"></a><span data-ttu-id="68431-103">tipo de recurso post</span><span class="sxs-lookup"><span data-stu-id="68431-103">post resource type</span></span>

<span data-ttu-id="68431-104">Namespace: microsoft.graph Representa um item Post individual dentro de uma [entidade conversationThread.](conversationthread.md)</span><span class="sxs-lookup"><span data-stu-id="68431-104">Namespace: microsoft.graph Represents an individual Post item within a [conversationThread](conversationthread.md) entity.</span></span>

<span data-ttu-id="68431-105">Embora você não possa criar explicitamente uma postagem, seguir um destes procedimentos criaria uma postagem:</span><span class="sxs-lookup"><span data-stu-id="68431-105">Even though you cannot explicitly create a post, doing any of the following would create a post:</span></span>

- [<span data-ttu-id="68431-106">Responder a uma postagem existente</span><span class="sxs-lookup"><span data-stu-id="68431-106">Reply to an existing post</span></span>](../api/post-reply.md) 
- [<span data-ttu-id="68431-107">Responder a um thread existente</span><span class="sxs-lookup"><span data-stu-id="68431-107">Reply to an existing thread</span></span>](../api/conversationthread-reply.md) 
- [<span data-ttu-id="68431-108">Criar um thread em uma nova conversa</span><span class="sxs-lookup"><span data-stu-id="68431-108">Create a thread in a new conversation</span></span>](../api/group-post-threads.md)
- [<span data-ttu-id="68431-109">Criar uma nova conversa</span><span class="sxs-lookup"><span data-stu-id="68431-109">Create a new conversation</span></span>](../api/group-post-conversations.md)

<span data-ttu-id="68431-110">Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](/graph/extensibility-overview).</span><span class="sxs-lookup"><span data-stu-id="68431-110">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="68431-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="68431-111">Methods</span></span>

| <span data-ttu-id="68431-112">Método</span><span class="sxs-lookup"><span data-stu-id="68431-112">Method</span></span>       | <span data-ttu-id="68431-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68431-113">Return Type</span></span>  |<span data-ttu-id="68431-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="68431-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68431-115">Listar postagens</span><span class="sxs-lookup"><span data-stu-id="68431-115">List posts</span></span>](../api/conversationthread-list-posts.md) | [<span data-ttu-id="68431-116">post</span><span class="sxs-lookup"><span data-stu-id="68431-116">post</span></span>](post.md) |<span data-ttu-id="68431-117">Obtenha as postagens do thread especificado.</span><span class="sxs-lookup"><span data-stu-id="68431-117">Get the posts of the specified thread.</span></span> |
|[<span data-ttu-id="68431-118">Obter postagem</span><span class="sxs-lookup"><span data-stu-id="68431-118">Get post</span></span>](../api/post-get.md) | [<span data-ttu-id="68431-119">post</span><span class="sxs-lookup"><span data-stu-id="68431-119">post</span></span>](post.md) |<span data-ttu-id="68431-120">Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado.</span><span class="sxs-lookup"><span data-stu-id="68431-120">Get the properties and relationships of a post in a specified thread.</span></span>|
|[<span data-ttu-id="68431-121">Responder</span><span class="sxs-lookup"><span data-stu-id="68431-121">Reply</span></span>](../api/post-reply.md)|<span data-ttu-id="68431-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="68431-122">None</span></span>|<span data-ttu-id="68431-123">Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.</span><span class="sxs-lookup"><span data-stu-id="68431-123">Reply to a post and add a new post to the specified thread in a group conversation.</span></span>|
|[<span data-ttu-id="68431-124">Encaminhar</span><span class="sxs-lookup"><span data-stu-id="68431-124">Forward</span></span>](../api/post-forward.md)|<span data-ttu-id="68431-125">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="68431-125">None</span></span>|<span data-ttu-id="68431-126">Encaminhe uma postagem para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="68431-126">Forward a post to a recipient.</span></span>|
|<span data-ttu-id="68431-127">**Anexos**</span><span class="sxs-lookup"><span data-stu-id="68431-127">**Attachments**</span></span>| | |
|[<span data-ttu-id="68431-128">List attachments</span><span class="sxs-lookup"><span data-stu-id="68431-128">List attachments</span></span>](../api/post-list-attachments.md) |<span data-ttu-id="68431-129">Coleção [anexo](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="68431-129">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="68431-130">Obtenha todos os anexos em uma postagem.</span><span class="sxs-lookup"><span data-stu-id="68431-130">Get all attachments on a post.</span></span>|
|[<span data-ttu-id="68431-131">Add attachment</span><span class="sxs-lookup"><span data-stu-id="68431-131">Add attachment</span></span>](../api/post-post-attachments.md) |[<span data-ttu-id="68431-132">attachment</span><span class="sxs-lookup"><span data-stu-id="68431-132">attachment</span></span>](attachment.md)| <span data-ttu-id="68431-133">Adicione um anexo a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="68431-133">Add an attachment to a post.</span></span> |
|<span data-ttu-id="68431-134">**Extensões abertas**</span><span class="sxs-lookup"><span data-stu-id="68431-134">**Open extensions**</span></span>| | |
|[<span data-ttu-id="68431-135">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="68431-135">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="68431-136">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="68431-136">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="68431-137">Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="68431-137">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="68431-138">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="68431-138">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="68431-139">Coleção [openTypeExtension](opentypeextension.md)</span><span class="sxs-lookup"><span data-stu-id="68431-139">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="68431-140">Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="68431-140">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="68431-141">**Extensões de esquema**</span><span class="sxs-lookup"><span data-stu-id="68431-141">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="68431-142">Adicionar valores de extensões de esquema</span><span class="sxs-lookup"><span data-stu-id="68431-142">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="68431-143">Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.</span><span class="sxs-lookup"><span data-stu-id="68431-143">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="68431-144">**Propriedades estendidas**</span><span class="sxs-lookup"><span data-stu-id="68431-144">**Extended properties**</span></span>| | |
|[<span data-ttu-id="68431-145">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="68431-145">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="68431-146">post</span><span class="sxs-lookup"><span data-stu-id="68431-146">post</span></span>](post.md)  |<span data-ttu-id="68431-147">Criar uma ou mais propriedades estendidas de valor único em uma postagem nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="68431-147">Create one or more single-value extended properties in a new or existing post.</span></span>   |
|[<span data-ttu-id="68431-148">Obter postagem com propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="68431-148">Get post with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="68431-149">post</span><span class="sxs-lookup"><span data-stu-id="68431-149">post</span></span>](post.md) | <span data-ttu-id="68431-150">Obtenha postagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="68431-150">Get posts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="68431-151">Criar propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="68431-151">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="68431-152">post</span><span class="sxs-lookup"><span data-stu-id="68431-152">post</span></span>](post.md) | <span data-ttu-id="68431-153">Crie uma ou mais propriedades estendidas de vários valores em uma postagem nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="68431-153">Create one or more multi-value extended properties in a new or existing post.</span></span>  |
|[<span data-ttu-id="68431-154">Obter postagem com propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="68431-154">Get post with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="68431-155">post</span><span class="sxs-lookup"><span data-stu-id="68431-155">post</span></span>](post.md) | <span data-ttu-id="68431-156">Obtenha uma postagem que contenha uma propriedade estendida de vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="68431-156">Get a post that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="68431-157">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68431-157">Properties</span></span>
| <span data-ttu-id="68431-158">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68431-158">Property</span></span>     | <span data-ttu-id="68431-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="68431-159">Type</span></span>   |<span data-ttu-id="68431-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="68431-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68431-161">corpo</span><span class="sxs-lookup"><span data-stu-id="68431-161">body</span></span>|[<span data-ttu-id="68431-162">itemBody</span><span class="sxs-lookup"><span data-stu-id="68431-162">itemBody</span></span>](itembody.md)|<span data-ttu-id="68431-p101">O conteúdo da postagem. Esta é uma propriedade padrão. Esta propriedade pode ser nula.</span><span class="sxs-lookup"><span data-stu-id="68431-p101">The contents of the post. This is a default property. This property can be null.</span></span>|
|<span data-ttu-id="68431-166">Categorias</span><span class="sxs-lookup"><span data-stu-id="68431-166">categories</span></span>|<span data-ttu-id="68431-167">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="68431-167">String collection</span></span>|<span data-ttu-id="68431-168">As categorias associadas à postagem.</span><span class="sxs-lookup"><span data-stu-id="68431-168">The categories associated with the post.</span></span>|
|<span data-ttu-id="68431-169">changeKey</span><span class="sxs-lookup"><span data-stu-id="68431-169">changeKey</span></span>|<span data-ttu-id="68431-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68431-170">String</span></span>|<span data-ttu-id="68431-p102">Identifica a versão da postagem. Toda vez que a postagem muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.</span><span class="sxs-lookup"><span data-stu-id="68431-p102">Identifies the version of the post. Every time the post is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="68431-174">conversationId</span><span class="sxs-lookup"><span data-stu-id="68431-174">conversationId</span></span>|<span data-ttu-id="68431-175">String</span><span class="sxs-lookup"><span data-stu-id="68431-175">String</span></span>|<span data-ttu-id="68431-p103">ID exclusiva da conversa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68431-p103">Unique ID of the conversation. Read-only.</span></span>|
|<span data-ttu-id="68431-178">conversationThreadId</span><span class="sxs-lookup"><span data-stu-id="68431-178">conversationThreadId</span></span>|<span data-ttu-id="68431-179">String</span><span class="sxs-lookup"><span data-stu-id="68431-179">String</span></span>|<span data-ttu-id="68431-p104">ID exclusiva do thread de conversa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68431-p104">Unique ID of the conversation thread. Read-only.</span></span>|
|<span data-ttu-id="68431-182">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="68431-182">createdDateTime</span></span>|<span data-ttu-id="68431-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68431-183">DateTimeOffset</span></span>|<span data-ttu-id="68431-184">Especifica quando a postagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="68431-184">Specifies when the post was created.</span></span> <span data-ttu-id="68431-185">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="68431-185">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68431-186">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="68431-186">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="68431-187">from</span><span class="sxs-lookup"><span data-stu-id="68431-187">from</span></span>|[<span data-ttu-id="68431-188">recipient</span><span class="sxs-lookup"><span data-stu-id="68431-188">recipient</span></span>](recipient.md)|<span data-ttu-id="68431-p106">Usado em cenários de acesso de representante. Indica quem postou a mensagem em nome de outro usuário. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="68431-p106">Used in delegate access scenarios. Indicates who posted the message on behalf of another user. This is a default property.</span></span>|
|<span data-ttu-id="68431-192">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="68431-192">hasAttachments</span></span>|<span data-ttu-id="68431-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="68431-193">Boolean</span></span>|<span data-ttu-id="68431-p107">Indica se a postagem tem pelo menos um anexo. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="68431-p107">Indicates whether the post has at least one attachment. This is a default property.</span></span>|
|<span data-ttu-id="68431-196">id</span><span class="sxs-lookup"><span data-stu-id="68431-196">id</span></span>|<span data-ttu-id="68431-197">String</span><span class="sxs-lookup"><span data-stu-id="68431-197">String</span></span>| <span data-ttu-id="68431-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68431-198">Read-only.</span></span>|
|<span data-ttu-id="68431-199">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68431-199">lastModifiedDateTime</span></span>|<span data-ttu-id="68431-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68431-200">DateTimeOffset</span></span>|<span data-ttu-id="68431-201">Especifica quando a postagem foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="68431-201">Specifies when the post was last modified.</span></span> <span data-ttu-id="68431-202">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="68431-202">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68431-203">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="68431-203">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="68431-204">newParticipants</span><span class="sxs-lookup"><span data-stu-id="68431-204">newParticipants</span></span>|<span data-ttu-id="68431-205">Coleção [recipient](recipient.md)</span><span class="sxs-lookup"><span data-stu-id="68431-205">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="68431-206">Participantes da conversa que foram adicionados ao thread como parte desta postagem.</span><span class="sxs-lookup"><span data-stu-id="68431-206">Conversation participants that were added to the thread as part of this post.</span></span>|
|<span data-ttu-id="68431-207">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="68431-207">receivedDateTime</span></span>|<span data-ttu-id="68431-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68431-208">DateTimeOffset</span></span>|<span data-ttu-id="68431-209">Especifica quando a postagem foi recebida.</span><span class="sxs-lookup"><span data-stu-id="68431-209">Specifies when the post was received.</span></span> <span data-ttu-id="68431-210">O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="68431-210">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68431-211">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="68431-211">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="68431-212">sender</span><span class="sxs-lookup"><span data-stu-id="68431-212">sender</span></span>|[<span data-ttu-id="68431-213">recipient</span><span class="sxs-lookup"><span data-stu-id="68431-213">recipient</span></span>](recipient.md)|<span data-ttu-id="68431-p110">Contém o endereço do remetente. O valor de Sender será considerado o endereço do usuário autenticado caso o remetente não seja especificado. Esta é uma propriedade padrão.</span><span class="sxs-lookup"><span data-stu-id="68431-p110">Contains the address of the sender. The value of Sender is assumed to be the address of the authenticated user in the case when Sender is not specified. This is a default property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68431-217">Relações</span><span class="sxs-lookup"><span data-stu-id="68431-217">Relationships</span></span>
| <span data-ttu-id="68431-218">Relação</span><span class="sxs-lookup"><span data-stu-id="68431-218">Relationship</span></span> | <span data-ttu-id="68431-219">Tipo</span><span class="sxs-lookup"><span data-stu-id="68431-219">Type</span></span>   |<span data-ttu-id="68431-220">Descrição</span><span class="sxs-lookup"><span data-stu-id="68431-220">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68431-221">attachments</span><span class="sxs-lookup"><span data-stu-id="68431-221">attachments</span></span>|<span data-ttu-id="68431-222">Coleção [Attachment](attachment.md)</span><span class="sxs-lookup"><span data-stu-id="68431-222">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="68431-p111">Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="68431-p111">Read-only. Nullable.</span></span>|
|<span data-ttu-id="68431-225">extensions</span><span class="sxs-lookup"><span data-stu-id="68431-225">extensions</span></span>|<span data-ttu-id="68431-226">Coleção [Extension](extension.md)</span><span class="sxs-lookup"><span data-stu-id="68431-226">[Extension](extension.md) collection</span></span>|<span data-ttu-id="68431-227">A coleção de extensões abertas definidas para a postagem.</span><span class="sxs-lookup"><span data-stu-id="68431-227">The collection of open extensions defined for the post.</span></span> <span data-ttu-id="68431-228">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68431-228">Read-only.</span></span> <span data-ttu-id="68431-229">Anulável.</span><span class="sxs-lookup"><span data-stu-id="68431-229">Nullable.</span></span>|
|<span data-ttu-id="68431-230">inReplyTo</span><span class="sxs-lookup"><span data-stu-id="68431-230">inReplyTo</span></span>|[<span data-ttu-id="68431-231">post</span><span class="sxs-lookup"><span data-stu-id="68431-231">post</span></span>](post.md)| <span data-ttu-id="68431-232">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="68431-232">Read-only.</span></span>|
|<span data-ttu-id="68431-233">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="68431-233">multiValueExtendedProperties</span></span>|<span data-ttu-id="68431-234">Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="68431-234">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="68431-p113">A coleção de propriedades estendidas de vários valores definidas para a postagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="68431-p113">The collection of multi-value extended properties defined for the post. Read-only. Nullable.</span></span>|
|<span data-ttu-id="68431-238">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="68431-238">singleValueExtendedProperties</span></span>|<span data-ttu-id="68431-239">Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="68431-239">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="68431-p114">A coleção de propriedades estendidas de valor único definidas para a postagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="68431-p114">The collection of single-value extended properties defined for the post. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68431-243">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68431-243">JSON representation</span></span>

<span data-ttu-id="68431-244">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="68431-244">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="68431-245">Confira também</span><span class="sxs-lookup"><span data-stu-id="68431-245">See also</span></span>

- [<span data-ttu-id="68431-246">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="68431-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="68431-247">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="68431-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="68431-248">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="68431-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

