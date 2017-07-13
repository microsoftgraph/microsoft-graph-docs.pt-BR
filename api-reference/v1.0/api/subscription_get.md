<span data-ttu-id="52ebd-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52ebd-p101">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório. |

## <span data-ttu-id="52ebd-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52ebd-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="52ebd-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52ebd-117">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="52ebd-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ebd-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="52ebd-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52ebd-119">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="52ebd-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52ebd-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="52ebd-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52ebd-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="52ebd-122">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52ebd-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="52ebd-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="52ebd-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="52ebd-124">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52ebd-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
