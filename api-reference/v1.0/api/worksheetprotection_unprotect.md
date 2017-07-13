<span data-ttu-id="b88c1-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b88c1-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="b88c1-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b88c1-125">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="b88c1-126">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="b88c1-126">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="b88c1-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b88c1-127">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b88c1-128">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b88c1-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
Content-type: application/json
Content-length: 34

{
  "password": "password-value"
}
```

##### <span data-ttu-id="b88c1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b88c1-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b88c1-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b88c1-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->