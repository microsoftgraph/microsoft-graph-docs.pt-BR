<span data-ttu-id="28c69-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28c69-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="28c69-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28c69-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="28c69-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28c69-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="28c69-121">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28c69-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <span data-ttu-id="28c69-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c69-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="28c69-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28c69-123">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->