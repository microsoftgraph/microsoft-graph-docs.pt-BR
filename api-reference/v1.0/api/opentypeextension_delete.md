<span data-ttu-id="ae536-p105">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae536-p105">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <span data-ttu-id="ae536-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ae536-156">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="ae536-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ae536-157">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="ae536-158">O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="ae536-158">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="ae536-159">O segundo exemplo exclui uma extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="ae536-159">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <span data-ttu-id="ae536-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ae536-160">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="ae536-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ae536-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->