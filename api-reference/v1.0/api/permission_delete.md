<span data-ttu-id="15381-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15381-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="15381-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="15381-123">Example</span></span>

##### <a name="request"></a><span data-ttu-id="15381-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15381-124">Request</span></span>

<span data-ttu-id="15381-125">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15381-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="15381-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="15381-126">Response</span></span>

<span data-ttu-id="15381-127">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15381-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="15381-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="15381-128">Remarks</span></span>

* <span data-ttu-id="15381-129">[Drives](../resources/drive.md) com **driveType** `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="15381-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
