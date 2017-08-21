# <a name="list-attachments"></a><span data-ttu-id="83bc1-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="83bc1-101">List attachments</span></span>

<span data-ttu-id="83bc1-102">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma postagem.</span><span class="sxs-lookup"><span data-stu-id="83bc1-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a post.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83bc1-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="83bc1-103">Prerequisites</span></span>
<span data-ttu-id="83bc1-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="83bc1-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="83bc1-105">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="83bc1-105">Group.Read.All</span></span>
* <span data-ttu-id="83bc1-106">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83bc1-106">Group.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="83bc1-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="83bc1-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="83bc1-108">Anexos de uma [post](../resources/post.md) em um [thread](../resources/conversationthread.md) que pertence a uma [conversation](../resources/conversation.md) de um grupo.</span><span class="sxs-lookup"><span data-stu-id="83bc1-108">Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="83bc1-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="83bc1-109">Optional query parameters</span></span>
<span data-ttu-id="83bc1-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="83bc1-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="83bc1-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="83bc1-111">Request headers</span></span>
| <span data-ttu-id="83bc1-112">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="83bc1-112">Header</span></span>       | <span data-ttu-id="83bc1-113">Valor</span><span class="sxs-lookup"><span data-stu-id="83bc1-113">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="83bc1-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="83bc1-114">Authorization</span></span>  | <span data-ttu-id="83bc1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="83bc1-p101">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="83bc1-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="83bc1-117">Request body</span></span>
<span data-ttu-id="83bc1-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="83bc1-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83bc1-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="83bc1-119">Response</span></span>

<span data-ttu-id="83bc1-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="83bc1-120">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="83bc1-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="83bc1-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="83bc1-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="83bc1-122">Request</span></span>
<span data-ttu-id="83bc1-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="83bc1-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="83bc1-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="83bc1-124">Response</span></span>
<span data-ttu-id="83bc1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="83bc1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
