<span data-ttu-id="bdfdc-p103">Se bem sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdfdc-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="bdfdc-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdfdc-119">Example</span></span>
<span data-ttu-id="bdfdc-120">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="bdfdc-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="bdfdc-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdfdc-121">Request</span></span>
<span data-ttu-id="bdfdc-122">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdfdc-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <a name="response"></a><span data-ttu-id="bdfdc-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdfdc-123">Response</span></span>
<span data-ttu-id="bdfdc-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdfdc-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
