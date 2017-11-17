# <a name="plannerappliedcategories-resource-type"></a>Tipo de recurso plannerAppliedCategories


O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md). Pode haver até seis categorias aplicadas a uma tarefa. Descrições de categorias, por exemplo, `category1`, `category2` etc., fazem parte do objeto [plan details](plannerplandetails.md). Este é um Tipo Aberto.

### <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`. 

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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

Exemplo: 

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