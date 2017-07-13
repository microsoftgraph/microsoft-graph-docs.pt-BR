<span data-ttu-id="c99b2-p103">Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.</span><span class="sxs-lookup"><span data-stu-id="c99b2-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.|
|<span data-ttu-id="c99b2-135">referências</span><span class="sxs-lookup"><span data-stu-id="c99b2-135">references</span></span>|[<span data-ttu-id="c99b2-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c99b2-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="c99b2-137">A coleção de referências na tarefa.</span><span class="sxs-lookup"><span data-stu-id="c99b2-137">The collection of references on the task.</span></span>|

## <span data-ttu-id="c99b2-138">Relações</span><span class="sxs-lookup"><span data-stu-id="c99b2-138">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="c99b2-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c99b2-139">None</span></span>


## <span data-ttu-id="c99b2-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c99b2-140">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="c99b2-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c99b2-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->