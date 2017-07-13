<span data-ttu-id="28dee-p104">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28dee-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="28dee-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28dee-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="28dee-128">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="28dee-128">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="28dee-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28dee-129">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="28dee-130">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28dee-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <span data-ttu-id="28dee-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="28dee-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="28dee-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28dee-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
