<span data-ttu-id="e28f1-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e28f1-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="e28f1-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e28f1-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e28f1-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e28f1-120">Request</span></span>
<span data-ttu-id="e28f1-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e28f1-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="e28f1-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="e28f1-122">Response</span></span>
<span data-ttu-id="e28f1-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e28f1-123">Here is an example of the response.</span></span> 
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