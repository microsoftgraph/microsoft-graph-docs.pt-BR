# <a name="list-attachments"></a><span data-ttu-id="2925f-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="2925f-101">List attachments</span></span>

<span data-ttu-id="2925f-102">Recupera uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="2925f-102">Retrieve a list of attachment objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2925f-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2925f-103">Prerequisites</span></span>
<span data-ttu-id="2925f-104">Os seguintes **escopos** são necessários para executar esta API: _Mail.Read_</span><span class="sxs-lookup"><span data-stu-id="2925f-104">The following **scopes** are required to execute this API: _Mail.Read_</span></span>
## <a name="http-request"></a><span data-ttu-id="2925f-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2925f-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2925f-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2925f-106">Optional query parameters</span></span>
<span data-ttu-id="2925f-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2925f-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2925f-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2925f-108">Request headers</span></span>
| <span data-ttu-id="2925f-109">Nome</span><span class="sxs-lookup"><span data-stu-id="2925f-109">Name</span></span>       | <span data-ttu-id="2925f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2925f-110">Type</span></span> | <span data-ttu-id="2925f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2925f-111">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2925f-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="2925f-112">Authorization</span></span>  | <span data-ttu-id="2925f-113">string</span><span class="sxs-lookup"><span data-stu-id="2925f-113">string</span></span>  | <span data-ttu-id="2925f-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2925f-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2925f-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2925f-116">Request body</span></span>
<span data-ttu-id="2925f-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2925f-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2925f-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="2925f-118">Response</span></span>

<span data-ttu-id="2925f-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2925f-119">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2925f-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2925f-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2925f-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2925f-121">Request</span></span>
<span data-ttu-id="2925f-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2925f-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="2925f-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="2925f-123">Response</span></span>
<span data-ttu-id="2925f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2925f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
