# <a name="plannerplan-resource-type"></a>Tipo de recurso plannerPlan

O recurso **plannerPlan** representa um plano no Office 365. Um plano pode pertencer a um [grupo](group.md) e conter uma coleção de [plannerTasks](plannerTask.md). Ele também pode ter uma coleção de [plannerBuckets](plannerBucket.md). Cada objeto de plano tem um objeto [details](plannerPlanDetails.md) que pode conter mais informações sobre o plano. Para saber mais sobre as relações entre grupos, planos e tarefas, confira o [Planner](planner_overview.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter plannerPlan](../api/plannerplan_get.md) | [plannerPlan](plannerplan.md) |Leia as propriedades e as relações do objeto **plannerPlan**.|
|[Listar buckets](../api/plannerplan_list_buckets.md) |Coleção [plannerBucket](plannerbucket.md)| Obter uma coleção de objetos **plannerBucket**.|
|[Listar tarefas](../api/plannerplan_list_tasks.md) |Coleção [plannerTask](plannertask.md)| Obter uma coleção de objetos **plannerTask**.|
|[Atualizar](../api/plannerplan_update.md) | [plannerPlan](plannerplan.md) |Atualize o objeto **plannerPlan**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Somente leitura. A data e a hora que o plano foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|Cadeia de caracteres| Somente leitura. ID do plano. Tem 28 caracteres de comprimento e diferencia maiúsculas de minúsculas. A[validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.|
|proprietário|Cadeia de caracteres|A ID do [Grupo](group.md) que possui o plano. Deve haver um grupo válido para que esse campo possa ser definido. Após definido, ele só poderá ser atualizado pelo proprietário.|
|título|Cadeia de caracteres|Obrigatório. Título do plano.|
|createdBy|[identitySet](identityset.md)|Somente leitura. O usuário que criou o plano.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|buckets|Coleção [plannerBucket](plannerbucket.md)| Somente leitura. Anulável. A coleção de buckets no plano.|
|detalhes|[plannerPlanDetails](plannerplandetails.md)| Somente leitura. Anulável. Outros detalhes sobre o plano.|
|tarefas|Coleção [plannerTask](plannertask.md)| Somente leitura. Anulável. A coleção de tarefas no plano.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->