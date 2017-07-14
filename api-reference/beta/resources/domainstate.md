# Tipo de recurso domainState
<a id="domainstate-resource-type" class="xliff"></a>

Representa o status das operações assíncronas agendadas em um domínio.

## Propriedades
<a id="properties" class="xliff"></a>

| Propriedade   | Tipo | Descrição |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | O carimbo de data/hora de quando a última atividade ocorreu. O valor é atualizado quando uma operação é agendada, a tarefa assíncrona começa e quando a operação é concluída. |
| operação | String | Tipo de operação assíncrona. Os valores podem ser *ForceDelete* ou *Verification* |
| status | String | Status atual da operação. <br> *Scheduled* – A operação foi agendada, mas não foi iniciada. <br> *InProgress* – A tarefa foi iniciada e está em andamento. <br> *Failed* - A operação falhou. |

## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->