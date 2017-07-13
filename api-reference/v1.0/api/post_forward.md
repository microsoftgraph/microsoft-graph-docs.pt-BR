<span data-ttu-id="30476-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30476-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="30476-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30476-128">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="30476-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="30476-129">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="30476-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30476-130">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="30476-131">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30476-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <span data-ttu-id="30476-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="30476-132">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="30476-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30476-133">Here is an example of the response.</span></span>
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
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
