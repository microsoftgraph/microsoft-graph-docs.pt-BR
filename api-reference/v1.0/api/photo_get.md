# <a name="get-photo"></a><span data-ttu-id="9c21c-101">Obter foto</span><span class="sxs-lookup"><span data-stu-id="9c21c-101">Get photo</span></span>

<span data-ttu-id="9c21c-102">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="9c21c-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c21c-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c21c-103">Prerequisites</span></span>
<span data-ttu-id="9c21c-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="9c21c-104">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="9c21c-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="9c21c-105">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="9c21c-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c21c-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c21c-107">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9c21c-107">Optional query parameters</span></span>
<span data-ttu-id="9c21c-108">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9c21c-108">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c21c-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c21c-109">Request headers</span></span>
| <span data-ttu-id="9c21c-110">Nome</span><span class="sxs-lookup"><span data-stu-id="9c21c-110">Name</span></span>       | <span data-ttu-id="9c21c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c21c-111">Type</span></span> | <span data-ttu-id="9c21c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c21c-112">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c21c-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c21c-113">Authorization</span></span>  | <span data-ttu-id="9c21c-114">string</span><span class="sxs-lookup"><span data-stu-id="9c21c-114">string</span></span>  | <span data-ttu-id="9c21c-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c21c-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c21c-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c21c-117">Request body</span></span>
<span data-ttu-id="9c21c-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c21c-118">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c21c-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c21c-119">Response</span></span>

<span data-ttu-id="9c21c-120">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c21c-120">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c21c-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c21c-121">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c21c-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c21c-122">Request</span></span>
<span data-ttu-id="9c21c-123">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c21c-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="9c21c-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c21c-124">Response</span></span>
<span data-ttu-id="9c21c-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c21c-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
