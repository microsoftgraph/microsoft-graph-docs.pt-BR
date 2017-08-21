# <a name="add-attachment"></a><span data-ttu-id="c4787-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="c4787-101">Add attachment</span></span>

<span data-ttu-id="c4787-p101">Use esta API para adicionar um [attachment](../resources/attachment.md) a uma postagem. Como atualmente há um limite de 4 MB para o tamanho total de cada solicitação REST, isso limita o tamanho do anexo que você pode adicionar a 4 MB.</span><span class="sxs-lookup"><span data-stu-id="c4787-p101">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c4787-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c4787-104">Prerequisites</span></span>
<span data-ttu-id="c4787-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="c4787-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="c4787-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4787-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c4787-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4787-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c4787-108">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="c4787-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="c4787-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4787-109">Request headers</span></span>
| <span data-ttu-id="c4787-110">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4787-110">Header</span></span>       | <span data-ttu-id="c4787-111">Valor</span><span class="sxs-lookup"><span data-stu-id="c4787-111">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4787-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4787-112">Authorization</span></span>  | <span data-ttu-id="c4787-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4787-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4787-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4787-115">Request body</span></span>
<span data-ttu-id="c4787-116">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c4787-116">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c4787-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4787-117">Response</span></span>

<span data-ttu-id="c4787-118">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4787-118">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="c4787-119">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="c4787-119">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="c4787-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4787-120">Request</span></span>
<span data-ttu-id="c4787-121">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4787-121">Here is an example of the request.</span></span>
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

<span data-ttu-id="c4787-122">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="c4787-122">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c4787-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4787-123">Response</span></span>
<span data-ttu-id="c4787-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4787-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-item-attachment"></a><span data-ttu-id="c4787-127">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="c4787-127">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="c4787-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4787-128">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="c4787-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4787-129">Response</span></span>
<span data-ttu-id="c4787-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4787-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
