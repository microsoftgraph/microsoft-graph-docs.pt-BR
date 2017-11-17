<span data-ttu-id="d956a-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`.</span><span class="sxs-lookup"><span data-stu-id="d956a-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span>
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`. 

## <span data-ttu-id="d956a-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d956a-112">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="d956a-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="d956a-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

<span data-ttu-id="d956a-114">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="d956a-114">Example:</span></span> 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->