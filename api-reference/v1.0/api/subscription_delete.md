<span data-ttu-id="0169a-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0169a-p101">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório. |

## <span data-ttu-id="0169a-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0169a-114">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="0169a-115">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0169a-115">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="0169a-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="0169a-116">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0169a-117">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0169a-117">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="0169a-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0169a-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="0169a-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0169a-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="0169a-120">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0169a-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="0169a-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="0169a-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="0169a-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0169a-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
