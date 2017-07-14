# Tipo de recurso plannerUser
<a id="planneruser-resource-type" class="xliff"></a>

O recurso **plannerUser** oferece acesso aos recursos do Planner para um [usuário](user.md). Ele não contém quaisquer propriedades utilizáveis.


## Métodos
<a id="methods" class="xliff"></a>

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar planos](../api/planneruser_list_plans.md) |Coleção [plannerPlan](plannerplan.md)| Obtenha uma coleção de objetos **plannerPlan**.|
|[Listar tarefas](../api/planneruser_list_tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|

## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. O identificador do plannerUser|

## Relações
<a id="relationships" class="xliff"></a>
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|plans|Coleção [plannerPlan](plannerplan.md)| Somente leitura. Anulável. Returna o [plannerTasks](plannertask.md) atribuídos ao usuário.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. Returna o objeto [plannerTasks](plannerplan.md) atribuído ao usuário.|

## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->