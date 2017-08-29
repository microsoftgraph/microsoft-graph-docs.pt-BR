# <a name="add-attachment"></a><span data-ttu-id="874ff-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="874ff-101">Add attachment</span></span>

<span data-ttu-id="874ff-102">Use esta API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="874ff-102">Use this API to create a new Attachment.</span></span>
## <a name="permissions"></a><span data-ttu-id="874ff-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="874ff-103">Permissions</span></span>
<span data-ttu-id="874ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="874ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="874ff-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="874ff-106">Permission type</span></span>      | <span data-ttu-id="874ff-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="874ff-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="874ff-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="874ff-108">Delegated (work or school account)</span></span> | <span data-ttu-id="874ff-109">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874ff-109">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="874ff-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="874ff-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="874ff-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874ff-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="874ff-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="874ff-112">Application</span></span> | <span data-ttu-id="874ff-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="874ff-113">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="874ff-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="874ff-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="874ff-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="874ff-115">Request headers</span></span>
| <span data-ttu-id="874ff-116">Nome</span><span class="sxs-lookup"><span data-stu-id="874ff-116">Name</span></span>       | <span data-ttu-id="874ff-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="874ff-117">Type</span></span> | <span data-ttu-id="874ff-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="874ff-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="874ff-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="874ff-119">Authorization</span></span>  | <span data-ttu-id="874ff-120">string</span><span class="sxs-lookup"><span data-stu-id="874ff-120">string</span></span>  | <span data-ttu-id="874ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874ff-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="874ff-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="874ff-123">Content-Type</span></span> | <span data-ttu-id="874ff-124">string</span><span class="sxs-lookup"><span data-stu-id="874ff-124">string</span></span>  | <span data-ttu-id="874ff-p103">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="874ff-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="874ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="874ff-127">Request body</span></span>
<span data-ttu-id="874ff-128">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="874ff-128">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="874ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ff-129">Response</span></span>

<span data-ttu-id="874ff-130">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="874ff-130">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="874ff-131">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="874ff-131">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="874ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874ff-132">Request</span></span>
<span data-ttu-id="874ff-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="874ff-133">Here is an example of the request.</span></span>
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

<span data-ttu-id="874ff-134">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="874ff-134">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="874ff-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ff-135">Response</span></span>
<span data-ttu-id="874ff-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="874ff-139">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="874ff-139">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="874ff-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="874ff-140">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="874ff-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="874ff-141">Response</span></span>
<span data-ttu-id="874ff-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="874ff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
