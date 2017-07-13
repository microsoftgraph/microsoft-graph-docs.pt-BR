<span data-ttu-id="f12d7-p107">A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="f12d7-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|


## <span data-ttu-id="f12d7-200">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f12d7-200">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="f12d7-201">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f12d7-201">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <span data-ttu-id="f12d7-202">Veja também</span><span class="sxs-lookup"><span data-stu-id="f12d7-202">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="f12d7-203">Usar a consulta delta para controlar alterações nos dados do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f12d7-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="f12d7-204">Obter as alterações incrementais para as mensagens em uma pasta</span><span class="sxs-lookup"><span data-stu-id="f12d7-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
