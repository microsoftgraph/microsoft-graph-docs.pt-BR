# <a name="create-multi-value-extended-property"></a><span data-ttu-id="56994-101">Criar uma propriedade estendida de vários valores</span><span class="sxs-lookup"><span data-stu-id="56994-101">Create multi-value extended property</span></span>

<span data-ttu-id="56994-102">Crie uma ou mais propriedades estendidas de vários valores em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="56994-102">Create one or more multi-value extended properties in a new or existing instance of a resource.</span></span> 

<span data-ttu-id="56994-103">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="56994-103">The following user resources are supported:</span></span>

- [<span data-ttu-id="56994-104">message</span><span class="sxs-lookup"><span data-stu-id="56994-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="56994-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="56994-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="56994-106">event</span><span class="sxs-lookup"><span data-stu-id="56994-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="56994-107">calendar</span><span class="sxs-lookup"><span data-stu-id="56994-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="56994-108">contact</span><span class="sxs-lookup"><span data-stu-id="56994-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="56994-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="56994-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="56994-110">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="56994-110">As well as the following group resources:</span></span>

- <span data-ttu-id="56994-111">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="56994-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="56994-112">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="56994-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="56994-113">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="56994-113">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="56994-114">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="56994-114">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="56994-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="56994-115">Permissions</span></span>
<span data-ttu-id="56994-p101">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso no qual você está criando a propriedade estendida. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="56994-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extended property in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="56994-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56994-118">Mail.ReadWrite</span></span>
- <span data-ttu-id="56994-119">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56994-119">Calendars.ReadWrite</span></span>
- <span data-ttu-id="56994-120">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56994-120">Contacts.ReadWrite</span></span>
- <span data-ttu-id="56994-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56994-121">Group.ReadWrite.All</span></span>
 
## <a name="http-request"></a><span data-ttu-id="56994-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56994-122">HTTP request</span></span>
<span data-ttu-id="56994-123">Você pode criar propriedades estendidas em uma instância de recurso nova ou existente.</span><span class="sxs-lookup"><span data-stu-id="56994-123">You can create extended properties in a new or existing resource instance.</span></span>

<span data-ttu-id="56994-p102">Para criar uma ou mais propriedades estendidas em uma _nova_ instância de recurso, use a mesma solicitação REST válida para a criação da instância e inclua as propriedades da nova instância de recurso _e a propriedade estendida_ no corpo da solicitação. Observe que alguns recursos dão suporte à criação de mais de uma maneira. Para saber mais sobre como criar essas instâncias de recurso, confira os tópicos correspondentes para a criação de [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md) e [group post](../resources/post.md).</span><span class="sxs-lookup"><span data-stu-id="56994-p102">To create one or more extended properties in a _new_ resource instance, use the same REST request as creating the instance, and include the properties of the new resource instance _and extended property_ in the request body. Note that some resources support creation in more than one way. For more information on creating these resource instances, see the corresponding topics for creating a [message](../resources/message.md), [mailFolder](../api/user_post_mailfolders.md), [event](../api/user_post_events.md), [calendar](../api/user_post_calendars.md), [contact](../api/user_post_contacts.md), [contactFolder](../api/user_post_contactfolders.md), [group event](../api/group_post_events.md), and [group post](../resources/post.md).</span></span> 
 
<span data-ttu-id="56994-127">Veja a seguir a sintaxe das solicitações.</span><span class="sxs-lookup"><span data-stu-id="56994-127">The following is the syntax of the requests.</span></span> 

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

<span data-ttu-id="56994-128">Para criar uma ou mais propriedades estendidas em uma instância de recurso existente, especifique essa instância na solicitação e inclua a propriedade estendida no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56994-128">To create one or more extended properties in an existing resource instance, specify the instance in the request, and include the extended property in the request body.</span></span>

<span data-ttu-id="56994-129">**Observação** Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="56994-129">**Note** You cannot create an extended property in an existing group post.</span></span>

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

## <a name="request-headers"></a><span data-ttu-id="56994-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56994-130">Request headers</span></span>
| <span data-ttu-id="56994-131">Nome</span><span class="sxs-lookup"><span data-stu-id="56994-131">Name</span></span>       | <span data-ttu-id="56994-132">Valor</span><span class="sxs-lookup"><span data-stu-id="56994-132">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="56994-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="56994-133">Authorization</span></span> | <span data-ttu-id="56994-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56994-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56994-136">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56994-136">Content-Type</span></span> | <span data-ttu-id="56994-137">aplicativo/json</span><span class="sxs-lookup"><span data-stu-id="56994-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="56994-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56994-138">Request body</span></span>

<span data-ttu-id="56994-139">Forneça um corpo JSON de cada objeto [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) na propriedade da coleção **multiValueExtendedProperties** da instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="56994-139">Provide a JSON body of each [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object in the **multiValueExtendedProperties** collection property of the resource instance.</span></span>

|<span data-ttu-id="56994-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56994-140">Property</span></span>|<span data-ttu-id="56994-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="56994-141">Type</span></span>|<span data-ttu-id="56994-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="56994-142">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="56994-143">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="56994-143">multiValueExtendedProperties</span></span>|<span data-ttu-id="56994-144">Coleção [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)</span><span class="sxs-lookup"><span data-stu-id="56994-144">[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection</span></span>| <span data-ttu-id="56994-145">Uma matriz de uma ou mais propriedades estendidas de vários valores.</span><span class="sxs-lookup"><span data-stu-id="56994-145">An array of one or more multi-valued extended properties.</span></span> |
|<span data-ttu-id="56994-146">id</span><span class="sxs-lookup"><span data-stu-id="56994-146">id</span></span>|<span data-ttu-id="56994-147">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="56994-147">String</span></span>|<span data-ttu-id="56994-p104">Para cada propriedade na coleção **multiValueExtendedProperties**, especifique isso para identificar a propriedade. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56994-p104">For each property in the **multiValueExtendedProperties** collection, specify this to identify the property. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="56994-152">valor</span><span class="sxs-lookup"><span data-stu-id="56994-152">value</span></span>|<span data-ttu-id="56994-153">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="56994-153">string</span></span>|<span data-ttu-id="56994-p105">Para cada propriedade na coleção **multiValueExtendedProperties**, especifique o valor da propriedade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56994-p105">For each property in the **multiValueExtendedProperties** collection, specify the property value. Required.</span></span>|

<span data-ttu-id="56994-156">Ao criar uma propriedade estendida em uma _nova_ instância de recurso, além da nova coleção **multiValueExtendedProperties**, forneça uma também uma representação JSON dessa instância de recurso (ou seja, [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.).</span><span class="sxs-lookup"><span data-stu-id="56994-156">When creating an extended property in a _new_ resource instance, in addition to the new **multiValueExtendedProperties** collection, provide a JSON representation of that resource instance (that is, a [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), etc.)</span></span>


## <a name="response"></a><span data-ttu-id="56994-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="56994-157">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="56994-158">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="56994-158">Response code</span></span>
<span data-ttu-id="56994-159">Uma operação bem-sucedida na criação de uma propriedade estendida em uma nova instância de recurso retorna `201 Created`, exceto em uma nova postagem de grupo. Dependendo do método usado, a operação pode retornar `200 OK` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="56994-159">An operation successful in creating an extended property in a new resource instance returns `201 Created`, except in a new group post, depending on the method used, the operation can return `200 OK` or `202 Accepted`.</span></span>

<span data-ttu-id="56994-160">Em uma instância de recurso existente, uma operação de criação bem-sucedida retorna `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="56994-160">In an existing resource instance, a successful create operation returns `200 OK`.</span></span> 


#### <a name="response-body"></a><span data-ttu-id="56994-161">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="56994-161">Response body</span></span>

<span data-ttu-id="56994-p106">Ao criar uma propriedade estendida em um recurso com suporte que não seja [group post](../resources/post.md), a resposta inclui apenas a instância nova ou existente, mas não a nova propriedade estendida. Para ver a propriedade estendida recém-criada, [obtenha a instância expandida com a propriedade estendida](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="56994-p106">When creating an extended property in a supported resource other than [group post](../resources/post.md), the response includes only the new or existing instance but not the new extended property. To see the newly created extended property, [get the instance expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>

<span data-ttu-id="56994-p107">Ao criar uma propriedade estendida em uma _nova_ postagem de grupo, a resposta inclui um código de resposta, mas não a nova postagem nem a propriedade estendida. Não é possível criar uma propriedade estendida em uma postagem de grupo existente.</span><span class="sxs-lookup"><span data-stu-id="56994-p107">When creating an extended property in a _new_ group post, the response includes only a response code but not the new post nor the extended property. You cannot create an extended property in an existing group post.</span></span>


## <a name="example"></a><span data-ttu-id="56994-166">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56994-166">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="56994-167">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="56994-167">Request 1</span></span>

<span data-ttu-id="56994-p108">O primeiro exemplo cria uma propriedade estendida de vários valores em um novo evento, tudo na mesma operação POST. Além das propriedades que você normalmente incluiria para um novo evento, o corpo da solicitação inclui a coleção **multiValueExtendedProperties**, que contém uma propriedade estendida. O corpo da solicitação inclui o seguinte para essa propriedade estendida de vários valores:</span><span class="sxs-lookup"><span data-stu-id="56994-p108">The first example creates a multi-value extended property in a new event all in the same POST operation. Apart from the properties you'd normally include for a new event, the request body includes the **multiValueExtendedProperties** collection which contains one extended property. The request body includes the following for that multi-value extended property:</span></span>

- <span data-ttu-id="56994-171">**id**, que especifica a propriedade como uma matriz de cadeias de caracteres com o GUID especificado e o nome `Recreation`.</span><span class="sxs-lookup"><span data-stu-id="56994-171">**id** which specifies the property as an array of strings with the specified GUID and the name `Recreation`.</span></span> 
- <span data-ttu-id="56994-172">**value**, que especifica `Recreation` como uma matriz de 3 valores de cadeia de caracteres, `["Food", "Hiking", "Swimming"]`.</span><span class="sxs-lookup"><span data-stu-id="56994-172">**value** which specifies `Recreation` as an array of 3 string values, `["Food", "Hiking", "Swimming"]`.</span></span>
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="56994-173">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="56994-173">Response 1</span></span>

<span data-ttu-id="56994-p109">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 201 Created` e inclui o novo evento em seu corpo, semelhante à resposta da [criação de apenas um evento](../api/user_post_events.md). A resposta não inclui propriedades estendidas recém-criadas.</span><span class="sxs-lookup"><span data-stu-id="56994-p109">A successful response is indicated by an `HTTP 201 Created` response code, and includes the new event in the response body, similar to the response from [creating just an event](../api/user_post_events.md). The response does not include any newly created extended properties.</span></span>

<span data-ttu-id="56994-176">Para ver a propriedade estendida recém-criada, [obtenha o evento expandido com a propriedade estendida](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="56994-176">To see the newly created extended property, [get the event expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


****

##### <a name="request-2"></a><span data-ttu-id="56994-177">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="56994-177">Request 2</span></span>

<span data-ttu-id="56994-p110">O segundo exemplo cria uma propriedade estendida de vários valores para a mensagem especificada. Essa propriedade estendida é o único elemento na coleção **multiValueExtendedProperties**. O corpo da solicitação inclui o seguinte para essa propriedade estendida:</span><span class="sxs-lookup"><span data-stu-id="56994-p110">The second example creates one multi-value extended property for the specified message. That extended property is the only element in the **multiValueExtendedProperties** collection. The request body includes the following for the extended property:</span></span>

- <span data-ttu-id="56994-181">**id** especifica a propriedade como uma matriz de cadeias de caracteres com o GUID especificado e o nome `Palette`.</span><span class="sxs-lookup"><span data-stu-id="56994-181">**id** specifies the property as an array of strings with the specified GUID and the name `Palette`.</span></span>
- <span data-ttu-id="56994-182">**value** especifica `Palette` como uma matriz de 3 valores de cadeia de caracteres, `["Green", "Aqua", "Blue"]`.</span><span class="sxs-lookup"><span data-stu-id="56994-182">**value** specifies `Palette` as an array of 3 string values, `["Green", "Aqua", "Blue"]`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="56994-183">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="56994-183">Response 2</span></span>

<span data-ttu-id="56994-p111">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK` e inclui a mensagem especificada em seu corpo, semelhante à resposta da [atualização de uma mensagem](../api/message_update.md). A resposta não inclui a propriedade estendida recém-criada.</span><span class="sxs-lookup"><span data-stu-id="56994-p111">A successful response is indicated by an `HTTP 200 OK` response code, and includes the specified message in the response body, similar to the response from [updating a message](../api/message_update.md). The response does not include the newly created extended property.</span></span>

<span data-ttu-id="56994-186">Para ver a propriedade estendida recém-criada, [obtenha a mensagem expandida com a propriedade estendida](../api/multivaluelegacyextendedproperty_get.md).</span><span class="sxs-lookup"><span data-stu-id="56994-186">To see the newly created extended property, [get the message expanded with the extended property](../api/multivaluelegacyextendedproperty_get.md).</span></span>


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




