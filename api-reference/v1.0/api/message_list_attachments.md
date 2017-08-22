# <a name="list-attachments"></a><span data-ttu-id="9c5eb-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="9c5eb-101">List attachments</span></span>

<span data-ttu-id="9c5eb-102">Recupere uma lista de objetos [attachment](../resources/attachment.md) anexados a uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-102">Retrieve a list of [attachment](../resources/attachment.md) objects attached to a message.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c5eb-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c5eb-103">Prerequisites</span></span>
<span data-ttu-id="9c5eb-104">Um dos seguintes **escopos** é necessário para executar esta API: *Mail.Read*</span><span class="sxs-lookup"><span data-stu-id="9c5eb-104">One of the following **scopes** is required to execute this API: *Mail.Read*</span></span> 
## <a name="http-request"></a><span data-ttu-id="9c5eb-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c5eb-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="9c5eb-106">Anexos de uma [message](../resources/message.md) em uma caixa de correio de usuário.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-106">Attachments for a [message](../resources/message.md) in a user's mailbox.</span></span>
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
<span data-ttu-id="9c5eb-107">Anexos de uma [message](../resources/message.md) contidos em uma [mailFolder](../resources/mailfolder.md) de nível superior na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-107">Attachments for a [message](../resources/message.md) contained in a top level [mailFolder](../resources/mailfolder.md) in a user's mailbox.</span></span>
```http
GET /me/mailFolders/{id}/messages/{id}/attachments
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments
```
<span data-ttu-id="9c5eb-p101">Anexos de uma [message](../resources/message.md) contidos em uma pasta filha de uma [mailFolder](../resources/mailfolder.md) na caixa de correio de um usuário.  O exemplo a seguir mostra um nível de aninhamento, mas uma mensagem pode estar localizada em um filho de um filho, e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-p101">Attachments for a [message](../resources/message.md) contained in a child folder of a [mailFolder](../resources/mailfolder.md) in a user's mailbox.  The example below shows one level of nesting, but a message can be located in a child of a child and so on.</span></span>
```http
GET /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c5eb-110">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c5eb-110">Optional query parameters</span></span>
<span data-ttu-id="9c5eb-111">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-111">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9c5eb-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c5eb-112">Request headers</span></span>
| <span data-ttu-id="9c5eb-113">Nome</span><span class="sxs-lookup"><span data-stu-id="9c5eb-113">Name</span></span>       | <span data-ttu-id="9c5eb-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c5eb-114">Type</span></span> | <span data-ttu-id="9c5eb-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c5eb-115">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c5eb-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c5eb-116">Authorization</span></span>  | <span data-ttu-id="9c5eb-117">string</span><span class="sxs-lookup"><span data-stu-id="9c5eb-117">string</span></span>  | <span data-ttu-id="9c5eb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c5eb-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c5eb-120">Request body</span></span>
<span data-ttu-id="9c5eb-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c5eb-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c5eb-122">Response</span></span>

<span data-ttu-id="9c5eb-123">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-123">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c5eb-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c5eb-124">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c5eb-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c5eb-125">Request</span></span>
<span data-ttu-id="9c5eb-126">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-126">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="9c5eb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c5eb-127">Response</span></span>
<span data-ttu-id="9c5eb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c5eb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "datetime-value",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
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