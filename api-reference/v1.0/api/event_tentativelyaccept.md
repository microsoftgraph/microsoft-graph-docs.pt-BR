<span data-ttu-id="80829-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80829-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="80829-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80829-135">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="80829-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="80829-136">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="80829-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80829-137">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="80829-138">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80829-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_tentativelyaccept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/tentativelyAccept
Content-type: application/json
Content-length: 56

{
  "comment": "comment-value",
  "sendResponse": true
}
```

##### <span data-ttu-id="80829-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="80829-139">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="80829-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="80829-140">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="80829-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80829-141">Here is an example of the response.</span></span>
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
  "description": "event: tentativelyAccept",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
