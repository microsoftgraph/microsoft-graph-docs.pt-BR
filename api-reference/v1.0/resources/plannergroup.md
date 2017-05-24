# <a name="plannergroup-resource-type"></a>Tipo de recurso plannerGroup

O recurso **plannerGroup** oferece acesso aos recursos do Planner para um [grupo](group.md). Ele não contém quaisquer propriedades utilizáveis.

### <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/plannergroup_list_plans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha uma coleção de objetos **plannerPlan**.|

### <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. O identificador do **plannerGroup**|

### <a name="relationships"></a>Relações
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|plans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Retorna o [plannerPlans](plannerplan.md) que pertence ao grupo.|

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerGroup"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->