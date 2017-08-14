<span data-ttu-id="20a5f-p101">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="20a5f-p101">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| <span data-ttu-id="20a5f-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20a5f-120">Property</span></span>     | <span data-ttu-id="20a5f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="20a5f-121">Type</span></span>   | <span data-ttu-id="20a5f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="20a5f-122">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="20a5f-123">**roles**</span><span class="sxs-lookup"><span data-stu-id="20a5f-123">**roles**</span></span>    | <span data-ttu-id="20a5f-124">String</span><span class="sxs-lookup"><span data-stu-id="20a5f-124">String</span></span> | <span data-ttu-id="20a5f-125">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="20a5f-125">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="20a5f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="20a5f-126">Response</span></span>

<span data-ttu-id="20a5f-127">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20a5f-127">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20a5f-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20a5f-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="20a5f-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20a5f-129">Request</span></span>

<span data-ttu-id="20a5f-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20a5f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="20a5f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="20a5f-131">Response</span></span>

<span data-ttu-id="20a5f-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20a5f-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
