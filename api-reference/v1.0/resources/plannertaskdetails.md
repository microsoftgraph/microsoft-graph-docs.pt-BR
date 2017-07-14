# Tipo de recurso plannerTaskDetails
<a id="plannertaskdetails-resource-type" class="xliff"></a>

O recurso **plannerTaskDetails** representa as informações adicionais sobre uma tarefa. Cada objeto [task](plannertask.md) tem um objeto de detalhes.


## Métodos
<a id="methods" class="xliff"></a>

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get plannerTaskDetails](../api/plannertaskdetails_get.md) | [plannerTaskDetails](plannertaskdetails.md) |Leia as propriedades e as relações do objeto **plannerTaskDetails**.|
|[Atualizar](../api/plannertaskdetails_update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Atualize o objeto **plannerTaskDetails**. |


## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|lista de verificação|[plannerChecklistItems](plannerchecklistitems.md)|A coleção de itens da lista de verificação na tarefa.|
|description|String|Descrição da tarefa|
|id|String| Somente leitura. ID dos detalhes da tarefa. Tem 28 caracteres e diferencia maiúsculas de minúsculas. [Formatar validação](planner_identifiers_disclaimer.md) é feito no serviço.|
|previewType|string|Isso define o tipo de visualização que aparece na tarefa. Os valores possíveis são: `automatic`, `noPreview`, `checklist`, `description` e `reference`. Quando definido como `automatic`, a visualização exibida é escolhida pelo aplicativo que exibe a tarefa.|
|referências|[plannerExternalReferences](plannerexternalreferences.md)|A coleção de referências na tarefa.|

## Relações
<a id="relationships" class="xliff"></a>
Nenhum


## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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