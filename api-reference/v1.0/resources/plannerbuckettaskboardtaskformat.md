# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>Tipo de recurso plannerBucketTaskBoardTaskFormat

O recurso **plannerBucketTaskBoardTaskFormat** representa as informações usadas para renderizar uma tarefa corretamente no modo de exibição Buckets do Quadro de Tarefas (um modo de exibição organizado por tarefas dentro dos buckets aos quais elas são atribuídas). Cada [tarefa](plannertask.md) terá um objeto **plannerBucketTaskBoardTaskFormat** associado a ela.


### <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat_get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |Leia as propriedades e as relações do objeto **plannerBucketTaskBoardTaskFormat**.|
|[Atualizar](../api/plannerbuckettaskboardtaskformat_update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)    |Atualize o objeto **plannerBucketTaskBoardTaskFormat**. |

### <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. A ID do recurso. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.|
|orderHint|String|Dica usada para ordenar tarefas no modo de exibição Bucket do Quadro de Tarefas. O formato é definido como descrito [aqui](planner_order_hint_format.md).|

### <a name="relationships"></a>Relações
Nenhum


### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->