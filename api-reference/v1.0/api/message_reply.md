<span data-ttu-id="b0ee1-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0ee1-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="b0ee1-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0ee1-131">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="b0ee1-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b0ee1-132">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="b0ee1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0ee1-133">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b0ee1-134">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0ee1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <span data-ttu-id="b0ee1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ee1-135">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="b0ee1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0ee1-136">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b0ee1-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0ee1-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
