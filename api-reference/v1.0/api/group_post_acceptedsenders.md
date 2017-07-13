<span data-ttu-id="0d56c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d56c-p102">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório.  |

## <span data-ttu-id="0d56c-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d56c-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="0d56c-116">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="0d56c-116">In the request body, supply the id of a user or group object.</span></span>


## <span data-ttu-id="0d56c-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d56c-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0d56c-118">Este método retorna o código de resposta `204, No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d56c-118">This method returns `204, No Content` response code and no response body.</span></span>

## <span data-ttu-id="0d56c-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d56c-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="0d56c-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d56c-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="0d56c-121">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d56c-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <span data-ttu-id="0d56c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d56c-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0d56c-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d56c-123">Here is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
