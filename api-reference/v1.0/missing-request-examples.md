# <a name="helpers-examples-that-arent-included-in-the-docs"></a><span data-ttu-id="8c311-101">Auxiliares (exemplos que não estão incluídos nos documentos)</span><span class="sxs-lookup"><span data-stu-id="8c311-101">Helpers (examples that aren't included in the docs)</span></span>

<span data-ttu-id="8c311-102">Estas são as coisas que tive que adicionar aos documentos para garantir que a ferramenta Markdown-Scanner conseguiria lidar adequadamente com os documentos do Graph.</span><span class="sxs-lookup"><span data-stu-id="8c311-102">These are things I had to add in the docs to make sure the Markdown-Scanner tool was able to properly handle the Graph docs.</span></span>


## <a name="define-the-me-as-singleton"></a><span data-ttu-id="8c311-103">Definir /me como singleton</span><span class="sxs-lookup"><span data-stu-id="8c311-103">Define the /me as singleton</span></span>

<!-- {"blockType": "request", "name": "get_current_user" } -->
```http
GET https://graph.microsoft.com/v1.0/me
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-drives-as-an-queryable-entityset"></a><span data-ttu-id="8c311-104">Defina as unidades como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="8c311-104">Define drives as an queryable entityset</span></span>
<!-- {"blockType": "request", "name": "get_drive_from_id" } -->
```http
GET https://graph.microsoft.com/v1.0/drives/{drive-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.drive", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


## <a name="define-users-as-an-queryable-entityset"></a><span data-ttu-id="8c311-105">Defina os usuários como um conjunto de entidades consultável</span><span class="sxs-lookup"><span data-stu-id="8c311-105">define users as an queryable entityset</span></span>

<!-- {"blockType": "request", "name": "get_users" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{user-id}
```

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.user", truncated: true } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
