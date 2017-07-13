<span data-ttu-id="2b306-p106">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b306-p106">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="2b306-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2b306-142">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="2b306-143">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2b306-143">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="2b306-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2b306-144">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="2b306-145">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2b306-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangesort_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/sort/apply
Content-type: application/json
Content-length: 358

{
  "fields": [
    {
      "key": 99,
      "sortOn": "sortOn-value",
      "ascending": true,
      "color": "color-value",
      "dataOption": "dataOption-value",
      "icon": {
        "set": "set-value",
        "index": 99
      }
    }
  ],
  "matchCase": true,
  "hasHeaders": true,
  "orientation": "orientation-value",
  "method": "method-value"
}
```

##### <span data-ttu-id="2b306-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2b306-146">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="2b306-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2b306-147">Here is an example of the response.</span></span> 
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
  "description": "RangeSort: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->