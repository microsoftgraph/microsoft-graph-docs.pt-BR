<span data-ttu-id="c7c2e-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.

## <a name="example"></a><span data-ttu-id="c7c2e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7c2e-129">Example</span></span>
<span data-ttu-id="c7c2e-130">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c7c2e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7c2e-131">Request</span></span>
<span data-ttu-id="c7c2e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-132">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c7c2e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7c2e-133">Response</span></span>
<span data-ttu-id="c7c2e-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7c2e-134">Here is an example of the response.</span></span>
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
