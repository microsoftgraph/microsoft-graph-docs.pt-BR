# <a name="list-attachments"></a><span data-ttu-id="6b62d-101">Listar anexos</span><span class="sxs-lookup"><span data-stu-id="6b62d-101">List attachments</span></span>

<span data-ttu-id="6b62d-102">Recuperar uma lista de objetos de anexo.</span><span class="sxs-lookup"><span data-stu-id="6b62d-102">Retrieve a list of attachment objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b62d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b62d-103">Permissions</span></span>
<span data-ttu-id="6b62d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b62d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b62d-106">Permission type</span></span>      | <span data-ttu-id="6b62d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b62d-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="6b62d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b62d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6b62d-109">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b62d-109">Mail.Read</span></span>    | 
|<span data-ttu-id="6b62d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b62d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b62d-111">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b62d-111">Mail.Read</span></span>    | 
|<span data-ttu-id="6b62d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b62d-112">Application</span></span> | <span data-ttu-id="6b62d-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="6b62d-113">Mail.Read</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6b62d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b62d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}/attachments
GET /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6b62d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b62d-115">Optional query parameters</span></span>
<span data-ttu-id="6b62d-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b62d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b62d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b62d-117">Request headers</span></span>
| <span data-ttu-id="6b62d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6b62d-118">Name</span></span>       | <span data-ttu-id="6b62d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b62d-119">Type</span></span> | <span data-ttu-id="6b62d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b62d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6b62d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b62d-121">Authorization</span></span>  | <span data-ttu-id="6b62d-122">string</span><span class="sxs-lookup"><span data-stu-id="6b62d-122">string</span></span>  | <span data-ttu-id="6b62d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b62d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b62d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b62d-125">Request body</span></span>
<span data-ttu-id="6b62d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b62d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b62d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b62d-127">Response</span></span>

<span data-ttu-id="6b62d-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Attachment](../resources/attachment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b62d-128">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6b62d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b62d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b62d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b62d-130">Request</span></span>
<span data-ttu-id="6b62d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b62d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="6b62d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b62d-132">Response</span></span>
<span data-ttu-id="6b62d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b62d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
