# <a name="plannerplandetails-resource-type"></a>Tipo de recurso plannerPlanDetails


O recurso **plannerPlanDetails** representa as informações adicionais sobre um plano. Cada objeto [plan](plannerplan.md) tem um objeto de detalhes.


### <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerPlanDetails](../api/plannerplandetails_get.md) | [plannerPlanDetails](plannerplandetails.md) |Leia as propriedades e as relações do objeto **plannerPlanDetails**.|
|[Atualizar](../api/plannerplandetails_update.md) | [plannerPlanDetails](plannerplandetails.md)    |Atualize o objeto **plannerPlanDetails**. |


### <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Um objeto que especifica as descrições das seis categorias que podem ser associadas a tarefas no plano|
|id|String| Somente leitura. ID dos detalhes dos planos. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.|
|sharedWith|[plannerUserIds](planneruserids.md)|Conjunto de identificações de usuários com o qual esse plano é compartilhado. Se você estiver aproveitando os Grupos do Office 365, use a API de Grupos para gerenciar a associação a um grupo para compartilhar o plano [do grupo](group.md). Você também pode adicionar membros existentes do grupo a essa coleção, embora isso não seja necessário para que eles possam acessar o plano do grupo. |

### <a name="relationships"></a>Relações
Nenhum


### <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->