<span data-ttu-id="1f15f-p118">Somente leitura. Anulável. Usado para renderizar a tarefa corretamente na exibição de quadro de tarefa quando agrupado por progresso.</span><span class="sxs-lookup"><span data-stu-id="1f15f-p118">Read-only. Nullable. Used to render the task correctly in the task board view when grouped by progress.</span></span>| Somente leitura. Anulável. Usado para renderizar a tarefa corretamente na exibição de quadro de tarefa quando agrupado por progresso.|

## <span data-ttu-id="1f15f-233">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f15f-233">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="1f15f-234">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f15f-234">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTask"
}-->

```json
{
  "activeChecklistItemCount": 1024,
  "appliedCategories": {"@odata.type": "microsoft.graph.plannerAppliedCategories"},
  "assigneePriority": "String",
  "assignments": {"@odata.type": "microsoft.graph.plannerAssignments"},
  "bucketId": "String",
  "checklistItemCount": 1024,
  "completedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "id": "String (identifier)",
  "orderHint": "String",
  "percentComplete": 1024,
  "planId": "String",
  "previewType": "string",
  "referenceCount": 1024,
  "startDateTime": "String (timestamp)",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTask resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->