<span data-ttu-id="58298-p123">Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="58298-p123">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.          |

## <a name="response"></a><span data-ttu-id="58298-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="58298-261">Response</span></span>

<span data-ttu-id="58298-262">Se bem-sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="58298-262">If successful, this method returns a `204 No Content` response code.</span></span>
## <a name="example"></a><span data-ttu-id="58298-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58298-263">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58298-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58298-264">Request</span></span>
<span data-ttu-id="58298-265">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58298-265">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```
##### <a name="response"></a><span data-ttu-id="58298-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="58298-266">Response</span></span>
<span data-ttu-id="58298-267">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58298-267">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
