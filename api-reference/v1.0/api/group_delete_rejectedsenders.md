<span data-ttu-id="916de-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916de-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="916de-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="916de-117">Example</span></span>
##### <a name="request"></a><span data-ttu-id="916de-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="916de-118">Request</span></span>
<span data-ttu-id="916de-119">Eis alguns exemplos da solicitação.</span><span class="sxs-lookup"><span data-stu-id="916de-119">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id="groups/{id}"
```

##### <a name="response"></a><span data-ttu-id="916de-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="916de-120">Response</span></span>
<span data-ttu-id="916de-121">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="916de-121">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->