<span data-ttu-id="21e8b-p111">A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="21e8b-p111">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.|

## <span data-ttu-id="21e8b-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21e8b-206">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="21e8b-207">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="21e8b-207">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
