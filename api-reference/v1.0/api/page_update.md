<span data-ttu-id="90bad-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.</span><span class="sxs-lookup"><span data-stu-id="90bad-p103">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
Se bem-sucedido, este método retorna um código de resposta `204 No Content`.  Nenhum dado JSON é retornado para uma solicitação PATCH.
## <span data-ttu-id="90bad-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90bad-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="90bad-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90bad-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="90bad-125">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90bad-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
##### <span data-ttu-id="90bad-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="90bad-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="90bad-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90bad-127">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
