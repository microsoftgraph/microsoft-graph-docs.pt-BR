<span data-ttu-id="2d408-p102">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="2d408-p102">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> | O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores. |

## <a name="response"></a><span data-ttu-id="2d408-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d408-126">Response</span></span>

<span data-ttu-id="2d408-127">Se for bem-sucedido, esse método retornará um código de resposta `204 OK` e um objeto [groupSetting](../resources/groupsetting.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2d408-127">If successful, this method returns a `204 OK` response code and [directoryObject](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d408-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2d408-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d408-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2d408-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="2d408-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2d408-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->