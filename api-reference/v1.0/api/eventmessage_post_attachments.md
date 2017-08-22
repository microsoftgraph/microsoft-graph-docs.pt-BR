# <a name="add-attachment"></a><span data-ttu-id="9e048-101">Adicionar anexo</span><span class="sxs-lookup"><span data-stu-id="9e048-101">Add attachment</span></span>

<span data-ttu-id="9e048-102">Use essa API para criar um novo Anexo.</span><span class="sxs-lookup"><span data-stu-id="9e048-102">Use this API to create a new Attachment.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e048-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9e048-103">Prerequisites</span></span>
<span data-ttu-id="9e048-104">Os seguintes **escopos** são necessários para executar esta API:  _Mail.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="9e048-104">The following **scopes** are required to execute this API: _Mail.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="9e048-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e048-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="9e048-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e048-106">Request headers</span></span>
| <span data-ttu-id="9e048-107">Nome</span><span class="sxs-lookup"><span data-stu-id="9e048-107">Name</span></span>       | <span data-ttu-id="9e048-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e048-108">Type</span></span> | <span data-ttu-id="9e048-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e048-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9e048-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e048-110">Authorization</span></span>  | <span data-ttu-id="9e048-111">string</span><span class="sxs-lookup"><span data-stu-id="9e048-111">string</span></span>  | <span data-ttu-id="9e048-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e048-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9e048-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9e048-114">Content-Type</span></span> | <span data-ttu-id="9e048-115">string</span><span class="sxs-lookup"><span data-stu-id="9e048-115">string</span></span>  | <span data-ttu-id="9e048-p102">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e048-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e048-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e048-118">Request body</span></span>
<span data-ttu-id="9e048-119">No corpo da solicitação, forneça uma representação JSON do objeto [Attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9e048-119">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e048-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e048-120">Response</span></span>

<span data-ttu-id="9e048-121">Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e048-121">If successful, this method returns `201, Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="9e048-122">Exemplo (anexo de arquivo)</span><span class="sxs-lookup"><span data-stu-id="9e048-122">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="9e048-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e048-123">Request</span></span>
<span data-ttu-id="9e048-124">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e048-124">Here is an example of the request.</span></span>
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

<span data-ttu-id="9e048-125">No corpo da solicitação, forneça uma representação JSON do objeto [attachment](../resources/attachment.md).</span><span class="sxs-lookup"><span data-stu-id="9e048-125">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9e048-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e048-126">Response</span></span>
<span data-ttu-id="9e048-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e048-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="9e048-130">Exemplo (anexo de item)</span><span class="sxs-lookup"><span data-stu-id="9e048-130">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="9e048-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e048-131">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="9e048-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e048-132">Response</span></span>
<span data-ttu-id="9e048-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e048-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
