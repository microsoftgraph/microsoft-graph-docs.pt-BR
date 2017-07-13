<span data-ttu-id="7d56d-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d56d-p101">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório. |
| <span data-ttu-id="7d56d-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7d56d-114">Content-Type</span></span>  | <span data-ttu-id="7d56d-115">application/json</span><span class="sxs-lookup"><span data-stu-id="7d56d-115">application/json</span></span>  |

## <span data-ttu-id="7d56d-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d56d-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="7d56d-117">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="7d56d-117">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <span data-ttu-id="7d56d-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d56d-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7d56d-119">Se bem-sucedido, este método retorna um código de resposta `204, No Content`.</span><span class="sxs-lookup"><span data-stu-id="7d56d-119">If successful, this method returns `204, No Content` response code.</span></span>

## <span data-ttu-id="7d56d-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d56d-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="7d56d-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d56d-121">Request</span></span>
<a id="request" class="xliff"></a>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <span data-ttu-id="7d56d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d56d-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="7d56d-123">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7d56d-123">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->