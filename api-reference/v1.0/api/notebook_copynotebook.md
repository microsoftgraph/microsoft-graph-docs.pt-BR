<span data-ttu-id="d052a-p106">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteOperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="d052a-p106">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteOperation_get.md).</span></span>
Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteOperation_get.md).

## <span data-ttu-id="d052a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d052a-136">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="d052a-137">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d052a-137">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="d052a-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d052a-138">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="d052a-139">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d052a-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "notebook_copynotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/{id}/copyNotebook
Content-type: application/json
Content-length: 108

{
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="d052a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d052a-140">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="d052a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d052a-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook: copyNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
