<span data-ttu-id="1da26-p103">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1da26-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="1da26-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1da26-119">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1da26-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1da26-120">Request</span></span>
<span data-ttu-id="1da26-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1da26-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <a name="response"></a><span data-ttu-id="1da26-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="1da26-122">Response</span></span>
<span data-ttu-id="1da26-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1da26-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="1da26-124">Veja também</span><span class="sxs-lookup"><span data-stu-id="1da26-124">See also</span></span>

- [<span data-ttu-id="1da26-125">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="1da26-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="1da26-126">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="1da26-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->