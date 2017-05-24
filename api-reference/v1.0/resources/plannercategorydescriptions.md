# <a name="plannercategorydescriptions-resource-type"></a>Tipo de recurso plannerCategoryDescriptions

O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto [plan details](plannerplandetails.md). Pode haver até 6 categorias definidas. 


### <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|categoria1|String|O rótulo associado à Categoria 1.|
|categoria2|String|O rótulo associado à Categoria 2.|
|categoria3|String|O rótulo associado à Categoria 3.|
|categoria4|String|O rótulo associado à Categoria 4.|
|categoria5|String|O rótulo associado à Categoria 5.|
|categoria6|String|O rótulo associado à Categoria 6.|

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->