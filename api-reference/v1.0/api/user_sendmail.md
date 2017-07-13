<span data-ttu-id="760ae-p105">Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="760ae-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `202, Accepted`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="760ae-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="760ae-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="760ae-134">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="760ae-134">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="760ae-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="760ae-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="760ae-136">Veja a seguir um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="760ae-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/sendMail
Content-type: application/json
Content-length: 512

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    "ccRecipients": [
      {
        "emailAddress": {
          "address": "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  "saveToSentItems": "false"
}
```

##### <span data-ttu-id="760ae-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="760ae-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="760ae-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="760ae-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: sendMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
