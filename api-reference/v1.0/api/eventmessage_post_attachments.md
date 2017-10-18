# <a name="add-attachment"></a><span data-ttu-id="51e58-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="51e58-101">Add attachment</span></span>

<span data-ttu-id="51e58-102">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="51e58-102">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="51e58-103">Um anexo pode ser de um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="51e58-103">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="51e58-104">Um arquivo (recurso [fileAttachment](../resources/fileattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="51e58-104">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="51e58-105">Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md)).</span><span class="sxs-lookup"><span data-stu-id="51e58-105">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource)</span></span>
* <span data-ttu-id="51e58-106">Um link para um arquivo (recurso [referenceAttachment](../resources/referenceAttachment.md)).</span><span class="sxs-lookup"><span data-stu-id="51e58-106">A link to a file ([referenceAttachment](../resources/referenceAttachment.md) resource).</span></span>

<span data-ttu-id="51e58-107">Todos esses tipos de recursos de anexo são derivados do recurso [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="51e58-107">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="51e58-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="51e58-108">Permissions</span></span>
<span data-ttu-id="51e58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51e58-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51e58-111">Permission type</span></span>      | <span data-ttu-id="51e58-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51e58-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51e58-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51e58-113">Delegated (work or school account)</span></span> | <span data-ttu-id="51e58-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e58-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51e58-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51e58-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e58-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e58-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="51e58-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51e58-117">Application</span></span> | <span data-ttu-id="51e58-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="51e58-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="51e58-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51e58-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="51e58-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51e58-120">Request headers</span></span>
| <span data-ttu-id="51e58-121">Nome</span><span class="sxs-lookup"><span data-stu-id="51e58-121">Name</span></span>       | <span data-ttu-id="51e58-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e58-122">Type</span></span> | <span data-ttu-id="51e58-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e58-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51e58-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="51e58-124">Authorization</span></span>  | <span data-ttu-id="51e58-125">string</span><span class="sxs-lookup"><span data-stu-id="51e58-125">string</span></span>  | <span data-ttu-id="51e58-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e58-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51e58-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51e58-128">Content-Type</span></span> | <span data-ttu-id="51e58-129">string</span><span class="sxs-lookup"><span data-stu-id="51e58-129">string</span></span>  | <span data-ttu-id="51e58-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e58-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51e58-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51e58-132">Request body</span></span>
<span data-ttu-id="51e58-133">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="51e58-133">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="51e58-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e58-134">Response</span></span>

<span data-ttu-id="51e58-135">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51e58-135">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="51e58-136">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="51e58-136">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="51e58-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e58-137">Request</span></span>
<span data-ttu-id="51e58-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e58-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="51e58-139">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="51e58-139">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="51e58-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e58-140">Response</span></span>
<span data-ttu-id="51e58-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51e58-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="51e58-144">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="51e58-144">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="51e58-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e58-145">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="51e58-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e58-146">Response</span></span>
<span data-ttu-id="51e58-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51e58-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
