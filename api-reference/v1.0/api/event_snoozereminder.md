<span data-ttu-id="e7278-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7278-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="e7278-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7278-129">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="e7278-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e7278-130">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="e7278-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7278-131">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e7278-132">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7278-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <span data-ttu-id="e7278-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7278-133">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e7278-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7278-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
