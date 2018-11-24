# <a name="create-single-value-extended-property"></a><span data-ttu-id="d8313-101">Criar uma propriedade estendida de valor único</span><span class="sxs-lookup"><span data-stu-id="d8313-101">Create single-value extended property</span></span>

<span data-ttu-id="d8313-102">Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="d8313-102">Create one or more single-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="d8313-103">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="d8313-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="d8313-104">calendar</span><span class="sxs-lookup"><span data-stu-id="d8313-104">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="d8313-105">contact</span><span class="sxs-lookup"><span data-stu-id="d8313-105">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="d8313-106">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d8313-106">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="d8313-107">evento</span><span class="sxs-lookup"><span data-stu-id="d8313-107">event</span></span>](../resources/event.md)
- [<span data-ttu-id="d8313-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d8313-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="d8313-109">message</span><span class="sxs-lookup"><span data-stu-id="d8313-109">message</span></span>](../resources/message.md)

<span data-ttu-id="d8313-110">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="d8313-110">As well as the following group resources:</span></span>

- <span data-ttu-id="d8313-111">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-111">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="d8313-112">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-112">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="d8313-113">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="d8313-114">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="d8313-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8313-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8313-115">Permissions</span></span>
<span data-ttu-id="d8313-116">Dependendo do recurso, você está criando a propriedade estendida no e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d8313-116">Depending on the resource you're creating the extended property in and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="d8313-117">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d8313-117">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d8313-118">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-118">Supported resource</span></span> | <span data-ttu-id="d8313-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8313-119">Delegated (work or school account)</span></span> | <span data-ttu-id="d8313-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8313-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8313-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8313-121">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="d8313-122">calendar</span><span class="sxs-lookup"><span data-stu-id="d8313-122">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="d8313-123">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-123">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8313-124">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-124">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8313-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-125">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="d8313-126">contato</span><span class="sxs-lookup"><span data-stu-id="d8313-126">contact</span></span>](../resources/contact.md) | <span data-ttu-id="d8313-127">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-127">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8313-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-128">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8313-129">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-129">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d8313-130">contactFolder</span><span class="sxs-lookup"><span data-stu-id="d8313-130">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="d8313-131">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-131">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8313-132">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-132">Contacts.ReadWrite</span></span> | <span data-ttu-id="d8313-133">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-133">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="d8313-134">evento</span><span class="sxs-lookup"><span data-stu-id="d8313-134">event</span></span>](../resources/event.md) | <span data-ttu-id="d8313-135">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-135">Calendars.ReadWrite</span></span> | <span data-ttu-id="d8313-136">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-136">Calendars.ReadWrite</span></span> |  <span data-ttu-id="d8313-137">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-137">Calendars.ReadWrite</span></span>|
| <span data-ttu-id="d8313-138">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-138">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="d8313-139">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8313-139">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8313-140">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-140">Not supported</span></span> | <span data-ttu-id="d8313-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-141">Not supported</span></span> |
| <span data-ttu-id="d8313-142">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-142">group [event](../resources/event.md)</span></span> | <span data-ttu-id="d8313-143">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8313-143">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8313-144">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-144">Not supported</span></span> | <span data-ttu-id="d8313-145">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-145">Not supported</span></span> |
| <span data-ttu-id="d8313-146">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-146">group [post](../resources/post.md)</span></span> | <span data-ttu-id="d8313-147">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8313-147">Group.ReadWrite.All</span></span> | <span data-ttu-id="d8313-148">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-148">Not supported</span></span> | <span data-ttu-id="d8313-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d8313-149">Not supported</span></span> |
| [<span data-ttu-id="d8313-150">mailFolder</span><span class="sxs-lookup"><span data-stu-id="d8313-150">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="d8313-151">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-151">Mail.ReadWrite</span></span> | <span data-ttu-id="d8313-152">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-152">Mail.ReadWrite</span></span> | <span data-ttu-id="d8313-153">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-153">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="d8313-154">mensagem</span><span class="sxs-lookup"><span data-stu-id="d8313-154">message</span></span>](../resources/message.md) | <span data-ttu-id="d8313-155">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-155">Mail.ReadWrite</span></span> | <span data-ttu-id="d8313-156">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-156">Mail.ReadWrite</span></span> | <span data-ttu-id="d8313-157">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8313-157">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8313-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8313-158">HTTP request</span></span>
<span data-ttu-id="d8313-159">Você pode criar propriedades estendidas em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="d8313-159">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="d8313-p102">Para criar uma ou mais propriedades estendidas em uma _nova_ instância de recurso, use a mesma solicitação REST válida para a criação da instância e inclua as propriedades da nova instância de recurso _e a propriedade estendida_ no corpo da solicitação. Observe que alguns recursos dão suporte à criação de mais de uma maneira. Para saber mais sobre como criar essas instâncias de recurso, confira os tópicos correspondentes para a criação de [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md) e [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="d8313-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="d8313-163">Veja a seguir a sintaxe das solicitações.</span><span class="sxs-lookup"><span data-stu-id="d8313-163">The following is the syntax of the requests.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

<span data-ttu-id="d8313-164">Para criar uma ou mais propriedades estendidas em uma instância de recurso existente, especifique essa instância na solicitação e inclua a propriedade estendida no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8313-164">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="d8313-165">**Observação** Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="d8313-165">**Note** You cannot create an extended property in an existing group post.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8313-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8313-166">Request headers</span></span>
| <span data-ttu-id="d8313-167">Nome</span><span class="sxs-lookup"><span data-stu-id="d8313-167">Name</span></span>       | <span data-ttu-id="d8313-168">Valor</span><span class="sxs-lookup"><span data-stu-id="d8313-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d8313-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8313-169">Authorization</span></span> | <span data-ttu-id="d8313-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8313-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8313-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8313-172">Content-Type</span></span> | <span data-ttu-id="d8313-173">application/json</span><span class="sxs-lookup"><span data-stu-id="d8313-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8313-174">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8313-174">Request body</span></span>

<span data-ttu-id="d8313-175">Forneça um corpo JSON de cada objeto [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) na propriedade da coleção **singleValueExtendedProperties** da instância do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8313-175">Provide a JSON body of each [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object in the **singleValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="d8313-176">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8313-176">Property</span></span>|<span data-ttu-id="d8313-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8313-177">Type</span></span>|<span data-ttu-id="d8313-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8313-178">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d8313-179">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="d8313-179">singleValueExtendedProperties</span></span>|<span data-ttu-id="d8313-180">Coleção [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)</span><span class="sxs-lookup"><span data-stu-id="d8313-180">[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="d8313-181">Uma matriz de uma ou mais propriedades estendidas de valor único.</span><span class="sxs-lookup"><span data-stu-id="d8313-181">An array of one or more single-valued extended properties.</span></span> |
|<span data-ttu-id="d8313-182">id</span><span class="sxs-lookup"><span data-stu-id="d8313-182">id</span></span>|<span data-ttu-id="d8313-183">String</span><span class="sxs-lookup"><span data-stu-id="d8313-183">String</span></span>|<span data-ttu-id="d8313-p104">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique isso para identificar a propriedade. Deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8313-p104">For each property in the **singleValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="d8313-188">valor</span><span class="sxs-lookup"><span data-stu-id="d8313-188">value</span></span>|<span data-ttu-id="d8313-189">string</span><span class="sxs-lookup"><span data-stu-id="d8313-189">string</span></span>|<span data-ttu-id="d8313-p105">Para cada propriedade na coleção **singleValueExtendedProperties**, especifique o valor da propriedade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8313-p105">For each property in the **singleValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="d8313-192">Ao criar uma propriedade estendida em uma _nova_ instância de recurso, além da nova coleção **singleValueExtendedProperties**, forneça uma representação JSON dessa instância de recurso (ou seja, [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span><span class="sxs-lookup"><span data-stu-id="d8313-192">When creating an extended property in a _new_ resource instance, in addition to the new **singleValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>

## <a name="response"></a><span data-ttu-id="d8313-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8313-193">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="d8313-194">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="d8313-194">Response code</span></span>
<span data-ttu-id="d8313-195">Uma operação bem-sucedida na criação de uma propriedade estendida em uma nova instância de recurso retorna `201 Created`, exceto em uma nova postagem de grupo. Dependendo do método usado, a operação pode retornar `200 OK` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d8313-195">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="d8313-196">Em uma instância de recurso existente, uma operação de criação bem-sucedida retorna `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d8313-196">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="d8313-197">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="d8313-197">Response body</span></span>

<span data-ttu-id="d8313-p106">Ao criar uma propriedade estendida, a resposta inclui apenas a instância nova ou existente, mas não a nova propriedade estendida. Para ver a propriedade estendida recém-criada, [obtenha a instância expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="d8313-p106">When creating an extended property, the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="d8313-200">Ao criar uma propriedade estendida em uma _nova_ [postagem de grupo](../resources/post.md) respondendo a um thread ou postagem, a resposta inclui um código de resposta, mas não a nova postagem nem a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="d8313-200">When creating an extended property in a _new_ [group post](../resources/post.md) by replying to a thread or post, the response includes only a response code but not the new post nor the extended property.</span></span>



## <a name="example"></a><span data-ttu-id="d8313-201">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8313-201">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d8313-202">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="d8313-202">Request 1</span></span>

<span data-ttu-id="d8313-p107">O primeiro exemplo cria um novo evento e uma propriedade de valor único estendida na mesma operação POST. Além das propriedades que você normalmente incluiria para um novo evento, o corpo da solicitação inclui a coleção **singleValueExtendedProperties**, que contém uma propriedade estendida de valor único e as seguintes informações sobre a propriedade:</span><span class="sxs-lookup"><span data-stu-id="d8313-p107">The first example creates a new event and a single-value extended property in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **singleValueExtendedProperties** collection that contains one single-value extended property, and the following for the property:</span></span>
- <span data-ttu-id="d8313-205">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Fun`.</span><span class="sxs-lookup"><span data-stu-id="d8313-205">**id** specifies the property type as `String`, the GUID, and the property named `Fun`.</span></span>
- <span data-ttu-id="d8313-206">**value** especifica `Food` como o valor da propriedade `Fun`.</span><span class="sxs-lookup"><span data-stu-id="d8313-206">**value** specifies `Food` as the value of the `Fun` property.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Celebrate Thanksgiving",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together!"
  },
  "start": {
      "dateTime": "2015-11-26T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-26T23:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    }
  ],
  "singleValueExtendedProperties": [
     {
           "id":"String {66f5a359-4659-4830-9070-00040ec6ac6e} Name Fun",
           "value":"Food"
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="d8313-207">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="d8313-207">Response 1</span></span>

<span data-ttu-id="d8313-p108">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 201 Created` e inclui o novo evento em seu corpo, semelhante à resposta da [criação de apenas um evento](../api/user_post_events.md). A resposta não inclui propriedades estendidas recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="d8313-p108">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="d8313-210">Para ver a propriedade estendida recém-criada, [obtenha o evento expandido com a propriedade estendida](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="d8313-210">To see the newly created extended property, [get the event expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="d8313-211">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="d8313-211">Request 2</span></span>

<span data-ttu-id="d8313-p109">O segundo exemplo cria uma propriedade estendido de valor único para a mensagem especificada existente. A propriedade estendida é o único elemento na matriz **singleValueExtendedProperties**. O corpo da solicitação inclui o seguinte para essa propriedade estendida:</span><span class="sxs-lookup"><span data-stu-id="d8313-p109">The second example creates one single-value extended property for the specified existing message. That extended property is the only element in the **singleValueExtendedProperties** array. The request body includes the following for the extended property:</span></span>
- <span data-ttu-id="d8313-215">**id** especifica o tipo de propriedade como `String`, o GUID e a propriedade nomeada `Color`.</span><span class="sxs-lookup"><span data-stu-id="d8313-215">**id** specifies the property type as `String`, the GUID, and the property named `Color`.</span></span>
- <span data-ttu-id="d8313-216">**value** especifica `Green` como o valor da propriedade `Color`.</span><span class="sxs-lookup"><span data-stu-id="d8313-216">**value** specifies `Green` as the value of the `Color` property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2_bs88AACHsLqWAAA=

Content-Type: application/json

{
  "singleValueExtendedProperties": [
      {
         "id":"String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
         "value":"Green"
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="d8313-217">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="d8313-217">Response 2</span></span>

<span data-ttu-id="d8313-p110">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e inclui a mensagem especificada em seu corpo, semelhante à resposta da [atualização de uma mensagem](../api/message_update.md). A resposta não inclui a propriedade estendida recém-criada.</span><span class="sxs-lookup"><span data-stu-id="d8313-p110">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="d8313-220">Para ver a propriedade estendida recém-criada, [obtenha a mensagem expandida com a propriedade estendida](../api/singlevaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="d8313-220">To see the newly created extended property, [get the message expanded with the extended property](../api/singlevaluelegacyextendedproperty_get.md).</span></span>

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

