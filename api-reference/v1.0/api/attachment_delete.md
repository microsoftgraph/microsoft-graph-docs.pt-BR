<span data-ttu-id="75899-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75899-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="75899-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75899-130">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="75899-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75899-131">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="75899-132">Veja um exemplo da solicitação para excluir um anexo em um evento.</span><span class="sxs-lookup"><span data-stu-id="75899-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <span data-ttu-id="75899-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="75899-133">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="75899-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75899-134">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
