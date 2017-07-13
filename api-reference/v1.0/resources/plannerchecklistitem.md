<span data-ttu-id="359bb-p104">Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido como descrito [aqui](planner_order_hint_format.md).</span><span class="sxs-lookup"><span data-stu-id="359bb-p104">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|Usado para definir a ordem relativa dos itens na lista de verificação. O formato é definido como descrito [aqui](planner_order_hint_format.md).|
|<span data-ttu-id="359bb-125">title</span><span class="sxs-lookup"><span data-stu-id="359bb-125">title</span></span>|<span data-ttu-id="359bb-126">String</span><span class="sxs-lookup"><span data-stu-id="359bb-126">String</span></span>|<span data-ttu-id="359bb-127">Título do item de lista de verificação</span><span class="sxs-lookup"><span data-stu-id="359bb-127">Title of the checklist item</span></span>|

## <span data-ttu-id="359bb-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="359bb-128">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="359bb-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="359bb-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->