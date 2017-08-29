# <a name="get-thumbnailset"></a><span data-ttu-id="da09d-101">Obter thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="da09d-101">Get thumbnailSet</span></span>

<span data-ttu-id="da09d-102">Recupere as propriedades e os relacionamentos de um objeto [thumbnailSet](../resources/thumbnailset.md).</span><span class="sxs-lookup"><span data-stu-id="da09d-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="da09d-103">Para saber mais, consulte [Listar miniaturas](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="da09d-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da09d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da09d-104">Prerequisites</span></span>
<span data-ttu-id="da09d-105">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="da09d-105">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="da09d-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="da09d-106">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="da09d-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da09d-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da09d-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da09d-108">Optional query parameters</span></span>
<span data-ttu-id="da09d-109">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da09d-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da09d-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da09d-110">Request headers</span></span>
| <span data-ttu-id="da09d-111">Nome</span><span class="sxs-lookup"><span data-stu-id="da09d-111">Name</span></span>       | <span data-ttu-id="da09d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="da09d-112">Type</span></span> | <span data-ttu-id="da09d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="da09d-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="da09d-114">Autorização</span><span class="sxs-lookup"><span data-stu-id="da09d-114">Authorization</span></span>  | <span data-ttu-id="da09d-115">string</span><span class="sxs-lookup"><span data-stu-id="da09d-115">string</span></span>  | <span data-ttu-id="da09d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da09d-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da09d-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da09d-118">Request body</span></span>
<span data-ttu-id="da09d-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da09d-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da09d-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="da09d-120">Response</span></span>

<span data-ttu-id="da09d-121">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [thumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da09d-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da09d-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da09d-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da09d-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da09d-123">Request</span></span>
<span data-ttu-id="da09d-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da09d-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="da09d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="da09d-125">Response</span></span>
<span data-ttu-id="da09d-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da09d-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
