# <a name="add-attachment"></a><span data-ttu-id="39fe7-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="39fe7-101">Add attachment</span></span>

<span data-ttu-id="39fe7-p101">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="39fe7-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="permissions"></a><span data-ttu-id="39fe7-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="39fe7-104">Permissions</span></span>
<span data-ttu-id="39fe7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="39fe7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39fe7-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39fe7-107">Permission type</span></span>      | <span data-ttu-id="39fe7-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39fe7-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39fe7-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39fe7-109">Delegated (work or school account)</span></span> | <span data-ttu-id="39fe7-110">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39fe7-110">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="39fe7-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39fe7-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39fe7-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39fe7-112">Not supported.</span></span>    |
|<span data-ttu-id="39fe7-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39fe7-113">Application</span></span> | <span data-ttu-id="39fe7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39fe7-114">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39fe7-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39fe7-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="39fe7-116">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="39fe7-116">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="39fe7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39fe7-117">Request headers</span></span>
| <span data-ttu-id="39fe7-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39fe7-118">Header</span></span>       | <span data-ttu-id="39fe7-119">Valor</span><span class="sxs-lookup"><span data-stu-id="39fe7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="39fe7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="39fe7-120">Authorization</span></span>  | <span data-ttu-id="39fe7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39fe7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39fe7-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39fe7-123">Request body</span></span>
<span data-ttu-id="39fe7-124">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="39fe7-124">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="39fe7-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="39fe7-125">Response</span></span>

<span data-ttu-id="39fe7-126">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39fe7-126">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="39fe7-127">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="39fe7-127">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="39fe7-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39fe7-128">Request</span></span>
<span data-ttu-id="39fe7-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39fe7-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "contentBytes-value"
}
```

<span data-ttu-id="39fe7-130">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="39fe7-130">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="39fe7-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="39fe7-131">Response</span></span>
<span data-ttu-id="39fe7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39fe7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="39fe7-135">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="39fe7-135">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="39fe7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39fe7-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="39fe7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="39fe7-137">Response</span></span>
<span data-ttu-id="39fe7-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39fe7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
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
