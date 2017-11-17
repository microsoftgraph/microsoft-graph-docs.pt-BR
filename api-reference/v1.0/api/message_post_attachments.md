# <a name="add-attachment"></a><span data-ttu-id="badba-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="badba-101">Add attachment</span></span>

<span data-ttu-id="badba-102">Use esta API para adicionar um [anexo](../resources/attachment.md) a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="badba-102">Use this API to add an [attachment](../resources/attachment.md) to a message.</span></span> 

<span data-ttu-id="badba-103">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="badba-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="badba-104">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="badba-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="badba-105">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="badba-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="badba-106">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="badba-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="badba-107">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="badba-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

<span data-ttu-id="badba-108">Você pode adicionar um anexo a uma mensagem existente postando na seu coleção de anexos, ou pode adicionar um anexo a uma mensagem que está sendo [criada e enviada dinamicamente](../api/user_sendmail.md).</span><span class="sxs-lookup"><span data-stu-id="badba-108">You can add an attachment to an existing message by posting to its attachments collection, or you can add an attachment to a message that is being [created and sent on the fly](../api/user_sendmail.md).</span></span>

<span data-ttu-id="badba-109">Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="badba-109">Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="badba-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="badba-110">Permissions</span></span>
<span data-ttu-id="badba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="badba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="badba-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="badba-113">Permission type</span></span>      | <span data-ttu-id="badba-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="badba-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="badba-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="badba-115">Delegated (work or school account)</span></span> | <span data-ttu-id="badba-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="badba-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="badba-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="badba-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="badba-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="badba-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="badba-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="badba-119">Application</span></span> | <span data-ttu-id="badba-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="badba-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="badba-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="badba-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="badba-122">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="badba-122">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="badba-123">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="badba-123">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
POST /me/mailFolders/{id}/messages/{id}/attachments
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="badba-p102">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="badba-p102">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
POST /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
POST /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="badba-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="badba-126">Request headers</span></span>
| <span data-ttu-id="badba-127">Nome</span><span class="sxs-lookup"><span data-stu-id="badba-127">Name</span></span>       | <span data-ttu-id="badba-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="badba-128">Type</span></span> | <span data-ttu-id="badba-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="badba-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="badba-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="badba-130">Authorization</span></span>  | <span data-ttu-id="badba-131">string</span><span class="sxs-lookup"><span data-stu-id="badba-131">string</span></span>  | <span data-ttu-id="badba-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="badba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="badba-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="badba-134">Content-Type</span></span> | <span data-ttu-id="badba-135">string</span><span class="sxs-lookup"><span data-stu-id="badba-135">string</span></span>  | <span data-ttu-id="badba-p104">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="badba-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="badba-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="badba-138">Request body</span></span>
<span data-ttu-id="badba-139">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="badba-139">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="badba-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="badba-140">Response</span></span>

<span data-ttu-id="badba-141">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="badba-141">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="badba-142">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="badba-142">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="badba-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="badba-143">Request</span></span>
<span data-ttu-id="badba-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="badba-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "smile",
  "contentBytes": "R0lGODdhEAYEAA7"
}
```

<span data-ttu-id="badba-145">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="badba-145">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="badba-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="badba-146">Response</span></span>
<span data-ttu-id="badba-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="badba-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAttachment"
} -->
```http
HTTP 201 Created
Content-type: application/json
Content-length: 202

{
    "id": "AAMkADNkN2R",
    "lastModifiedDateTime": "2017-01-26T08:48:28Z",
    "name": "smile",
    "contentType": "image/gif",
    "size": 1008,
    "isInline": false,
    "contentId": null,
    "contentLocation": null,
    "contentBytes": "R0lGODdhEAYEAA7"
}

```

## <a name="example-item-attachment"></a><span data-ttu-id="badba-148">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="badba-148">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="badba-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="badba-149">Request</span></span>
<span data-ttu-id="badba-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="badba-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_message"
}-->

```
POST https://graph.microsoft.com/v1.0/me/messages/AAMkpsDRVK/attachments
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "Holiday event", 
  "item": {
    "@odata.type": "microsoft.graph.event",
    "subject": "Discuss gifts for children",
    "body": {
      "contentType": "HTML",
      "content": "Let's look for funding!"
    },
    "start": {
      "dateTime": "2016-12-02T18:00:00",
      "timeZone": "Pacific Standard Time"
    },
    "end": {
      "dateTime": "2016-12-02T19:00:00",
      "timeZone": "Pacific Standard Time"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="badba-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="badba-151">Response</span></span>
<span data-ttu-id="badba-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="badba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemAttachment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 162

{
  "id":"AAMkADNkNJp5JVnQIe9r0=",
  "lastModifiedDateTime":"2016-12-01T22:27:13Z",
  "name":"Holiday event",
  "contentType":null,
  "size":2473,
  "isInline":false
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
