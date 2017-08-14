<span data-ttu-id="786b2-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="786b2-p101">Bearer {token}. Required.</span></span>  | {token} de portador. Obrigatório. |


## <a name="request-body"></a><span data-ttu-id="786b2-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="786b2-118">Request body</span></span>
<span data-ttu-id="786b2-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="786b2-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="786b2-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="786b2-120">Response</span></span>

<span data-ttu-id="786b2-121">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [thumbnailSet](../resources/thumbnailset.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786b2-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="786b2-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="786b2-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="786b2-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="786b2-123">Request</span></span>
<span data-ttu-id="786b2-124">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="786b2-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="786b2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="786b2-125">Response</span></span>
<span data-ttu-id="786b2-126">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="786b2-126">Here is an example of the response.</span></span>
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
