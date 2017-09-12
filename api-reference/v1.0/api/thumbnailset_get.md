# <a name="get-thumbnailset"></a><span data-ttu-id="46614-101">Obter thumbnailSet</span><span class="sxs-lookup"><span data-stu-id="46614-101">Get thumbnailSet</span></span>

<span data-ttu-id="46614-102">Recupere as propriedades e os relacionamentos de um objeto [thumbnailSet](../resources/thumbnailset.md).</span><span class="sxs-lookup"><span data-stu-id="46614-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="46614-103">Para saber mais, confira [Listar miniaturas](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="46614-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="46614-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="46614-104">Permissions</span></span>
<span data-ttu-id="46614-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="46614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="46614-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46614-107">Permission type</span></span>      | <span data-ttu-id="46614-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46614-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="46614-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46614-109">Delegated (work or school account)</span></span> | <span data-ttu-id="46614-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="46614-110">Files.Read</span></span>    | 
|<span data-ttu-id="46614-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46614-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46614-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="46614-112">Files.Read</span></span>    | 
|<span data-ttu-id="46614-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46614-113">Application</span></span> | <span data-ttu-id="46614-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46614-114">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="46614-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46614-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="46614-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46614-116">Optional query parameters</span></span>
<span data-ttu-id="46614-117">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46614-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46614-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46614-118">Request headers</span></span>
| <span data-ttu-id="46614-119">Nome</span><span class="sxs-lookup"><span data-stu-id="46614-119">Name</span></span>       | <span data-ttu-id="46614-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="46614-120">Type</span></span> | <span data-ttu-id="46614-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="46614-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="46614-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46614-122">Authorization</span></span>  | <span data-ttu-id="46614-123">string</span><span class="sxs-lookup"><span data-stu-id="46614-123">string</span></span>  | <span data-ttu-id="46614-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46614-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="46614-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46614-126">Request body</span></span>
<span data-ttu-id="46614-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46614-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46614-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46614-128">Response</span></span>

<span data-ttu-id="46614-129">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [thumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46614-129">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46614-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46614-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46614-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46614-131">Request</span></span>
<span data-ttu-id="46614-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46614-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="46614-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46614-133">Response</span></span>
<span data-ttu-id="46614-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46614-134">Here is an example of the response.</span></span>
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
