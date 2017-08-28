# <a name="list-attachments"></a><span data-ttu-id="fdb71-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="fdb71-101">List attachments</span></span>

<span data-ttu-id="fdb71-102">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="fdb71-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="permissions"></a><span data-ttu-id="fdb71-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdb71-103">Permissions</span></span>
<span data-ttu-id="fdb71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdb71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fdb71-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdb71-106">Permission type</span></span>      | <span data-ttu-id="fdb71-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdb71-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="fdb71-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdb71-108">Delegated (work or school account)</span></span> | <span data-ttu-id="fdb71-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb71-109">Group.Read.All, Group.Readwrite.All</span></span>    | 
|<span data-ttu-id="fdb71-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdb71-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fdb71-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdb71-111">Not supported.</span></span>    | 
|<span data-ttu-id="fdb71-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdb71-112">Application</span></span> | <span data-ttu-id="fdb71-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdb71-113">Group.Read.All, Group.Readwrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fdb71-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdb71-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="fdb71-115">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="fdb71-115">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fdb71-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fdb71-116">Optional query parameters</span></span>
<span data-ttu-id="fdb71-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb71-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fdb71-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb71-118">Request headers</span></span>
| <span data-ttu-id="fdb71-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdb71-119">Header</span></span>       | <span data-ttu-id="fdb71-120">Valor</span><span class="sxs-lookup"><span data-stu-id="fdb71-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fdb71-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdb71-121">Authorization</span></span>  | <span data-ttu-id="fdb71-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdb71-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fdb71-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb71-124">Request body</span></span>
<span data-ttu-id="fdb71-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdb71-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdb71-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb71-126">Response</span></span>

<span data-ttu-id="fdb71-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdb71-127">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fdb71-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdb71-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fdb71-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdb71-129">Request</span></span>
<span data-ttu-id="fdb71-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdb71-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="fdb71-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdb71-131">Response</span></span>
<span data-ttu-id="fdb71-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdb71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "id": "id-value",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "isInline": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
