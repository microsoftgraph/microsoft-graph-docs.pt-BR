<span data-ttu-id="2f710-p102">No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.</span><span class="sxs-lookup"><span data-stu-id="2f710-p102">In the request body, supply the values for relevant fields to be updated. Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance, only include changed values.</span></span>

No corpo da solicitação, forneça os valores para os campos relevantes que serão atualizados. As propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter melhor desempenho, somente inclua valores alterados.

## <a name="response"></a><span data-ttu-id="2f710-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f710-120">Response</span></span>

<span data-ttu-id="2f710-121">Se bem-sucedido, este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2f710-121">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f710-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f710-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f710-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f710-123">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/V1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="2f710-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f710-124">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->