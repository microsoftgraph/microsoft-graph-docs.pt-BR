<span data-ttu-id="63b73-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63b73-p102">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório.  |
| <span data-ttu-id="63b73-115">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63b73-115">Content-Type</span></span>   | <span data-ttu-id="63b73-116">application/json</span><span class="sxs-lookup"><span data-stu-id="63b73-116">application/json</span></span>  | 

## <span data-ttu-id="63b73-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63b73-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="63b73-118">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63b73-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="63b73-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="63b73-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="63b73-120">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63b73-120">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <span data-ttu-id="63b73-121">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63b73-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="63b73-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63b73-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="63b73-123">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63b73-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <span data-ttu-id="63b73-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="63b73-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="63b73-125">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63b73-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
