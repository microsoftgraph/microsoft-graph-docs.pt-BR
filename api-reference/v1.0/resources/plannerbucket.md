# <a name="plannerbucket-resource-type"></a>Tipo de recurso plannerBucket

O recurso **plannerBucket** representa um Bucket (ou "coluna personalizada") para tarefas em um plano no Office 365. Ele está contido em um [plannerPlan](plannerPlan.md) e pode ter uma coleção de [plannerTasks](plannerTask.md).



### <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |Leia as propriedades e as relações do objeto **plannerBucket**.|
|[Listar plannerTasks](../api/plannerbucket_list_tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|
|[Criar](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)    | Crie um novo objeto **plannerBucket**. |
|[Atualizar](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)    |Atualize o objeto **plannerBucket**. |
|[Excluir](../api/plannerbucket_delete.md) | None |Exclua o objeto **plannerBucket**. |

### <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID do bucket. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.|
|nome|String|Nome do bucket.|
|orderHint|String|Dica usada para ordenar itens deste tipo em um modo de exibição de lista. O formato é definido como descrito [aqui](planner_order_hint_format.md).|
|planId|String|ID do plano ao qual o bucket pertence.|

### <a name="relationships"></a>Relações
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. A coleção de tarefas no bucket.|

### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->