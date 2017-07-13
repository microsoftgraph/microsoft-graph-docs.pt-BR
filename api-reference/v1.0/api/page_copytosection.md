<span data-ttu-id="41b1e-p104">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="41b1e-p104">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).

## <span data-ttu-id="41b1e-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41b1e-134">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="41b1e-135">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="41b1e-135">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="41b1e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41b1e-136">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="41b1e-137">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41b1e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "page_copytosection"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/copyToSection
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "groupId": "groupId-value"
}
```

##### <span data-ttu-id="41b1e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b1e-138">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="41b1e-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="41b1e-139">Here is an example of the response.</span></span>
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
  "description": "page: copyToSection",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->