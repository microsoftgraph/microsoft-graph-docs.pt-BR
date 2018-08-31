# <a name="plannertaskdetails-resource-type"></a>Tipo de recurso plannerTaskDetails

O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |Leia as propriedades e as relações do objeto **plannerTaskDetails**.|
|[Atualizar](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Atualize o objeto **plannerTaskDetails**. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lista de verificação|[plannerChecklistItems](plannerchecklistitems.md)|A coleção de itens da lista de verificação na tarefa.|
|description|Sequência de caracteres|Descrição da tarefa|
|id|Cadeia de caracteres| Somente leitura. ID dos detalhes da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. A [validação de formato](planner_identifiers_disclaimer.md) é feita no serviço.|
|previewType|sequência de caracteres|Isto define o tipo de visualização que aparecerá na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Quando definido como `automatic` a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.|
|referências|[plannerExternalReferences](plannerexternalreferences.md)|A coleção de referências na tarefa.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
