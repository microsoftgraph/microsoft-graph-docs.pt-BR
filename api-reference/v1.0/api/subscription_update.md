<span data-ttu-id="b735d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b735d-p102">Bearer token. Required.</span></span>  | {token} de portador. Obrigatório. |

## <span data-ttu-id="b735d-117">Resposta</span><span class="sxs-lookup"><span data-stu-id="b735d-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b735d-118">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [subscription](../resources/subscription.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b735d-118">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="b735d-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b735d-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="b735d-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b735d-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="b735d-121">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b735d-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <span data-ttu-id="b735d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="b735d-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="b735d-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b735d-123">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
