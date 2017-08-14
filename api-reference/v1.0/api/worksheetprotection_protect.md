<span data-ttu-id="24c67-p104">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24c67-p104">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="24c67-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24c67-126">Example</span></span>
<span data-ttu-id="24c67-127">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="24c67-127">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="24c67-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24c67-128">Request</span></span>
<span data-ttu-id="24c67-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="24c67-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetprotection_protect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/protect
Content-type: application/json
Content-length: 383

{
  "options": {
    "allowFormatCells": true,
    "allowFormatColumns": true,
    "allowFormatRows": true,
    "allowInsertColumns": true,
    "allowInsertRows": true,
    "allowInsertHyperlinks": true,
    "allowDeleteColumns": true,
    "allowDeleteRows": true,
    "allowSort": true,
    "allowAutoFilter": true,
    "allowPivotTables": true
  }
}
```

##### <a name="response"></a><span data-ttu-id="24c67-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="24c67-130">Response</span></span>
<span data-ttu-id="24c67-131">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24c67-131">Here is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: protect",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
