<span data-ttu-id="1daff-p105">Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).</span><span class="sxs-lookup"><span data-stu-id="1daff-p105">If successful, this method returns a `202 Accepted` response code and an `Operation-Location` header. Poll the Operation-Location endpoint to [get the status of the copy operation](onenoteoperation_get.md).</span></span>
Se bem-sucedido, esse método retornará um código de resposta `202 Accepted` e um cabeçalho `Operation-Location`. Sonde o ponto de extremidade Operation-Location para [obter o status da operação de cópia](onenoteoperation_get.md).

## <span data-ttu-id="1daff-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1daff-138">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="1daff-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="1daff-139">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="1daff-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1daff-140">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="1daff-141">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1daff-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "section_copytonotebook"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/copyToNotebook
Content-type: application/json
Content-length: 84

{
  "id": "id-value",
  "groupId": "groupId-value",
  "renameAs": "renameAs-value"
}
```

##### <span data-ttu-id="1daff-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="1daff-142">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="1daff-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1daff-143">Here is an example of the response.</span></span>
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
  "description": "section: copyToNotebook",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->