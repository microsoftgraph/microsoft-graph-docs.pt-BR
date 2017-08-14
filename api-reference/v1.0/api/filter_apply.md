<span data-ttu-id="79b6c-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79b6c-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="79b6c-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79b6c-124">Example</span></span>
<span data-ttu-id="79b6c-125">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="79b6c-125">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="79b6c-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79b6c-126">Request</span></span>
<span data-ttu-id="79b6c-127">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79b6c-127">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="79b6c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="79b6c-128">Response</span></span>
<span data-ttu-id="79b6c-129">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79b6c-129">Here is an example of the response.</span></span> 
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
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->