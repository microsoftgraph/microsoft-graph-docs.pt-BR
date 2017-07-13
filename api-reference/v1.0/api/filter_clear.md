<span data-ttu-id="a59b3-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59b3-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="a59b3-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a59b3-117">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="a59b3-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a59b3-118">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="a59b3-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a59b3-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="a59b3-120">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a59b3-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <span data-ttu-id="a59b3-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="a59b3-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a59b3-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a59b3-122">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->