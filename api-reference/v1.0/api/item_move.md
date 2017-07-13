<span data-ttu-id="ff25e-p103">**Observação:** Ao mover itens para a raiz de um OneDrive, não é possível usar a sintaxe `"id:" "root"`. É preciso usar a ID real da pasta raiz ou usar `{"path": "/drive/root"}` para a referência do pai.</span><span class="sxs-lookup"><span data-stu-id="ff25e-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

**Observação:** Ao mover itens para a raiz de um OneDrive, não é possível usar a sintaxe `"id:" "root"`. É preciso usar a ID real da pasta raiz ou usar `{"path": "/drive/root"}` para a referência do pai.

## <span data-ttu-id="ff25e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff25e-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ff25e-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e o recurso [DriveItem](../resources/driveitem.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff25e-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="ff25e-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff25e-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="ff25e-128">Este exemplo move um item especificado por {item-id} para a pasta **Documentos** no OneDrive do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff25e-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

## <span data-ttu-id="ff25e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff25e-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ff25e-130">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff25e-130">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
