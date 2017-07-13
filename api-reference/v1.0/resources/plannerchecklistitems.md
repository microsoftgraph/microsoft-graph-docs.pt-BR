<span data-ttu-id="b316b-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser objetos [checklistItem](plannerchecklistitem.md). Um exemplo é mostrado abaixo. Para remover um item da lista de verificação, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="b316b-p102">Properties of an Open Type can be defined by the client. In this case, the client should provide **GUIDs** as properties and their values must be [checklistItem](plannerchecklistitem.md) objects. Example is shown below. To remove an item in the checklist, set the value of the property to `null`.</span></span>
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **GUIDs** como propriedades e seus valores devem ser objetos [checklistItem](plannerchecklistitem.md). Um exemplo é mostrado abaixo. Para remover um item da lista de verificação, defina o valor da propriedade como `null`.

## <span data-ttu-id="b316b-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b316b-111">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="b316b-112">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b316b-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItems"
}-->

```json
{
  "String-value":
  {
    "isChecked": true,
    "lastModifiedBy": "String-value",
    "lastModifiedByDateTime": "String(timestamp)",
    "orderHint": "String-value",
    "title": "String-value"
  }
}
```
<span data-ttu-id="b316b-113">// Exemplo</span><span class="sxs-lookup"><span data-stu-id="b316b-113">// Example</span></span>

```json
{
  "3a73c9dd-fb47-4230-9c0f-b80788fb0f9b": // client-generated GUID
  {
    "@odata.type": "microsoft.graph.checklistItem", // required in PATCH requests to edit the checklist on a task
    "isChecked": true,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0009005756397228702",
    "title": "Get stamps"
  },
  "5f36f5b2-1ec0-4c48-9c75-ed59429516c5":
  {
     "@odata.type": "microsoft.graph.checklistItem",
    "isChecked": false,
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedByDateTime": "2015-09-21T17:45:12.039Z",
    "orderHint": "0004105723397228784",
    "title": "Mail card at UPS"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItems resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->