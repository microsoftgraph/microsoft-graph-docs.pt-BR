<span data-ttu-id="d82c9-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82c9-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="d82c9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d82c9-130">Example</span></span>
<span data-ttu-id="d82c9-131">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d82c9-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d82c9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d82c9-132">Request</span></span>
<span data-ttu-id="d82c9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d82c9-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_setdata"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/setData
Content-type: application/json
Content-length: 70

{
  "sourceData": "sourceData-value",
  "seriesBy": "seriesBy-value"
}
```

##### <a name="response"></a><span data-ttu-id="d82c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d82c9-134">Response</span></span>
<span data-ttu-id="d82c9-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d82c9-135">Here is an example of the response.</span></span> 
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
  "description": "Chart: setData",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->