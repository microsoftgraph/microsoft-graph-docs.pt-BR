<span data-ttu-id="4bb0f-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb0f-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="4bb0f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4bb0f-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4bb0f-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4bb0f-120">Request</span></span>
<span data-ttu-id="4bb0f-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4bb0f-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="4bb0f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="4bb0f-122">Response</span></span>
<span data-ttu-id="4bb0f-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4bb0f-123">Here is an example of the response.</span></span> 
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
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->