<span data-ttu-id="59b98-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59b98-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="59b98-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59b98-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="59b98-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59b98-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="59b98-120">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59b98-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <span data-ttu-id="59b98-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="59b98-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="59b98-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59b98-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->