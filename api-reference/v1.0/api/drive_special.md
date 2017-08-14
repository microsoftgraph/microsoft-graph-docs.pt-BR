<span data-ttu-id="a21ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a21ae-p103">Bearer {token}. Required.</span></span> | {token} de portador. Obrigatório. |


## <a name="request-body"></a><span data-ttu-id="a21ae-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ae-128">Request body</span></span>
<span data-ttu-id="a21ae-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a21ae-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a21ae-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ae-130">Response</span></span>

<span data-ttu-id="a21ae-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [driveItem](../resources/driveitem.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-131">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a21ae-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a21ae-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a21ae-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a21ae-133">Request</span></span>
<span data-ttu-id="a21ae-134">Eis um exemplo da solicitação de unidades do usuário.</span><span class="sxs-lookup"><span data-stu-id="a21ae-134">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="a21ae-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a21ae-135">Response</span></span>
<span data-ttu-id="a21ae-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a21ae-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="a21ae-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="a21ae-137">Remarks</span></span>

<span data-ttu-id="a21ae-138">Para solicitar os filhos de uma pasta especial, você pode solicitar a coleção `children` ou usar a opção [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para expandir a coleção de filhos.</span><span class="sxs-lookup"><span data-stu-id="a21ae-138">To request the children of a special folder, you can request the `children` collection or use the [expand](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
