<span data-ttu-id="35aca-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35aca-p101">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório. |


## <span data-ttu-id="35aca-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35aca-118">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="35aca-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35aca-119">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="35aca-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="35aca-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="35aca-121">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [thumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35aca-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <span data-ttu-id="35aca-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35aca-122">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="35aca-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35aca-123">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="35aca-124">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35aca-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <span data-ttu-id="35aca-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="35aca-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="35aca-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35aca-126">Here is an example of the response.</span></span>
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
