<span data-ttu-id="3a63f-p110">Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3a63f-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 254

{
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/mailfolders/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
      "wellKnownName": "wellKnownName-value"
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="3a63f-158">Veja também</span><span class="sxs-lookup"><span data-stu-id="3a63f-158">See also</span></span>

- [<span data-ttu-id="3a63f-159">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3a63f-159">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="3a63f-160">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="3a63f-160">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->